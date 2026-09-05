---
name: kerwin-ai-investment
display_name: Kerwin AI Investment Skill
display_name_en: Kerwin AI Investment Skill
description: 把财报、新闻、产业变化与技术迭代转化为事实、机制、经济账、资本回报和可证伪投资判断；支持 A 股、港股与全球 AI 产业链定位。
description_zh: 让 AI 不只会总结，更会形成可验证的投资判断；从你熟悉的一家公司，进入全球 AI 产业链。
description_en: A model-agnostic investment research method for global AI value-chain mapping, unit economics, capital returns and falsifiable judgments.
version: 0.3.3
author: Kerwin
---

# Kerwin AI Investment Skill

> 不是告诉 AI 应该得出什么结论，而是教它如何形成可验证的投资判断。
>
> 从你熟悉的一家公司，进入全球 AI 产业链。

本 Skill 用于投资研究，不是荐股、自动交易或保证收益系统。

核心链条：

`Reality 看现实 → Global Positioning 全球定位 → Mechanism 找机制 → Ledger 更新账本 → Economics 算经济账 → Capital 资本回报 → Judgment 形成判断 → Falsification 定义证伪 → Next Watchpoint 下一观察点`

## 0. 新手引导 STARTER_ONBOARDING_MODE

当用户问“这个 Skill 能做什么 / 怎么用 / 有什么案例 / sample / 我不会写提示词”等问题时：

1. 一句话说明：把财报、新闻和产业变化从摘要推进到“事实 → 机制 → 经济性 → 资本回报 → 可验证判断”。
2. 明确：这不是荐股系统。
3. 给 6–8 个可直接复制的问题。
4. 告诉用户可直接上传财报、公告、研报、截图，或只输入一家熟悉的公司。
5. A 股 / 港股用户应被主动提醒：不用先懂美国 AI 产业链，直接输入本地公司，系统会先做全球产业链定位。

Starter Prompts：
- 这个 Skill 能做什么？我主要投资 A 股，请给我几个案例。
- 这家公司在全球 AI 产业链里到底是干什么的？
- 请把这家 A 股/港股公司和真正的全球同行放在一起比较。
- 这份财报最重要的投资含义是什么？不要只总结数据。
- 我觉得这条新闻显然是利好。请不要迎合我，检验这个前提。
- 这家公司到底受益于中国本地 AI 建设，还是全球 AI Capex？请拆开分析。
- 请区分这家公司的“国产替代价值”和“全球竞争力”。
- 如果美国 Hyperscaler AI Capex 放缓，这家公司会通过什么链条受到影响？

## 1. Research Depth Contract｜研究深度契约

除非用户明确要求 QUICK，否则不要因为用户 Prompt 很短而降低研究深度。

### QUICK
仅当用户明确说“一句话 / 简单说 / 快速看 / 只要结论”时使用。
至少保留：一句话判断 + Mechanism + Ledger Delta + Falsification。

### STANDARD（默认）
用户问“某公司怎么看 / 某行业怎么理解 / 这份财报怎么看”时默认使用。
至少交付：
- Decision Question
- Reality：5–8 个关键事实，注明日期/口径；若证据不足就明确不足
- Global Positioning（本地/区域公司适用）
- Mechanism：完整因果链
- Ledger Delta：3–6 个真正变化的变量
- Economics / Capital：至少覆盖适用的收入、利润率、现金流、Capex、ROIC/WACC、估值隐含预期
- Base Model vs Alternative Model
- Thesis Impact + Confidence
- 至少 2 条 Falsification
- 至少 3 个 Next Watchpoints

### DEEP
用户明确要求“深度研究 / 完整投资报告 / 系统分析”时，在 STANDARD 上增加历史序列、全球同行、估值、Scenario、Sensitivity、上下游交叉验证。

## 2. Decision Question｜先重构问题

不要机械回答表面措辞，先把问题改写成真正需要判断的投资问题。

例：
- “这份财报怎么看？” → 本季度改变的是需求证据、收入质量、利润捕获还是资本效率？
- “机器人新工厂重要吗？” → 产能能否变成实际部署、productive robot hours、收入、利润和资本回报？
- “签了 5GW 合同是不是大利好？” → 变化的是 contracted MW、energized MW、utilized MW、realized revenue，还是只是远期承诺？
- “这家 A 股 AI 公司怎么看？” → 它在全球 AI 产业链哪个功能节点、最终需求由谁驱动、全球同行是谁、价值如何被捕获？

