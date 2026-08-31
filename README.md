<div align="center">

# Tim White

### AI agents · security engineering

I work on agent runtimes, evaluation harnesses, and security tooling, with an interest in systems that are observable, recoverable, and grounded in external evidence.

[Current interests](#current-interests) · [Projects](#projects) · [Security work](#security-work) · [Working preferences](#working-preferences) · [中文简介](#中文简介) · [Email](mailto:twhite.zh@gmail.com)

</div>

---

## Current interests

My background is in offensive security. More recently, I have been spending time on agent systems and on the infrastructure around them.

| Area | Topics |
| --- | --- |
| **Agent runtimes & harnesses** | Tools, durable state, context management, live steering, and recovery. |
| **Evaluation & self-improvement** | Verifier feedback, reproducible trajectories, bounded changes, and regression checks. |
| **AI × security** | Agent-readable interfaces for reverse engineering and security analysis, with explicit evidence and safety boundaries. |

## Projects

| Project | Area | Notes |
| --- | --- | --- |
| **[AutoRE-CLI](https://github.com/timwhitez/AutoRE-CLI)** | AI × reverse engineering | A bounded static-analysis interface for humans and agents, with traceable JSON, CFG, and IL output and explicit evidence states. |
| **[Aegis Agent](https://github.com/timwhitez/aegis-agent)** | Local agent runtime · Go | A local agent harness with a Web console, tools, durable session state, compaction, live steering, provider adapters, and safety boundaries. |
| **[HarnessEvolver](https://github.com/timwhitez/harness-evolver)** | Coding-agent evaluation · Rust/Python | An experimental harness that uses Harbor and verifier output to study failures and review bounded harness changes. |
| **[dsh-self-evolving](https://github.com/timwhitez/dsh-self-evolving)** | Self-evolution controller · TypeScript | Experiments with resumable candidate generation, isolated admission and evaluation, lineage, budgets, and trust boundaries. |

[ida-pro-skill](https://github.com/timwhitez/ida-pro-skill) is a small companion project for connecting coding agents to a live IDA database through a local, bounded interface.

## Security work

A few public projects from my earlier and ongoing security work:

| Project | Area | Notes |
| --- | --- | --- |
| **[Doge-Gabh](https://github.com/timwhitez/Doge-Gabh)** | Windows internals · Go | A native-API toolkit covering PE parsing, API hashing, ntdll remapping, syscall-related experiments, DLL unhooking, and proxy calls. |
| **[BinHol](https://github.com/timwhitez/BinHol)** | PE binary engineering · Go | A PE rewriting tool with function patching, entry-point changes, TLS injection, certificate-table handling, and dynamic patch sizing. |
| **[crawlergo_x_XRAY](https://github.com/timwhitez/crawlergo_x_XRAY)** | Web attack-surface automation · Python | Connects dynamic crawling with passive vulnerability scanning for repeatable request discovery and analysis. |
| **[Cobalt-Strike-Aggressor-Scripts](https://github.com/timwhitez/Cobalt-Strike-Aggressor-Scripts)** | Operator automation | A collection of Aggressor scripts developed around practical red-team workflows. |

These repositories are published for authorized research, engineering, and defensive understanding.

## Working preferences

- Keep the harness relatively simple and leave open-ended reasoning to the model where practical.
- Prefer external verification to a model's own report of success.
- Keep validated facts, inferences, and unresolved questions separate.
- Design long-running work so it can be inspected, resumed, and reproduced.
- Add enough instrumentation to tell model limitations from harness problems.

## 中文简介

之前主要从事攻防安全、安全架构和工具工程，最近把更多时间放在 **AI Agent、Agent Harness、评测、自进化系统，以及 AI × 安全工具** 上。这里整理了一些公开项目和仍在探索的方向。

做系统时，我通常倾向于保持框架简单，把开放式推理留给模型，同时补足工具、状态、反馈、验证和恢复能力。相比演示效果，我更关注过程是否 **可观测、可复现、可恢复**。

---

Contact: [twhite.zh@gmail.com](mailto:twhite.zh@gmail.com)
