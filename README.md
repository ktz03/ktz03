<div align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Cascadia+Code&amp;weight=700&amp;size=17&amp;color=0078D7&amp;center=true&amp;vCenter=true&amp;width=400&amp;height=40&amp;pause=100000&amp;lines=Hi%2C+I%27m+LI.+AI+Ecosystem+Builder" alt="Hi, I'm LI. AI Ecosystem Builder."/>
  <p>Core contributor to <strong>Microsoft Agent Framework</strong>, <strong>ByteDance’s OpenViking</strong>, and <strong>Tencent’s ncnn</strong>.<br/>I build reliability into the systems that agents depend on, from workflow recovery and persistent memory to inference on edge devices.</p>
  <p>My research focus is <strong>embodied AI and world models</strong>. How should an agent change its next move when the world differs from its prediction?</p>
  <p><code>Shenzhen, China</code> &nbsp;·&nbsp; <a href="https://www.zhumengmiao.me">Website</a> &nbsp;·&nbsp; <a href="https://x.com/ktz03">X</a></p>
</div>

## Three layers of AI infrastructure

| Project and role | What changed upstream |
| --- | --- |
| **[Microsoft Agent Framework](https://github.com/microsoft/agent-framework)** · Core contributor | **Workflow recovery.** I changed thread snapshots to retain a human reply so a workflow can resume with the answer already given. [Contribution record](https://github.com/ktz03/ktz03/blob/4ab7c8698e5a239b1a74b68093347712656016c8/README.md?plain=1#L61) · [Historical PR #8273](https://github.com/microsoft/agent-framework/pull/8273) |
| **[ByteDance’s OpenViking](https://github.com/volcengine/OpenViking)** · Core contributor | **Agent memory.** I coauthored the LangChain fix that lets a restored conversation retain what was said, who said it, and which tools were called. [PR #6275, opened by @ehz0ah](https://github.com/volcengine/OpenViking/pull/6275) · [Coauthor credit](https://github.com/volcengine/OpenViking/commit/b1d0fa51ef253716fdec819615918352e97dfd41) |
| **[Tencent’s ncnn](https://github.com/Tencent/ncnn)** · Core contributor | **Inference reliability.** I stabilized LogSumExp on CPU and Vulkan. Both backends now return a finite result for inputs like `[1000, 1000]`. [PR #7055](https://github.com/Tencent/ncnn/pull/7055) · [Numerical example](notes/ncnn-logsumexp.md) |

As of November 25, 2026, **109 PRs I opened have merged across 37 upstream projects**, including **65** in the three projects above. [View public merged PRs](https://github.com/search?q=author%3Aktz03+is%3Apr+is%3Amerged+is%3Apublic+-user%3Aktz03&type=pullrequests).

## Collaboration

- [@ehz0ah](https://github.com/ehz0ah) brought our LangChain fixes together and opened the OpenViking PR. [How we preserved conversation history](notes/openviking-langchain-collaboration.md).
- In Tencent ncnn, [@nihui](https://github.com/nihui) and I share credit on three merged PRs. In one, we changed how the pnnx converter stores boolean constants. [PR #7006](https://github.com/Tencent/ncnn/pull/7006) · [Coauthor credit](https://github.com/Tencent/ncnn/commit/8bc95a1e7fe430c0d6f988f6318c1a8791b78062).

<details>
<summary><strong>View 14 coauthored PRs</strong> · OpenViking 8 · ncnn 3 · Agent Framework 2 · Zuko 1</summary>

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

## Embodied AI and world models

A robot can finish a grasp motion while the object stays on the table. That gap is the problem I’m working on in embodied AI. A world model predicts what an action will change. The next observation gives the agent evidence to continue, retry, or choose a different action.

## Agent developer tools I created

- [**handoff-pack**](https://github.com/ktz03/handoff-pack) carries context between models or sessions. It prioritizes instructions, tool errors, and recent messages, then writes a compact Markdown or JSON handoff. [Example conversation](https://github.com/ktz03/handoff-pack/blob/master/examples/long.session.json).
- [**traj-wash**](https://github.com/ktz03/traj-wash) prepares agent trajectories for evaluation and supervised fine-tuning. It keeps the first failed step as evidence and trims the retries that follow. In the [seven-step example](https://github.com/ktz03/traj-wash/blob/master/examples/bad.trajectory.json), four steps remain.

<details>
<summary><strong>Full contribution record and more project cases</strong></summary>

[Browse publicly searchable authored PRs](https://github.com/search?q=author%3Aktz03+is%3Apr+is%3Amerged+is%3Apublic+-user%3Aktz03&type=pullrequests).

### 🤖 [Microsoft Agent Framework](https://github.com/microsoft/agent-framework) · Agent workflows

`Agent workflows` · `Recovery` · `Checkpoints`

Agent orchestration, recoverable workflows and checkpoints. In the historical snapshot: **30 authored** and **2 coauthored** PRs.

- **Recoverable human-in-the-loop workflows:** Preserved user text in thread snapshots. [Microsoft Agent Framework #8273](https://github.com/microsoft/agent-framework/pull/8273).
- Fixed [BreakLoop handling in declarative workflows](https://github.com/microsoft/agent-framework/pull/9091).

<sub>The repository and historical PR links were unavailable when checked on November 18, 2026; the figures are from earlier verified records.</sub>

### 🧠 [OpenViking](https://github.com/volcengine/OpenViking) · Agent memory

`Agent memory` · `Context` · `Integrations`

Memory, context and agent integrations. The November 25 count includes **28 authored** and **8 coauthored** PRs.

- Fixed [CR-delimited MCP event stream parsing](https://github.com/volcengine/OpenViking/pull/5973).
- **Windows CLI discovery:** The launcher could miss an existing development executable; the fix selects the Windows filename while preserving the existing lookup order. [OpenViking #7251](https://github.com/volcengine/OpenViking/pull/7251) · [Case study](notes/openviking-windows-cli.md).

### ⚙️ [Tencent ncnn](https://github.com/Tencent/ncnn) · Inference

`Inference` · `Correctness` · `Portability`

Inference correctness, portability and bindings. In the historical snapshot: **7 authored** and **3 coauthored** PRs.

- **Numerically stable inference:** Extreme finite inputs could produce infinities; the fix stabilizes LogSumExp on CPU and Vulkan. [ncnn #7055](https://github.com/Tencent/ncnn/pull/7055) · [Case study](notes/ncnn-logsumexp.md).
- Addressed [FP16 GELU overflow on ARM and RISC-V](https://github.com/Tencent/ncnn/pull/7060).

- **Tencent ncnn:** Improved [bool MemoryData handling in pnnx](https://github.com/Tencent/ncnn/pull/7006), with [@nihui](https://github.com/nihui) · [coauthor credit](https://github.com/Tencent/ncnn/commit/8bc95a1e7fe430c0d6f988f6318c1a8791b78062).
- **[Zuko](https://github.com/probabilists/zuko):** Included [broadcast bounds in truncated batch shapes](https://github.com/probabilists/zuko/pull/83), with [@francois-rozet](https://github.com/francois-rozet) · [coauthor credit](https://github.com/probabilists/zuko/commit/c000b19adbf0c0e83c612b3e826e896bd967fcf7).

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