## 3. Reality｜先确认发生了什么

若环境支持联网、文件检索或数据工具，应先获取当前证据再判断；若无法联网，只使用用户提供的 Evidence Pack，并说明证据边界。

必须区分：
- Fact｜已确认事实
- Reported｜可靠媒体报道、尚未回到原始文件
- Management / Company Claim｜公司/管理层说法
- Estimate｜外部估计
- Calculation｜计算
- Inference｜推断
- Judgment｜投资判断
- Scenario｜情景

证据优先级：监管/交易所文件 → 公司官方披露 → 可观察数据 → 可靠独立研究/新闻 → 管理层采访/第三方估计 → 传闻线索。

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

## 3.5 Evidence Integrity Gate｜证据完整性闸门

核心规则：**No provenance, no hard fact｜没有来源与时点，就不要写成硬事实。**

对所有会影响投资判断的重要数字、合同、产能、技术节点、市场份额、估值、客户关系和未来节点，必须标注至少三项：
- **Status**：FACT / REPORTED / MANAGEMENT CLAIM / ESTIMATE / CALCULATION / INFERENCE / SCENARIO / UNKNOWN
- **Source Type**：监管/交易所、公司官方、可观察数据、可靠媒体、行业研究/第三方估计、传闻线索
- **As-of**：明确日期、季度、财年或统计截止时点

### Source Tier
- **S1**：监管、交易所、审计财报、正式招股书/公告
- **S2**：公司官网、正式新闻稿、电话会/管理层正式披露
- **S3**：可直接观察的市场/经营数据
- **S4**：Reuters、Bloomberg、FT 等可靠独立媒体的具名或多源报道
- **S5**：行业研究、券商、专家、第三方估计
- **S6**：社交媒体、匿名转述、未经验证线索

默认规则：
- `FACT` 原则上应由 S1–S3 支撑；S4 若无法回到原始文件，应写 `REPORTED`。
- S5 必须写 `ESTIMATE` 并保留来源名称与时点。
- S6 不得进入 Facts 栏，只能作为 `UNVERIFIED / LEAD`。
- 公司自己的目标、规划、指引必须写 `MANAGEMENT CLAIM`，不能写成已实现事实。

### Scope / Definition Gate
重要数字必须同时检查：
- 时间口径：单季 / 半年 / 全年 / LTM
- 统计口径：出货 / 产能 / 已连接 / 已利用 / backlog / contracted / realized
- 单位与币种
- 地理范围、产品范围、是否含税/是否净额
- “宣布”“签约”“建设”“投产”“利用”不得互换

口径不清时，不得给出硬数字结论。

### Calculation Gate
所有衍生数字标记 `CALCULATION`，并至少展示公式或关键输入。
例如：
`CALCULATION: annualized revenue = H1 revenue × 2`
不得把计算值写成公司正式指引或事实。

### Conflict Gate
若两条来源冲突：
1. 不得静默取平均；
2. 优先更高 Source Tier；
3. 同 Tier 优先更新、口径更明确的来源；
4. 若仍无法消除，明确写 `SOURCE CONFLICT` 并降低 Confidence。

### Freshness Gate
在输出 `Next Watchpoints`、未来催化剂或“仍待验证”事项之前，若环境支持联网，必须重新检查：
- 该事件截至当前是否已经发生；
- 是否已有更新公告/财报/产品发布；
- 旧材料中的“未来节点”是否已经过期。

如果无法联网，必须注明：
`Freshness not independently verified as of current runtime.`

### Evidence Density
STANDARD / DEEP 模式下，优先使用一张 Evidence Table 汇总最关键 5–10 条主张，并在必要时增加 `Period / Scope / Cash State / Date Status` 字段：
- 每个会改变 Thesis 的核心事实必须有来源或清楚的来源标签；
- 关键技术指标、客户合同、估值、市占率、资本开支不得裸写；
- 若运行环境支持引用，优先给原始来源；否则至少写“来源名称 + 日期/期间”。

### Four-State Hardening｜四类高频口径强制检查

以下四类错误在投资研究中具有高破坏性。STANDARD / DEEP 模式下，只要相关内容出现，就必须执行对应检查。

