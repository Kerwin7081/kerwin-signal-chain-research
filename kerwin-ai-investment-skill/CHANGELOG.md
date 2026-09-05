# Changelog — Kerwin AI Investment Skill

## v0.3.3 — 2026-09-05

### Added
- `CURRENT vs HISTORICAL Gate`：历史数据不得省略年份后写成当前值；当前值缺失时必须明确 `CURRENT VALUE UNKNOWN`。
- `CASH RECEIVED vs FUTURE COMMITMENT Gate`：拆分已到账现金、未来合同付款、条件付款、backlog / purchase commitment。
- `OFFICIAL DATE vs ESTIMATED DATE Gate`：未来财报/发布/IPO/交付日期只有 S1/S2 官方确认才可标 `CONFIRMED`。
- `PRODUCT-LINE SCOPE vs COMPANY-WIDE SCOPE Gate`：产品线/工厂/地区/子公司指标不得未经说明扩展为公司整体。
- `Material Claim Checklist`：Thesis 前对关键 5–10 项事实执行时点、状态、现金、日期、scope 与来源冲突检查。

### Changed
- STANDARD / DEEP 的 Evidence Table 允许增加 `Period / Scope / Cash State / Date Status` 字段。
- `REPORTED` 正式进入 Reality 基础分类，避免可靠媒体报道自动被写成 FACT。
- Evidence Integrity 的 Critical Failure 扩展到：历史数据冒充当前值、未来付款冒充已到账现金、估计日期冒充官方日期、产品线口径冒充公司整体。

## v0.3.2 — 2026-09-05

### Added
- `Evidence Integrity Gate`：核心规则 `No provenance, no hard fact`；
- `Evidence Status`、`Source Tier S1–S6`；
- `Scope / Definition Gate`、`Calculation Gate`、`Conflict Gate`、`Freshness Gate`；
- `Evidence-led Confidence`；
- 5 个固定 Runtime Eval 与 20 分 Rubric。

## v0.3.1 — 2026-09-05
- WorkBuddy Desktop Compatibility Packaging：ZIP 根目录直接包含 `SKILL.md`。

## v0.3.0 — 2026-09-04
- `Research Depth Contract`：QUICK / STANDARD / DEEP；STANDARD 默认。

## v0.2.0 — 2026-09-04
- 首个公开发布候选版本：Onboarding、Starter Prompts、Global AI Chain Mapping、WorkBuddy 包与 EnyaClawd 产品页。

## Versioning
- `PATCH`：证据规则、兼容性、示例和小修复；
- `MINOR`：新增研究能力、Ledger 或 Runtime 适配；
- `MAJOR`：核心研究方法或产品契约的重要变化。
