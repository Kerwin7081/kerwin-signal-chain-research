# Evidence Policy — v0.3.3

核心原则：**No provenance, no hard fact｜没有来源与时点，就不要写成硬事实。**

证据优先级：监管/交易所文件 → 公司官方披露 → 可直接观察的数据 → 可靠独立媒体 → 行业研究/券商/专家估计 → 社交媒体或传闻线索。

## Evidence Status
- `FACT`：已确认事实，原则上由 S1–S3 支撑
- `REPORTED`：可靠媒体报道但尚未回到原始文件
- `MANAGEMENT CLAIM`：公司或管理层目标、规划、指引、解释
- `ESTIMATE`：外部研究、专家、券商、行业模型估计
- `CALCULATION`：基于已知输入的衍生计算
- `INFERENCE`：推断
- `JUDGMENT`：投资判断
- `SCENARIO`：情景假设
- `UNKNOWN / UNVERIFIED`：尚未验证

## Source Tier
- S1：监管、交易所、审计财报、正式招股书/公告
- S2：公司官网、正式新闻稿、电话会/管理层正式披露
- S3：可直接观察的市场/经营数据
- S4：可靠独立媒体的具名或多源报道
- S5：行业研究、券商、专家、第三方估计
- S6：社交媒体、匿名转述、未经验证线索

## Required Fields
对会改变投资判断的重要数字、合同、产能、技术节点、市场份额、估值和客户关系，至少记录：
`Status + Source Type/Tier + As-of + Scope/Definition`

## Four-State Hardening

### CURRENT vs HISTORICAL
- 历史市占率、产能、价格、估值倍数、竞争格局必须带参考期；
- 历史值只能标 `HISTORICAL FACT / HISTORICAL BENCHMARK`；
- 找不到当前值时写 `CURRENT VALUE UNKNOWN`，不得用历史值替代。

### CASH RECEIVED vs FUTURE COMMITMENT
- `CASH RECEIVED`：已到账/已确认收取；
- `CONTRACTED FUTURE PAYMENT`：合同约定未来支付；
- `CONDITIONAL PAYMENT`：满足条件后才支付；
- `BACKLOG / PURCHASE COMMITMENT`：订单/采购承诺，不等于现金。
不得把这些项目加总后统一写成“已预付”。

### OFFICIAL DATE vs ESTIMATED DATE
- S1/S2 官方确认的未来日期写 `CONFIRMED DATE`；
- 第三方财经日历、媒体推算、历史规律只能写 `ESTIMATED DATE`；
- 未官方确认不得写“已确认”。

### PRODUCT-LINE SCOPE vs COMPANY-WIDE SCOPE
- product line / plant / subsidiary / geography / consolidated company 必须明确；
- 产品线或工厂数据不得自动泛化到集团整体；
- scope 不清写 `SCOPE UNCLEAR`。

## Hard Rules
- S4 未回到原始文件时写 `REPORTED`。
- S5 必须写 `ESTIMATE`。
- S6 不得进入 Facts 栏。
- 管理层目标写 `MANAGEMENT CLAIM`。
- 衍生数字写 `CALCULATION` 并展示关键输入。
- 来源冲突不得静默平均，仍无法解决写 `SOURCE CONFLICT`。

不要自动等同：
- announced capacity = active capacity
- contracted revenue = realized revenue
- backlog = revenue
- future payment = cash received
- historical share = current share
- estimated calendar date = confirmed date
- product-line capacity = company-wide capacity
- product launch = adoption
- adoption = monetization
- EBITDA = FCF
- revenue growth = ROIC improvement

## Freshness Gate
输出 Next Watchpoints、未来催化剂或“仍待验证”事项前，若可联网，必须重新确认事项是否已经发生或被更新；若无法联网，注明 freshness 未独立验证。

## Material Claim Checklist
形成 Thesis 前，对最关键 5–10 项事实逐条检查：
1. 当前还是历史？
2. 已发生还是目标/预测？
3. 现金已到账还是未来承诺？
4. 日期官方确认还是估计？
5. scope 属于产品线/工厂/地区/子公司还是集团？
6. 是否有更高 Tier 或更新来源冲突？

## Confidence
- High：核心结论主要由 S1–S3 支撑，口径清楚且新鲜
- Medium：混合 S1–S5，少量未知不改变主结论
- Low：关键链依赖估计、冲突、旧数据或未验证变量
