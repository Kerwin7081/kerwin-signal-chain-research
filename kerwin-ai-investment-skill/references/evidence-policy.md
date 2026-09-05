# Evidence Policy — v0.3.2

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

重要数字必须检查时间口径、统计口径、单位币种、产品/地区范围。口径不清时不得写硬结论。

## Hard Rules

- S4 未回到原始文件时写 `REPORTED`，不自动升级为 FACT。
- S5 必须写 `ESTIMATE` 并保留来源名称与日期。
- S6 不得进入 Facts 栏，只能作为 `UNVERIFIED / LEAD`。
- 管理层目标、规划、未来产能写 `MANAGEMENT CLAIM`，不能写成已实现。
- 衍生数字写 `CALCULATION`，至少展示关键公式或输入。
- 来源冲突时不得静默平均；优先更高 Tier、更新且口径更明确的来源；仍无法解决则标记 `SOURCE CONFLICT`。

不要自动等同：
- announced capacity = active capacity
- contracted revenue = realized revenue
- backlog = revenue
- product launch = adoption
- adoption = monetization
- customer savings = vendor revenue
- gross bookings = platform revenue
- EBITDA = FCF
- revenue growth = ROIC improvement
- management target = achieved result

## Freshness Gate

在输出 Next Watchpoints、未来催化剂或“仍待验证”事项之前，若运行环境支持联网，必须重新确认该事项截至当前是否已经发生或被更新。

若无法联网，注明：`Freshness not independently verified as of current runtime.`

## Confidence

- High：核心结论主要由 S1–S3 支撑，口径清楚且新鲜
- Medium：混合 S1–S5，存在少量未知但不改变主结论
- Low：关键链依赖估计、冲突来源、旧数据或未验证变量

若一个结论需要两个以上关键 `UNKNOWN / UNVERIFIED` 才能成立，优先输出 `INSUFFICIENT_EVIDENCE` 或把它降为 Scenario。

若用户的问题带有强预设，例如“这显然证明……对吧？”，必须检验前提而不是迎合。
