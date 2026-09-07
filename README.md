### Hi, I'm ktz03

**Agent runtime / memory systems** — small upstream fixes that survive review, plus local-first Agent tooling.

---

### Open source (selected)

**[volcengine/OpenViking](https://github.com/volcengine/OpenViking)** — external contributor (merged):

| PR | Focus |
|----|--------|
| [#4702](https://github.com/volcengine/OpenViking/pull/4702) | pi-extension: watermark + drain budget (review follow-up) |
| [#4643](https://github.com/volcengine/OpenViking/pull/4643) | dsh-plugin: parallel profile + recall on pre-step |
| [#4608](https://github.com/volcengine/OpenViking/pull/4608) | opencode-plugin: isolate `flushAll` session failures |
| [#4040](https://github.com/volcengine/OpenViking/pull/4040) | rerank: send `top_n` on OpenAI-compatible path |

Also shipping deeper threads under review (e.g. [pending-queue batch replay](https://github.com/volcengine/OpenViking/pull/4714), [path filters in staging](https://github.com/volcengine/OpenViking/pull/4604)) — design iteration with maintainers, not drive-by patches.

Occasional fixes elsewhere: [Tencent/ncnn#6906](https://github.com/Tencent/ncnn/pull/6906).

---

### Building

| Repo | One-liner |
|------|-----------|
| **[traj-wash](https://github.com/ktz03/traj-wash)** | Find failure onset → wash cascade fails → export clean Agent trajectories |
| **[handoff-pack](https://github.com/ktz03/handoff-pack)** | Compress OpenAI-compatible `messages[]` into a paste-ready model handoff pack |
| **[AIFlowHub](https://github.com/ktz03/AIFlowHub)** | NL → executable AI workflows / agents (skill routing, validation, private deploy) |
| **[Site Agent](https://zhumengmiao.me)** | Guided navigation Agent (SSE, context engineering, allowlisted deep-links) |

---

### Focus

Python · TypeScript · Agent / LLM apps · memory & tool loops · product+eng ownership

*Prefer merged, reviewed work over open PR volume.*
