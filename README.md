# ktz03

### Making agent systems more reliable

I contribute upstream fixes to **OpenViking, Microsoft Agent Framework and Tencent ncnn**, focusing on **agent memory, workflow recovery and inference correctness**.

**42 merged PRs across 9 upstream projects · 36 merges in my three core projects**

[Explore merged contributions](https://github.com/search?q=author%3Aktz03+is%3Apr+is%3Amerged+is%3Apublic&type=pullrequests) · [Website](https://zhumengmiao.me)

## Core work

- **[OpenViking](https://github.com/volcengine/OpenViking) — 15 merged PRs.** Memory and retrieval integrations, MCP streams, transport errors and context handling.
- **[Microsoft Agent Framework](https://github.com/microsoft/agent-framework) — 15 merged PRs.** Conversation persistence, human-in-the-loop recovery and declarative workflow correctness.
- **[Tencent ncnn](https://github.com/Tencent/ncnn) — 6 merged PRs.** Numerical correctness, portability and Python bindings.

## Selected upstream fixes

- **Agent integration:** [Parse CR-delimited MCP event streams](https://github.com/volcengine/OpenViking/pull/5973) and [preserve response-body transport failures](https://github.com/volcengine/OpenViking/pull/5661).
- **Workflow recovery:** [Persist HITL user text in thread snapshots](https://github.com/microsoft/agent-framework/pull/8273) and [honor BreakLoop in declarative workflows](https://github.com/microsoft/agent-framework/pull/9091).
- **Inference correctness:** [Fix even-sized LRN channel windows](https://github.com/Tencent/ncnn/pull/7070) and [retain Python custom-layer factories for their required lifetime](https://github.com/Tencent/ncnn/pull/7049).

My contribution loop: **reproduce the failure → preserve normal behavior → add a focused regression → close the review loop**.

Other merged work spans **TensorLy, PydanticAI, Qdrant Client, sklearn-onnx, RapidOCR and pyts**.

## Tools & collaboration

[handoff-pack](https://github.com/ktz03/handoff-pack) — turn chat `messages[]` into a paste-ready handoff pack.

Open to upstream collaboration and engineering opportunities around agent infrastructure, memory systems and model tooling.

*Public contribution snapshot: October 14, 2026. The headline counts merges into repositories owned by others that are not forks; personal repositories and external forks are excluded.*
