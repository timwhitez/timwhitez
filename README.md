<div align="center">

# Tim White

### AI Agent Systems · Security Engineering · Applied Research

**Model-led agents, verifier-grounded evaluation, and AI-native security tooling.**

I build systems around the model—tools, state, context, feedback, verification, and recovery—without replacing open-ended reasoning with brittle workflow logic.

[Research direction](#research-direction) · [Selected projects](#selected-projects) · [Security engineering](#security-engineering) · [Engineering principles](#engineering-principles) · [中文简介](#中文简介) · [Email](mailto:twhite.zh@gmail.com)

</div>

---

## Research direction

My work connects two threads: a background in offensive security and a current focus on autonomous systems that can operate against real environments and produce evidence you can trust.

| Track | What I care about |
| --- | --- |
| **Agent runtimes & harnesses** | Preserve model autonomy while improving tools, durable state, context management, live steering, and recovery. |
| **Evaluation & self-improvement** | Turn verifier evidence and reproducible trajectories into bounded improvements without optimizing for self-report, demos, or benchmark-specific workflow logic. |
| **AI × security** | Expose reverse-engineering and security environments through safe, bounded, agent-readable interfaces with explicit evidence strength. |

## Selected projects

| Project | Focus | What makes it different |
| --- | --- | --- |
| **[AutoRE-CLI](https://github.com/timwhitez/AutoRE-CLI)** | AI × reverse engineering | Bounded static analysis for humans and agents, with traceable JSON/CFG/IL output, explicit evidence states, agent-sized context, and no execution of target bytes. |
| **[Aegis Agent](https://github.com/timwhitez/aegis-agent)** | Local agent runtime · Go | The model remains the agent. The harness supplies a Web console, tools, durable session state, compaction, live steering, provider adapters, and explicit safety boundaries. |
| **[HarnessEvolver](https://github.com/timwhitez/harness-evolver)** | Coding-agent evaluation · Rust/Python | Harbor/verifier output is ground truth; verified failures become small, reviewable harness changes with regression gates and auditable evidence. |
| **[dsh-self-evolving](https://github.com/timwhitez/dsh-self-evolving)** | Self-evolution controller · TypeScript | Crash-resumable candidate generation, isolated admission and evaluation, durable lineage, budget enforcement, and explicit trust boundaries. |

**Companion project:** [ida-pro-skill](https://github.com/timwhitez/ida-pro-skill) provides a skill-first bridge that lets coding agents work against a live IDA database through a local, bounded interface.

## Security engineering

Security is not only my earlier background; it is the systems discipline behind how I think about attack surfaces, trust boundaries, observability, and failure. These projects best represent the depth and reach of my public security work.

| Project | Area | Why it stands out |
| --- | --- | --- |
| **[Doge-Gabh](https://github.com/timwhitez/Doge-Gabh)** | Windows internals · Go | A reusable native-API toolkit combining PE parsing, API hashing, ntdll remapping, syscall discovery and invocation, DLL unhooking, and proxy-call research. |
| **[BinHol](https://github.com/timwhitez/BinHol)** | PE binary engineering · Go | A Windows PE rewriting tool supporting function patching, entry-point hijacking, TLS injection, certificate-table handling, and dynamic patch sizing. |
| **[crawlergo_x_XRAY](https://github.com/timwhitez/crawlergo_x_XRAY)** | Web attack-surface automation · Python | Connects dynamic crawling with passive vulnerability scanning, turning browser-discovered paths and requests into a repeatable security pipeline. |
| **[Cobalt-Strike-Aggressor-Scripts](https://github.com/timwhitez/Cobalt-Strike-Aggressor-Scripts)** | Operator automation | A modular Aggressor scripting collection that translated red-team workflows into reusable tooling and achieved sustained community adoption. |

`crawlergo_x_XRAY` and `Cobalt-Strike-Aggressor-Scripts` represent open-source reach; `Doge-Gabh` and `BinHol` better represent systems-level and binary-engineering depth.

Public security work is intended for authorized research, engineering, and defensive understanding.

## Engineering principles

- **Model capability first.** Prefer general mechanisms that amplify reasoning over hand-authored workflows that constrain it.
- **Verifier over self-report.** A plausible completion is not an outcome; external evidence decides what happened.
- **Evidence before confidence.** Separate what is validated, inferred, unresolved, and deliberately not claimed.
- **Recoverability is a feature.** Durable state, replay, explicit failure modes, and deterministic checks matter in long-running systems.
- **Measure the harness.** Instrument enough of the environment to distinguish model limitations from harness defects.

## 中文简介

我长期从事攻防安全、安全架构与工具工程，公开项目覆盖 **Windows 原生调用、PE 二进制工程、Web 攻击面自动化与红队工具工程**。目前主要研究和构建 **AI Agent、Agent Harness、自进化系统、评测与验证器，以及 AI × 安全工具**。

核心思路是：不让复杂工作流替代模型推理，而是通过更好的环境、工具、反馈、状态管理和验证放大模型能力，并让长程任务保持 **可观测、可恢复、可审计**。

---

**Contact:** [twhite.zh@gmail.com](mailto:twhite.zh@gmail.com)
