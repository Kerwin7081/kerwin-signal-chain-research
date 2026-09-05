# Kerwin AI Investment Skill — Community Edition v0.3.3

> 不是告诉 AI 应该得出什么结论，而是教它如何形成可验证的投资判断。
>
> 从你熟悉的一家公司，进入全球 AI 产业链。

这是 Kerwin AI Investment Skill 的公开 Community Edition。它把财报、新闻、产业变化与技术迭代转化为一套可重复的研究程序：

`Reality 看现实 → Global Positioning 全球定位 → Mechanism 找机制 → Ledger 更新账本 → Economics 算经济账 → Capital 资本回报 → Judgment 形成判断 → Falsification 定义证伪 → Next Watchpoint 下一观察点`

## v0.3.3：Evidence Integrity Hardening

本版本基于北京通美 / AXT 的真实 Runtime 测试，对 v0.3.2 Evidence Gate 做四项强制加固：

- **CURRENT vs HISTORICAL**：历史市占率、产能、价格和估值不得省略年份后冒充当前值；
- **CASH RECEIVED vs FUTURE COMMITMENT**：已到账预付款、未来分期款、条件付款、backlog / purchase commitment 必须分开；
- **OFFICIAL DATE vs ESTIMATED DATE**：财报、发布、IPO 等未来日期只有 S1/S2 官方确认才可写 `CONFIRMED`；
- **PRODUCT-LINE SCOPE vs COMPANY-WIDE SCOPE**：产品线、工厂、地区和子公司数据不得未经说明扩展为公司整体。

同时新增 `Material Claim Checklist`：在形成 Thesis 前，对最关键 5–10 个事实逐条检查时点、状态、现金状态、日期状态、scope 与来源冲突。

## v0.3.2：Evidence Integrity

- **No provenance, no hard fact**：没有来源与时点，不写成硬事实；
- 关键数据统一标记 `FACT / REPORTED / MANAGEMENT CLAIM / ESTIMATE / CALCULATION / INFERENCE / SCENARIO / UNKNOWN`；
- 引入 S1–S6 Source Tier；
- 增加 Scope / Definition、Calculation、Conflict 与 Freshness Gate；
- Confidence 必须由证据质量驱动，而不是由语言强度驱动。

## Research Depth

v0.3.0 起新增 QUICK / STANDARD / DEEP 三档研究深度，**STANDARD 为默认**。用户哪怕只问一句“这家公司怎么看？”，也不能因为 Prompt 很短而退化为新闻摘要。

## Runtime Evals

固定五个 Runtime Eval：
1. 长鑫科技
2. 中际旭创
3. 宇树科技
4. Snowflake
5. 5GW AI Infrastructure Contract

每例 20 分。v0.4.0 才进入 Cross-Model Consistency。

## 产品页与下载

https://enyaclawd.com/kerwin-ai-investment-skill/

当前版本：`v0.3.3`

## 边界

这不是荐股系统、自动交易系统或保证收益产品。公开版包含方法、空白账本、Evals 和使用引导，不包含 Kerwin 的私有组合、实时 Thesis Registry、专有 benchmark、客户数据或内部自动化。
