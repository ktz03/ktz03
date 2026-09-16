### Hi, I'm ktz03

**Agent runtime / memory systems** — small upstream fixes that survive review, plus local-first Agent tooling.

Also contributing to **[Tencent/ncnn](https://github.com/Tencent/ncnn)** (mobile inference) alongside Agent/memory work.

---

### Open source (selected)

**[volcengine/OpenViking](https://github.com/volcengine/OpenViking)** — external contributor (merged):

| PR | Focus |
|----|--------|
| [#4875](https://github.com/volcengine/OpenViking/pull/4875) | fs: normalize S3 virtual-directory `ls` rows |
| [#4848](https://github.com/volcengine/OpenViking/pull/4848) | bot: strip client `openviking_connection` on proxy forward |
| [#4825](https://github.com/volcengine/OpenViking/pull/4825) | web-studio: honor task API status |
| [#4702](https://github.com/volcengine/OpenViking/pull/4702) | pi-extension: watermark + drain budget (review follow-up) |
| [#4643](https://github.com/volcengine/OpenViking/pull/4643) | dsh-plugin: parallel profile + recall on pre-step |
| [#4608](https://github.com/volcengine/OpenViking/pull/4608) | opencode-plugin: isolate `flushAll` session failures |

Deeper threads still under review (e.g. [pending-queue batch replay](https://github.com/volcengine/OpenViking/pull/4714)) — design iteration with maintainers, not drive-by patches.

**[microsoft/agent-framework](https://github.com/microsoft/agent-framework)** — merged:

| PR | Focus |
|----|--------|
| [#8274](https://github.com/microsoft/agent-framework/pull/8274) | mcp: do not duplicate `structuredContent` when content present |
| [#8272](https://github.com/microsoft/agent-framework/pull/8272) | checkpoint: preserve dicts whose keys collide after `str()` |
| [#8149](https://github.com/microsoft/agent-framework/pull/8149) | ag-ui: dedupe client-replayed transcripts on resume |

**[Tencent/ncnn](https://github.com/Tencent/ncnn)** — merged + open:

| PR | Focus |
|----|--------|
| [#6906](https://github.com/Tencent/ncnn/pull/6906) | allocator: drop `_POSIX_C_SOURCE` from `posix_memalign` branch |
| [#6954](https://github.com/Tencent/ncnn/pull/6954) *(open)* | mat: zero-init freshly allocated Mat buffers |
| [#6952](https://github.com/Tencent/ncnn/pull/6952) *(open)* | vulkan: omit zero-count descriptor pool sizes |
| [#6956](https://github.com/Tencent/ncnn/pull/6956) *(open)* | pnnx: widen bool MemoryData attributes to fp32 in `.bin` |

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

Python · TypeScript · C++ (ncnn) · Agent / LLM apps · memory & tool loops · product+eng ownership

*Prefer merged, reviewed work over open PR volume.*
