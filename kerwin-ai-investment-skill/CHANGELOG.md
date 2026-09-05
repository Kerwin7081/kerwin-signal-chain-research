# Changelog — Kerwin AI Investment Skill

## v0.3.2 — 2026-09-05

### Added

- `Evidence Integrity Gate`：核心规则 `No provenance, no hard fact`；
- `Evidence Status`：FACT / REPORTED / MANAGEMENT CLAIM / ESTIMATE / CALCULATION / INFERENCE / SCENARIO / UNKNOWN；
- `Source Tier S1–S6`：区分监管文件、公司披露、可观察数据、可靠媒体、第三方估计与未验证线索；
- `Scope / Definition Gate`：检查时间口径、统计口径、单位币种、产品/地区范围；
- `Calculation Gate`：衍生值必须展示公式或关键输入；
- `Conflict Gate`：来源冲突不得静默平均；
- `Freshness Gate`：Next Watchpoints 输出前确认未来节点是否已经发生；
- `Evidence-led Confidence`：Confidence 由证据质量驱动；
- 5 个固定 Runtime Eval：长鑫科技、中际旭创、宇树科技、Snowflake、5GW AI Infrastructure Contract；
- 20 分 Runtime Eval Rubric 与 Critical Failure 规则。

### Changed

- STANDARD 默认输出中的 Reality 改为 Evidence Table；
- 核心技术指标、合同、产能、市占率、估值与资本开支不得裸写；
- S4 媒体报道在未回到原始文件前默认写 `REPORTED`；
- S5 行业/券商/专家数据默认写 `ESTIMATE`；
- 无法联网执行 Freshness Gate 时必须明确 freshness 未独立验证。

## v0.3.1 — 2026-09-05

### Changed

- WorkBuddy Desktop Compatibility Packaging：安装 ZIP 根目录直接包含 `SKILL.md`；
- 提供 standalone 单文件导入方式，减少不同 Runtime 对目录结构的兼容问题。

## v0.3.0 — 2026-09-04

### Added

- `Research Depth Contract`：QUICK / STANDARD / DEEP 三档研究深度；
- `STANDARD` 成为默认研究模式：短 Prompt 不再等于浅回答；
- 跨模型最低质量规则，要求保留 Mechanism / Ledger / Economics / Capital / Model Competition / Falsification；
- 强传播性叙事必须标记为 `Hypothesis / Inference`，并给出 Alternative Model 与证伪条件。

### Changed

- STANDARD 输出要求增加 5–8 个关键事实及日期/口径；
- 本地/区域公司默认增加全球产业链定位与 3–5 个真正可比全球同行；
- 数据不足时保留资本层公式、缺失变量与验证项，而不是直接跳过；
- QUICK 仅在用户明确要求“一句话 / 简单说说 / 快速看一下”等场景触发。

## v0.2.0 — 2026-09-04

首个公开发布候选版本。

### Added

- `STARTER_ONBOARDING_MODE`；
- `Starter Prompts`；
- `Global AI Chain Mapping`；
- `Global Ontology, Local Reality`；
- `Global Peer Mapping Ledger`；
- WorkBuddy ZIP 安装包；
- EnyaClawd 产品页、永久产品页二维码和版本化下载地址。

### Core Method

`Reality → Global Positioning（如适用） → Mechanism → Ledger → Economics → Capital → Judgment → Falsification → Next Watchpoint`

### Boundary

这不是荐股系统、自动交易系统或保证收益产品。Community Edition 发布方法、空白模板和使用引导，不包含 Kerwin 私有组合、实时 Thesis Registry、专有 benchmark、客户资料或内部自动化。

## Versioning

后续版本继续采用语义化版本号：`MAJOR.MINOR.PATCH`。

- `PATCH`：文案、示例、兼容性和小修复；
- `MINOR`：新增研究能力、Ledger、Onboarding 或 Runtime 适配；
- `MAJOR`：核心研究方法或产品契约发生重要变化。
