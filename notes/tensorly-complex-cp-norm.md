# When a complex weight makes a tensor norm imaginary

A Frobenius norm should be real and nonnegative. In TensorLy, a CP tensor with a complex weight could instead produce an imaginary norm.

The smallest example has one weight, `1j`, and two real factor columns, `[1, 2]` and `[3, 4]`. The represented tensor is:

```text
[[3j, 4j],
 [6j, 8j]]
```

Its squared Frobenius norm is `9 + 16 + 36 + 64 = 125`, so its norm is about `11.1803398875`. The old CP norm calculation returned `11.1803398875j`.

## The fix

The weight product needs a complex conjugate: `w[r] * conj(w[s])`. Multiplying the two weights directly makes `1j * 1j = -1`; conjugation gives `1j * -1j = 1`.

The fix also takes the real part of the squared norm before the square root and exposes the backend `real` operation through TensorLy's existing dispatch mechanism. This keeps the mathematical result real and handles backends whose complex square-root operation is unavailable on CPU.

The regression compares `cp_norm` and `CPTensor.norm()` with the dense tensor's norm. It covers complex64/complex128 weights, real and complex factors, weighted and unweighted inputs, output dtype, and float32/float64 controls.

## Reproduce the arithmetic without dependencies

```python
import cmath
import math

weight = 1j
factor_energy = (1**2 + 2**2) * (3**2 + 4**2)

old_norm = cmath.sqrt(weight * weight * factor_energy)
fixed_norm = math.sqrt((weight * weight.conjugate() * factor_energy).real)

print(old_norm)    # 11.180339887498949j
print(fixed_norm)  # 11.180339887498949
```

## Upstream result

[TensorLy PR #656](https://github.com/tensorly/tensorly/pull/656) was authored by [@ktz03](https://github.com/ktz03) and merged by [@aarmey](https://github.com/aarmey) on October 11, 2026. It extends the earlier complex-factor support in [PR #423](https://github.com/tensorly/tensorly/pull/423) to complex weights.

- [Merged change and regression tests](https://github.com/tensorly/tensorly/pull/656/files)
- [Merge commit](https://github.com/tensorly/tensorly/commit/b75ca108ac0a04892cd0800d06a9528fcb2e35f6)
- [Original bug report](https://github.com/tensorly/tensorly/issues/655)

The useful check is simple: compare the compact representation's norm with the dense tensor it represents, and keep real-valued inputs as controls.
