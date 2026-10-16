# ktz03

### AI OSS Ecosystem Connector

**Healthcare CRO AI Product Manager · Upstream Contributor · AI Agent & 3D Builder**

I connect **healthcare AI product work** with the **open-source infrastructure behind agent systems**. My work spans product decisions, upstream engineering and building AI agents and 3D spaces.

**50+ merged upstream PRs · 14 upstream projects · 37 merges across OpenViking, Microsoft Agent Framework and Tencent ncnn**

From persistent agent memory and recoverable workflows to inference edge cases, I contribute focused fixes that make AI systems more dependable—and work with upstream reviewers to get them landed.

[Merged contributions](https://github.com/search?q=author%3Aktz03+is%3Apr+is%3Amerged+is%3Apublic+-user%3Aktz03&type=pullrequests) · [X / Twitter](https://x.com/ktz03) · [Personal website](https://www.zhumengmiao.me)

## Upstream impact

- **[OpenViking](https://github.com/volcengine/OpenViking) — 16 merged PRs.** Agent memory and retrieval integrations, MCP streams, transport handling and OpenWebUI compatibility.
- **[Microsoft Agent Framework](https://github.com/microsoft/agent-framework) — 15 merged PRs.** Conversation persistence, human-in-the-loop recovery and declarative workflow correctness.
- **[Tencent ncnn](https://github.com/Tencent/ncnn) — 6 merged PRs.** Inference correctness, portability and Python binding lifetimes.

## Selected work: fixes that landed upstream

- **Agent integrations:** [Handle CR-delimited MCP event streams](https://github.com/volcengine/OpenViking/pull/5973) and [support bracketed IPv6 bind addresses in the OpenWebUI integration](https://github.com/volcengine/OpenViking/pull/6106).
- **Durable workflows:** [Persist HITL user text in thread snapshots](https://github.com/microsoft/agent-framework/pull/8273) and [honor BreakLoop in declarative workflows](https://github.com/microsoft/agent-framework/pull/9091).
- **Inference runtimes:** [Correct even-sized LRN channel windows](https://github.com/Tencent/ncnn/pull/7070) and [retain Python custom-layer factories for their required lifetime](https://github.com/Tencent/ncnn/pull/7049).
- **Python infrastructure:** [Reject readonly buffers before consuming buffered data in fsspec](https://github.com/fsspec/filesystem_spec/pull/2260) and [preserve defaultdict batch conversion in PyTorch Ignite](https://github.com/pytorch/ignite/pull/3891).
- **Numerical stability:** [Prevent overflow when summing probability-selection fitness in PyGAD](https://github.com/ahmedfgad/GeneticAlgorithmPython/pull/381).

My contribution loop: **reproduce the failure → preserve normal behavior → add a focused regression → close the review loop**.

Further merged work includes **TensorLy, PydanticAI, Qdrant Client, sklearn-onnx, RapidOCR, pyts, scikit-lego and Patsy**.

## The crossover

- **Healthcare × AI product:** currently an AI product manager in a healthcare CRO, bringing a domain and product perspective to AI systems.
- **Agents × infrastructure:** building AI agents while contributing to memory, workflow recovery, model conversion and inference reliability upstream.
- **3D × personal IP:** working on 3D spaces and developing an anime-inspired personal identity through [zhumengmiao.me](https://www.zhumengmiao.me).

## Projects I build

- **[AIFlowHub](https://github.com/ktz03/AIFlowHub)** — my independent continuation of Flowise, focused on skill-driven workflow generation, cloud/local LLM integration and quota, cost and evaluation tooling.
- **[handoff-pack](https://github.com/ktz03/handoff-pack)** — a CLI that turns agent conversation messages into a compact handoff pack for the next model or session.

Based in **Shenzhen, China**. Open to collaboration across **healthcare AI products, agent infrastructure, open-source tooling and 3D experiences**.

*Contribution metrics use the October 16, 2026, 15:11 UTC+8 public snapshot. Counts cover merged PRs in repositories owned by others that are not forks; personal repositories and external forks are excluded.*
