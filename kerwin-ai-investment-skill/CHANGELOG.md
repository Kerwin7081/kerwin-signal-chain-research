# Changelog — Kerwin AI Investment Skill

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

- `STARTER_ONBOARDING_MODE`：当用户问“能做什么 / 怎么用 / 有什么 sample”时自动进入新手引导；
- `Starter Prompts`：提供可直接复制的财报、新闻、产业链、公司对比与 A 股 / 港股场景提示词；
- `Global AI Chain Mapping`：把本地 AI 公司放回全球产业链定位；
- `Global Ontology, Local Reality`：全球产业框架、本地经营现实；
- `Global Peer Mapping Ledger`：比较本地公司与全球同行的功能、技术、客户、利润率、资本强度和 ROIC；
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
