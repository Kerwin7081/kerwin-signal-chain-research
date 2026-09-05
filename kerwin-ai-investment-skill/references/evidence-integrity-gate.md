# Evidence Integrity Gate — v0.3.2

核心原则：**No provenance, no hard fact｜没有来源与时点，就不要写成硬事实。**

## Mandatory Evidence Fields

对会改变投资判断的重要数据，至少记录：

| Field | Allowed values |
|---|---|
| Status | FACT / REPORTED / MANAGEMENT CLAIM / ESTIMATE / CALCULATION / INFERENCE / SCENARIO / UNKNOWN |
| Source Tier | S1 / S2 / S3 / S4 / S5 / S6 |
| As-of | date / quarter / fiscal period |
| Scope | unit / geography / product / accounting definition |

## Source Tier

- S1：监管、交易所、审计财报、正式招股书/公告
- S2：公司官网、新闻稿、电话会/管理层正式披露
- S3：可直接观察的市场/经营数据
- S4：可靠独立媒体的具名或多源报道
- S5：券商、行业研究、专家、第三方估计
- S6：社交媒体、匿名转述、未经验证线索

## Hard Rules

1. FACT 原则上必须由 S1–S3 支撑；S4 未回到原始文件时写 REPORTED。
2. S5 必须写 ESTIMATE，不得进入 Facts 栏。
3. S6 不得进入 Facts，只能作为 UNVERIFIED / LEAD。
4. 管理层目标、产能规划、未来指引写 MANAGEMENT CLAIM，不写成已实现。
5. 衍生值写 CALCULATION，并展示关键公式或输入。
6. 来源冲突时不得静默平均，必须标记 SOURCE CONFLICT。
7. STANDARD / DEEP 的核心数字不得裸写。

## Freshness Gate

在输出 Next Watchpoints 前，若可联网，必须再次检查未来节点是否已经发生或被更新。
无法联网时注明：`Freshness not independently verified as of current runtime.`

## Confidence

- High：主要由 S1–S3 支撑，口径明确且新鲜
- Medium：混合 S1–S5，少量未知不改变主结论
- Low：关键链依赖估计、旧数据或冲突来源