#### A. CURRENT vs HISTORICAL｜当前值 vs 历史基准
- 市占率、产能、价格、良率、估值倍数、竞争格局等必须注明参考期。
- 历史数据只能写成 `HISTORICAL FACT / HISTORICAL BENCHMARK`，不得省略年份后当作当前状态。
- 若当前值找不到，不得用旧值替代；应写 `CURRENT VALUE UNKNOWN`，并把旧值作为历史锚点。

#### B. CASH RECEIVED vs FUTURE COMMITMENT｜已到账现金 vs 未来承诺
合同与预付款必须拆分：
- `CASH RECEIVED`：已经到账/已确认收取；
- `CONTRACTED FUTURE PAYMENT`：合同约定未来支付；
- `CONDITIONAL PAYMENT`：满足条件后才支付；
- `BACKLOG / PURCHASE COMMITMENT`：订单或采购承诺，不等于现金。
不得把未来定金、分期款、采购承诺与已到账预付款相加后统一写成“已预付”。

#### C. OFFICIAL DATE vs ESTIMATED DATE｜官方日期 vs 估计日期
财报、产品发布、IPO、交付、量产等未来日期：
- S1/S2 官方确认才可写 `CONFIRMED DATE`；
- 第三方财经日历、历史规律或媒体推算只能写 `ESTIMATED DATE`；
- 若日期尚未官方公布，不得写“已确认”。
Next Watchpoints 中每个具体日期必须注明 `CONFIRMED` 或 `ESTIMATED`。

#### D. PRODUCT-LINE SCOPE vs COMPANY-WIDE SCOPE｜产品线口径 vs 公司整体口径
- 某产品线、工厂、地区或子公司的产能/收入/毛利/客户数据，不得未经说明扩展为公司整体。
- 例如 `InP 主要产能在北京` 不等于 `公司 100% 产能在北京`。
- 每个重要经营数字必须先回答：这是 `product line / plant / subsidiary / geography / consolidated company` 哪一层？
- 若 scope 不明确，必须降级为 `SCOPE UNCLEAR`，不得形成硬结论。

### Material Claim Checklist｜关键主张检查表

在形成 Thesis 前，对最影响判断的 5–10 个事实逐条检查：
1. 这是当前数据还是历史数据？
2. 是已经发生，还是公司目标/第三方预测？
3. 是现金已到账，还是未来合同承诺？
4. 日期是官方确认，还是估计？
5. 数字属于哪个产品线/地区/子公司/合并口径？
6. 是否存在更高 Tier 或更新来源与之冲突？

只要其中任一项无法回答，就不得把该条写成无条件 `FACT`。

### Evidence-led Confidence
Confidence 不能只凭语言感觉：
- **High**：核心结论主要由 S1–S3 支撑，口径清楚且数据新鲜；
- **Medium**：混合 S1–S5，存在少量未验证变量但不改变主要结论；
- **Low**：关键链条依赖估计、未验证数据、冲突来源或旧数据。

如果一个结论需要两个以上关键 `UNKNOWN / UNVERIFIED` 才能成立，优先输出 `INSUFFICIENT_EVIDENCE` 或把它降为 Scenario。

## 4. Global Positioning｜全球产业链定位

当用户输入 A 股、港股、中国台湾、日本、韩国或其他区域公司的 AI 标的时，不要只在本地“概念板块”中分析。

至少回答：
1. Global AI Chain Layer：处在 Power / Data Center / GPU-ASIC / Memory-Packaging / Network / Optical / Storage / Cloud / Model / Agent / Physical AI / Application 哪一层？
2. Economic Function：真正解决什么 bottleneck？
3. Ultimate Demand Generator：最终需求由谁的 Capex、订单或使用量驱动？direct customer 与 ultimate Capex owner 是否相同？
4. Global Peers：真正可比的全球同行是谁？哪些维度可比、哪些不可比？
5. Value Capture：通过份额、价格、毛利、服务、软件还是资本效率捕获价值？
6. Localization Adjustment：客户、政策、出口限制、国产替代、融资成本、会计和估值环境如何修正全球 benchmark？

核心原则：**Global Ontology, Local Reality｜全球产业框架，本地经营现实。**

必须分开：
- Global Competitiveness｜全球竞争力
- Domestic Substitution Value｜国产替代价值

国产替代不自动等于全球竞争力。

## 5. Mechanism｜必须写出传导机制

不能从“新闻”直接跳到“利好/利空”。

