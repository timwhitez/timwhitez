# A guide to a few public projects

[Back to profile](README.md) · [中文导览](#中文导览)

I work on security tooling and agent infrastructure. This page offers a few starting points based on what you are trying to do, rather than a list of everything I have built. The project documentation remains the source of truth for installation, scope, and limitations.

## Inspect a binary without running it

**[AutoRE-CLI](https://github.com/timwhitez/AutoRE-CLI)** is a static-analysis CLI and companion Agent Skill. It exposes bounded JSON and binary-analysis evidence for human analysts and agents. Findings distinguish validated evidence, inference, unresolved questions, and claims that were not made.

Start with the [installation instructions](https://github.com/timwhitez/AutoRE-CLI#install), then the [controlled demo](https://github.com/timwhitez/AutoRE-CLI/tree/main/examples/controlled). The demo uses a benign, independently authored C fixture compiled into an object file; do not execute the generated object or replace it with a live unknown sample for a first trial. Inspect the report and verification output, including warnings and missing evidence, rather than treating a generated explanation as a verified result.

**Boundary:** this is a public binary distribution with MIT-licensed public scripts, Skill, examples, and documentation. The engine implementation is not published. It is not a debugger, emulator, or guarantee of accurate source recovery. The static-only design is not a claim that parsing untrusted files is risk-free; follow the project's [security guidance](https://github.com/timwhitez/AutoRE-CLI/blob/main/SECURITY.md).

Useful feedback: installation failures, unclear output fields, and a specific static-analysis workflow that the documented interface does not explain. Use the [issue tracker](https://github.com/timwhitez/AutoRE-CLI/issues) for reproducible bugs and documentation corrections. Do not attach malware, secrets, proprietary binaries, or private analysis output.

## Review security boundaries in an AI/GPU cloud

**[neocloud-sec](https://github.com/timwhitez/neocloud-sec)** collects a vendor-neutral security baseline, reference architecture, practice guides, and local documentation/evidence-metadata validators. English and Chinese reading paths are available in its README.

Start with the [scope and limitations](https://github.com/timwhitez/neocloud-sec/blob/main/docs/en/SCOPE_AND_LIMITATIONS.md), then choose the baseline, architecture, or practice guide from the [project index](https://github.com/timwhitez/neocloud-sec#start-here). A useful review exercise is to take one control and ask: who owns it, what evidence would verify it, and what remains unknown? Keep actual assets and evidence in your own private system.

**Boundary:** the baseline is a draft. Documentation and metadata validation do not deploy controls, test tenant isolation, certify a provider, or establish compliance. No open-source license is currently granted; public visibility should not be read as a blanket reuse permission. The project is independent and does not claim endorsement by any provider or rating organization.

Useful feedback: an ambiguous control, a missing service boundary, an outdated primary reference, or a mismatch between the English and Chinese text. Follow the [contribution process](https://github.com/timwhitez/neocloud-sec/blob/main/CONTRIBUTING.md) and the [private security-reporting guidance](https://github.com/timwhitez/neocloud-sec/blob/main/SECURITY.md).

## Study how an agent harness handles failure evidence

**[HarnessEvolver](https://github.com/timwhitez/harness-evolver)** is research software for studying a Rust Worker, Python orchestration, verifier feedback, and bounded harness changes.

Read [status and scope](https://github.com/timwhitez/harness-evolver#status-and-scope) and the [architecture](https://github.com/timwhitez/harness-evolver/blob/main/docs/architecture.md) first. Its quick start separates deterministic checks and dry runs from real benchmark execution. Real trials need separately obtained tasks, compatible tooling, and provider configuration.

**Boundary:** the repository does not claim a published TerminalBench score or a state-of-the-art result. A passing unit test or a model's completion message is not evidence of benchmark performance. Local commands and examples on this page are reading pointers, not new benchmark results.

Useful feedback: reproducible setup problems, unclear evidence handling, or a focused regression case. Follow [CONTRIBUTING.md](https://github.com/timwhitez/harness-evolver/blob/main/CONTRIBUTING.md); keep credentials, private endpoints, and raw campaign artifacts out of public reports.

## 中文导览

这里按使用目的整理了三个入口，具体安装方法和能力边界以各项目文档为准。

| 你正在做的事情 | 从哪里开始 | 需要注意的边界 |
| --- | --- | --- |
| 给人或 Agent 提供可追溯的二进制静态分析结果 | [AutoRE-CLI 中文说明](https://github.com/timwhitez/AutoRE-CLI/blob/main/README_zh.md)，然后看 [受控示例](https://github.com/timwhitez/AutoRE-CLI/tree/main/examples/controlled) | 不执行目标；公开的是二进制发行包和配套公开内容，不是完整引擎源码；不是“完美还原源代码”的承诺。 |
| 梳理 AI/GPU 云的安全责任、控制和验证证据 | [neocloud-sec 中文入口](https://github.com/timwhitez/neocloud-sec/blob/main/README.zh-CN.md) | 是文档基线草案，不是已部署的控制平台、认证或厂商背书；当前未授予开源许可。 |
| 研究 Agent 的执行、失败证据与受约束的 Harness 更新 | [HarnessEvolver](https://github.com/timwhitez/harness-evolver#status-and-scope) | 是研究软件，没有已发布的榜单成绩或领先性结论；测试通过不等于模型能力提升。 |

安装卡在哪一步、哪段文档不清楚、哪项假设不符合实际，比泛泛评价更有帮助。欢迎在对应项目中提交可复现的问题或具体文档建议；请勿上传敏感样本、凭据、私有数据或未经处理的运行记录。安全问题请使用各项目的私下报告渠道。

## Follow the work

For related public projects, you can [follow my GitHub profile](https://github.com/timwhitez). For one project's changes, use its release notes, changelog, and issue tracker where available. Reports of limitations and things that did not work are welcome too.
