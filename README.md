<div align="center">

# Tim White

### AI Agent Systems · Security Engineering · Applied Research

**Model-led agents, verifier-grounded evaluation, and AI-native security tooling.**

I build systems around the model—tools, state, context, feedback, verification, and recovery—without replacing open-ended reasoning with brittle workflow logic.

[Selected projects](#selected-projects) · [Research direction](#research-direction) · [Engineering principles](#engineering-principles) · [中文简介](#中文简介) · [Email](mailto:twhite.zh@gmail.com)

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
| **[Aegis Agent](https://github.com/timwhitez/aegis-agent)** | Local agent runtime · Go | The model remains the agent. The harness supplies a Web console, tools, durable session state, compaction, live steering, provider adapters, and explicit safety boundaries. |
| **[AutoRE-CLI](https://github.com/timwhitez/AutoRE-CLI)** | AI × reverse engineering | Bounded static analysis for humans and agents, with traceable JSON/CFG/IL output, explicit evidence states, agent-sized context, and no execution of target bytes. |
| **[HarnessEvolver](https://github.com/timwhitez/harness-evolver)** | Coding-agent evaluation · Rust/Python | Harbor/verifier output is ground truth; verified failures become small, reviewable harness changes with regression gates and auditable evidence. |
| **[dsh-self-evolving](https://github.com/timwhitez/dsh-self-evolving)** | Self-evolution controller · TypeScript | Crash-resumable candidate generation, isolated admission and evaluation, durable lineage, budget enforcement, and explicit trust boundaries. |

**Related tool:** [ida-pro-skill](https://github.com/timwhitez/ida-pro-skill) provides a skill-first bridge that lets coding agents work against a live IDA database through a local, bounded interface.

## Engineering principles

- **Model capability first.** Prefer general mechanisms that amplify reasoning over hand-authored workflows that constrain it.
- **Verifier over self-report.** A plausible completion is not an outcome; external evidence decides what happened.
- **Evidence before confidence.** Separate what is validated, inferred, unresolved, and deliberately not claimed.
- **Recoverability is a feature.** Durable state, replay, explicit failure modes, and deterministic checks matter in long-running systems.
- **Measure the harness.** Instrument enough of the environment to distinguish model limitations from harness defects.

## Security research foundation

Earlier public work focused on offensive security, Windows internals, red-team tooling, and attack-surface automation. That experience now informs how I design agent tools, evaluators, isolation boundaries, and failure models.

- **[Cobalt-Strike-Aggressor-Scripts](https://github.com/timwhitez/Cobalt-Strike-Aggressor-Scripts)** — operator automation and offensive-security research.
- **[Spoofing-Gate](https://github.com/timwhitez/Spoofing-Gate)** — Windows syscall and Gate-technique research around ntdll-mediated execution.
- **[crawlergo_x_XRAY](https://github.com/timwhitez/crawlergo_x_XRAY)** — web discovery and security-scanning automation.

Public security work is intended for authorized research, engineering, and defensive understanding.

## 中文简介

我长期从事攻防安全、安全架构与工具工程，目前主要研究和构建 **AI Agent、Agent Harness、自进化系统、评测与验证器，以及 AI × 安全工具**。

核心思路是：不让复杂工作流替代模型推理，而是通过更好的环境、工具、反馈、状态管理和验证放大模型能力，并让长程任务保持 **可观测、可恢复、可审计**。

---

**Contact:** [twhite.zh@gmail.com](mailto:twhite.zh@gmail.com)