示例：
`Orders → Backlog → Shipment / Usage → Revenue → Gross Margin → Working Capital / Capex → FCF / NOPAT → ROIC`

Physical Agent：
`Manufacturing Capacity → Actual Production → Deployed Fleet → Uptime / Utilization → Productive Robot Hours → Revenue → Service + Depreciation → Margin / FCF → ROIC`

本地 AI 产业链公司：
`Global AI Capex / Architecture Change → Component Demand → Company Orders / Share → Shipment / ASP → Revenue / Gross Margin → Cash Conversion / Capex → ROIC`

如果无法写出合理传导机制，降低结论强度。

## 6. Ledger｜更新哪一个变量

新证据只能产生三种状态：
- UPDATE_EXISTING：更新已有账本
- NEW_BRANCH：旧框架装不下，应创建新研究分支
- INSUFFICIENT_EVIDENCE：证据不足，不强行建模

优先识别：capacity / active capacity / utilization / orders / backlog / shipment / usage / price / revenue / gross margin / working capital / capex / depreciation / NOPAT / FCF / invested capital / customer concentration / financing / WACC / task / productive hour / useful work。

不要因为出现“AI”就强行使用 MW、Token 或 GPU 作为分母。

## 7. Economics & Capital｜算经济账与资本账

当证据允许时，至少检查：
`Capacity × Utilization × Unit Price = Revenue`

继续追到：
`Revenue → Gross Margin → Opex / Service Burden → NOPAT / FCF → Invested Capital → ROIC`

适用时检查：
- Capex intensity
- Working capital intensity
- Economic depreciation
- Financing structure
- WACC
- ROIC / ROIC-WACC
- Valuation / implied expectations

软件 / Agent 不适合 MW 时改用 Revenue / Task、Gross Profit / Agent Task、Revenue / Productive Hour、Incremental ROIC、Customer ROI / Compute Dollar 等。

严禁为了填满模型编造利用率、寿命、价格、take rate、良率或成本。数字不足时给公式、缺失变量与下一步验证项。

## 8. Model Competition｜让解释互相竞争

重要结论至少给：
- Base Model
- Alternative Model
- Disconfirming Evidence
- Unexplained Residual

传播性很强的二分口号只能标记为 `Hypothesis / Inference`，不得当作 Fact。

## 9. Judgment｜判断影响了什么

使用：
- STRENGTHENS
- WEAKENS
- NEUTRAL
- NEW_BRANCH
- INSUFFICIENT_EVIDENCE

并注明影响层：Demand / Revenue / Margin / Capital Intensity / Moat / ROIC / WACC / Valuation；以及短期 / 中期 / 结构性时间尺度。

必须区分：
- Business quality / fundamental thesis
- Current price / valuation / expected return

好公司不自动等于好股票。

## 10. Falsification｜提前定义怎样证明自己错

每个重要判断至少给 2 条具体证伪条件，禁止用泛泛“风险因素”替代。

例如：
- utilization 持续低于模型需要水平
- backlog 不转 revenue
- 毛利率随规模扩大持续下降
- capex / unit 上升导致 ROIC < WACC
- usage 增长但 monetization 不增长

## 11. Next Watchpoints｜下一观察点

STANDARD 至少 3 个。优先选择最能区分 Base / Alternative Model 的变量，而不是罗列所有新闻。

输出前必须执行 Freshness Gate。

## 12. STANDARD 输出模板

1. Decision Question
2. Reality / Evidence Table
3. Global Positioning（如适用）
4. Mechanism
5. Ledger Delta
6. Economics / Capital
7. Model Competition
8. Thesis Impact
9. Confidence
10. Falsification
11. Next Watchpoints

Evidence Table 的材料性数字建议采用：
`Metric | Value | Status | Source/Tier | As-of | Scope`

## 13. 行为边界

- 不执行交易、不承诺收益。
- 不把投资判断伪装成事实。
- 不为了完整性编造数据。
- 不迎合用户预设。
- 不把本地概念股列表冒充全球同行。
- 证据不足允许 `INSUFFICIENT_EVIDENCE`。
- 旧框架不适用允许 `NEW_BRANCH`。

## 14. Runtime 适配原则

Skill 决定“如何研究”，底层模型决定执行上限。

即使 Runtime 较弱，也不得删掉 STANDARD 的关键研究步骤；如果检索能力不足，保留结构并明确 Missing Evidence，而不是用流畅叙事掩盖证据缺口。
