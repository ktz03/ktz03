# ktz03

### AI Ecosystem Builder

Core contributor to **Microsoft Agent Framework**, **ByteDance's OpenViking**, and **Tencent's ncnn**. Working on **embodied AI and world models**.

I connect agent orchestration, memory and context, and inference runtimes through upstream fixes and collaboration.

[Personal website](https://www.zhumengmiao.me) · [X / Twitter](https://x.com/ktz03) · [Merged PRs](https://github.com/search?q=author%3Aktz03+is%3Apr+is%3Amerged+is%3Apublic+-user%3Aktz03&type=pullrequests)

## Open-source contributions

**113 merged upstream PRs: 99 authored and 14 additional coauthored · 35 upstream projects**

This is a public upstream snapshot from **November 14, 2026**. Coauthored work is a verified lower bound, not a complete count.

| Ecosystem | Authored | Coauthored | Areas |
| --- | ---: | ---: | --- |
| [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) | 30 | 2 | Agent orchestration, workflow recovery and checkpoints |
| [OpenViking](https://github.com/volcengine/OpenViking) | 22 | 8 | Agent memory, integrations and context handling |
| [Tencent ncnn](https://github.com/Tencent/ncnn) | 7 | 3 | Inference correctness, portability and bindings |
| [Zuko](https://github.com/probabilists/zuko) | — | 1 | Numerical correctness |

Microsoft Agent Framework's repository and related links are currently unavailable; its figures above reflect previously verified historical records.

## Selected authored work

- **Agent memory and integration — OpenViking:** Fixed [CR-delimited MCP event stream parsing](https://github.com/volcengine/OpenViking/pull/5973) and [Windows development CLI executable discovery](https://github.com/volcengine/OpenViking/pull/7251).
- **Agent orchestration — Microsoft Agent Framework:** Contributed fixes for [HITL user text in thread snapshots](https://github.com/microsoft/agent-framework/pull/8273) and [BreakLoop in declarative workflows](https://github.com/microsoft/agent-framework/pull/9091). These historical PR links may currently be unavailable.
- **Inference — Tencent ncnn:** Improved [LogSumExp stability on CPU and Vulkan](https://github.com/Tencent/ncnn/pull/7055) and addressed [FP16 GELU overflow on ARM and RISC-V](https://github.com/Tencent/ncnn/pull/7060).

## Collaboration and coauthored work

These contributions landed through PRs opened by other authors, with coauthor credit retained in the upstream commits.

- **OpenViking:** Preserved [conversation text, roles and tool history](https://github.com/volcengine/OpenViking/pull/6275), with [@ehz0ah](https://github.com/ehz0ah) · [coauthor credit](https://github.com/volcengine/OpenViking/commit/b1d0fa51ef253716fdec819615918352e97dfd41).
- **Tencent ncnn:** Improved [bool MemoryData handling in pnnx](https://github.com/Tencent/ncnn/pull/7006), with [@nihui](https://github.com/nihui) · [coauthor credit](https://github.com/Tencent/ncnn/commit/8bc95a1e7fe430c0d6f988f6318c1a8791b78062).
- **Zuko:** Included [broadcast bounds in truncated batch shapes](https://github.com/probabilists/zuko/pull/83), with [@francois-rozet](https://github.com/francois-rozet) · [coauthor credit](https://github.com/probabilists/zuko/commit/c000b19adbf0c0e83c612b3e826e896bd967fcf7).

<details>
<summary><strong>View 14 coauthored PRs</strong></summary>

- [volcengine/OpenViking#7040](https://github.com/volcengine/OpenViking/pull/7040) — fix(langchain): preserve Unicode archive query terms · PR by [@ehz0ah](https://github.com/ehz0ah) · [coauthor credit](https://github.com/volcengine/OpenViking/commit/8dc1121102ab80378bac6e29a5ec2be798839717)
- [probabilists/zuko#83](https://github.com/probabilists/zuko/pull/83) — Include broadcast bounds in Truncated batch shape · PR by [@francois-rozet](https://github.com/francois-rozet) · [coauthor credit](https://github.com/probabilists/zuko/commit/c000b19adbf0c0e83c612b3e826e896bd967fcf7)
- [volcengine/OpenViking#6479](https://github.com/volcengine/OpenViking/pull/6479) — fix(langchain): isolate session commits and report reset failures · PR by [@ehz0ah](https://github.com/ehz0ah) · [coauthor credit](https://github.com/volcengine/OpenViking/commit/2260f6899e882a8d7f693cca4dd8559dfc66b8cf)
- [volcengine/OpenViking#6404](https://github.com/volcengine/OpenViking/pull/6404) — fix(langchain): honor nested filters and index field selectors · PR by [@ehz0ah](https://github.com/ehz0ah) · [coauthor credit](https://github.com/volcengine/OpenViking/commit/d5022f57559fef83b14c63789ca75a0b2dc7a9c9)
- [volcengine/OpenViking#6342](https://github.com/volcengine/OpenViking/pull/6342) — fix(langchain): preserve Store reads and namespace discovery · PR by [@ehz0ah](https://github.com/ehz0ah) · [coauthor credit](https://github.com/volcengine/OpenViking/commit/6ec6116b7beb83d99cc87303076613cfabc47731)
- [volcengine/OpenViking#6338](https://github.com/volcengine/OpenViking/pull/6338) — fix(langchain): preserve recall inputs and context metadata · PR by [@ehz0ah](https://github.com/ehz0ah) · [coauthor credit](https://github.com/volcengine/OpenViking/commit/7c12d3062fecd5a37cebc61087d1a4eb01826108)
- [volcengine/OpenViking#6324](https://github.com/volcengine/OpenViking/pull/6324) — fix(langchain): align Store deletion, validation and removal errors · PR by [@ehz0ah](https://github.com/ehz0ah) · [coauthor credit](https://github.com/volcengine/OpenViking/commit/d8f485496451f4b70a5485e0bb9d85ace299d291)
- [volcengine/OpenViking#6275](https://github.com/volcengine/OpenViking/pull/6275) — fix(langchain): preserve conversation text, roles and tool history · PR by [@ehz0ah](https://github.com/ehz0ah) · [coauthor credit](https://github.com/volcengine/OpenViking/commit/b1d0fa51ef253716fdec819615918352e97dfd41)
- [microsoft/agent-framework#8284](https://github.com/microsoft/agent-framework/pull/8284) — Python: add public TypedDict for AgentExecutor checkpoint state (#8201) · PR by [@FOWEPJF255](https://github.com/FOWEPJF255) · [coauthor credit](https://github.com/microsoft/agent-framework/commit/435012e55c6cbfad659b4715b84132607d495bcc)
- [microsoft/agent-framework#8163](https://github.com/microsoft/agent-framework/pull/8163) — Python: include checkpoint_id on AG-UI interrupt metadata (#8150) · PR by [@FOWEPJF255](https://github.com/FOWEPJF255) · [coauthor credit](https://github.com/microsoft/agent-framework/commit/3b110ade39ea798486b1060f40ee9e2c6329d0ae)
- [Tencent/ncnn#7006](https://github.com/Tencent/ncnn/pull/7006) — pnnx: store bool MemoryData attributes as raw int8 · PR by [@nihui](https://github.com/nihui) · [coauthor credit](https://github.com/Tencent/ncnn/commit/8bc95a1e7fe430c0d6f988f6318c1a8791b78062)
- [Tencent/ncnn#7003](https://github.com/Tencent/ncnn/pull/7003) — layer param hardening · PR by [@nihui](https://github.com/nihui) · [coauthor credit](https://github.com/Tencent/ncnn/commit/5ea98309e3e203215e860692ff8226072c0658a4)
- [Tencent/ncnn#6989](https://github.com/Tencent/ncnn/pull/6989) — harden net loading · PR by [@nihui](https://github.com/nihui) · [coauthor credit](https://github.com/Tencent/ncnn/commit/0cdc3351c8407657b30746df9ffeb0251ca7112d)
- [volcengine/OpenViking#4692](https://github.com/volcengine/OpenViking/pull/4692) — fix(pi-extension): replay offline backlog through the batch endpoint · PR by [@ZaynJarvis](https://github.com/ZaynJarvis) · [coauthor credit](https://github.com/volcengine/OpenViking/commit/854ff4ceb052d0b2586dd5ffdf9d6156f0e1c79d)

</details>

<details>
<summary><strong>More selected upstream work</strong></summary>

## Selected work: fixes that landed upstream

- **Agent integrations:** [Handle CR-delimited MCP event streams](https://github.com/volcengine/OpenViking/pull/5973) and [support bracketed IPv6 bind addresses in the OpenWebUI integration](https://github.com/volcengine/OpenViking/pull/6106).
- **Durable workflows:** [Persist HITL user text in thread snapshots](https://github.com/microsoft/agent-framework/pull/8273) and [honor BreakLoop in declarative workflows](https://github.com/microsoft/agent-framework/pull/9091).
- **Inference runtimes:** [Correct even-sized LRN channel windows](https://github.com/Tencent/ncnn/pull/7070) and [retain Python custom-layer factories for their required lifetime](https://github.com/Tencent/ncnn/pull/7049).
- **Python infrastructure:** [Reject readonly buffers before consuming buffered data in fsspec](https://github.com/fsspec/filesystem_spec/pull/2260) and [preserve defaultdict batch conversion in PyTorch Ignite](https://github.com/pytorch/ignite/pull/3891).
- **Numerical correctness:** [Fix complex-weight CP tensor norms in TensorLy](https://github.com/tensorly/tensorly/pull/656) — [walkthrough and minimal reproduction](notes/tensorly-complex-cp-norm.md). [Prevent overflow when summing probability-selection fitness in PyGAD](https://github.com/ahmedfgad/GeneticAlgorithmPython/pull/381).

My contribution loop: **reproduce the failure → preserve normal behavior → add a focused regression → close the review loop**.

Further merged work includes **TensorLy, PydanticAI, Qdrant Client, sklearn-onnx, RapidOCR, pyts, scikit-lego and Patsy**.

</details>

## Current direction

Working on **embodied AI and world models**, building on experience across agent workflows, memory and inference.

Based in **Shenzhen, China**. Open to collaboration around AI agents, memory systems, inference and embodied AI.
