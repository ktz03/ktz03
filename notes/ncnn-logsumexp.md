# ncnn: stabilizing LogSumExp on CPU and Vulkan

**Project:** Tencent ncnn · **Area:** inference correctness · **Outcome:** merged upstream

[PR #7055](https://github.com/Tencent/ncnn/pull/7055) · [Issue #7053](https://github.com/Tencent/ncnn/issues/7053)

## Problem

Computing `log(sum(exp(x)))` directly could return infinities for finite inputs such as `[1000, 1000]` and `[-1000, -1000]`.

## Change

Use maximum-shifted LogSumExp to improve numerical stability. The change covers CPU and Vulkan paths while retaining existing operator behavior for the tested cases.

## Evidence and scope

The PR describes focused regression and reference comparisons for CPU and Vulkan, including large-magnitude and non-finite inputs. Its reported validation is operator-level; it does not claim full-model coverage or a performance improvement. See the PR for the individual test environments and limitations.
