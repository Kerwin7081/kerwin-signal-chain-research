# Runtime Eval — Grok Chat / Snowflake / v0.3.3

- Runtime: Grok Chat
- Underlying model: Grok (exact model not surfaced)
- Skill version: v0.3.3
- Run date: 2026-09-05
- Topic: Snowflake / Enterprise Data & Agent Platform
- Prompt: Snowflake 怎么看？投资价值如何？（user test context）

## Score — 18.9 / 20

| Dimension | Score /2 | Notes |
|---|---:|---|
| Decision Question | 2.0 | Correctly reframes whether AI adds durable incremental workloads/consumption versus merely changing the interface while gross margin and RPO lag. |
| Reality | 1.9 | Strong current Q2 FY27 evidence table, correct GAAP/non-GAAP separation, RPO/NRR/customer metrics and explicit guidance status. |
| Evidence Integrity | 1.8 | Strong FACT / MANAGEMENT CLAIM / ESTIMATE / CALCULATION discipline; Q2 6% adjusted FCF is explicitly not annualized. Minor issue: forward total-revenue PS estimate appears too low and some WACC/general market-cost language is unsourced inference. |
| Global Positioning | 1.8 | Correct Cloud/Data Platform and AI-on-governed-data positioning; hyperscalers are suppliers and competitors, not ultimate capex owners. Could more explicitly include enterprise Agent Control Plane peers such as Salesforce and ServiceNow. |
| Mechanism | 2.0 | Correct software/agent mechanism: workloads → consumption → product revenue → cloud/model COGS → product gross margin → opex → OCF/FCF → light invested capital. Crucially avoids treating AWS commitment as owned capex. |
| Ledger | 1.9 | Tracks consumption, NRR, large customers, RPO, margin mix, cash seasonality and AI-adoption proxy while keeping AI dollar monetization undisclosed. |
| Economics / Capital | 1.7 | Correctly frames cloud cost rather than heavy-asset capex and uses FCF/SBC/dilution. Still lacks full reverse-expectations / incremental-ROIC backsolve; forward total-revenue PS arithmetic needs correction. |
| Model Competition | 1.9 | Strong durable-AI-consumption base case versus first-wave AI adoption / optimization / Databricks-Fabric displacement alternative. |
| Judgment | 1.9 | Separates product-growth strengthening, cash/RPO uncertainty and valuation neutrality without overcalling structural capital deterioration. |
| Falsification / Freshness | 1.8 | Good Q3/Q4 product-growth, RPO, margin, FCF and AI monetization tests; dates are kept estimated where appropriate. |

## No Critical Failure Triggered

This run passes the software-layer migration test. It does not force MW/GPU-hour or owned-capex logic onto Snowflake, and it correctly treats cloud infrastructure spend as a cost/commitment variable rather than balance-sheet heavy-asset ownership.

## What worked particularly well

1. **Correct capital taxonomy.** AWS/Azure/GCP appear in cloud COGS / infrastructure commitments, not as Snowflake-owned capex.
2. **Single-quarter cash discipline.** Q2 adjusted FCF margin of ~6% is explicitly described as seasonal and not annualized; FY27 adjusted FCF margin guidance of 23% remains the full-year test.
3. **AI adoption vs monetization separation.** CoCo/CoWork account counts remain adoption proxies; AI dollar revenue and take rate are left undisclosed.
4. **Consumption-model logic is preserved.** RPO is treated as useful but imperfect because consumption timing can differ from contracted capacity.
5. **Software-specific mechanism is correct.** `task/query volume × compute/storage consumption → product revenue → cloud COGS → product margin → opex → FCF → incremental ROIC`.

## Main weaknesses

1. **Forward total-revenue PS arithmetic appears understated.** With market cap about $116.9B and FY27 product revenue guidance of $6.07B, adding a modest services component does not obviously reduce forward total-revenue PS to 16–17×; the calculation should be rechecked and explicitly show the denominator.
2. **Reverse Expectations remains incomplete.** The report still mostly asks whether 19× product revenue / ~100× FCF is expensive rather than back-solving the sustainable revenue growth, contribution margin, FCF margin, dilution and terminal cash economics required by the current price.
3. **Agent Control Plane positioning could be broader.** Databricks / Fabric / BigQuery / Redshift cover data-platform competition well, but Salesforce / ServiceNow / Microsoft should enter when evaluating who controls enterprise agent context, governance, tools and actions.
4. **WACC language should be labeled as inference.** Statements that high-growth US software has lower capital cost than A-share theme stocks are directional judgments, not measured company-specific WACC.
5. **$6B AWS wording should stay precise.** Official Snowflake/AWS language is a multi-year infrastructure commitment including Graviton compute and AI spend; it should not be simplified into a customer contract or owned infrastructure asset.

## Cross-runtime read-through vs WorkBuddy

- WorkBuddy and Grok Chat agree that Snowflake's AI/data consumption growth is real and that AI workloads currently dilute product gross margin somewhat.
- The key divergence is capital interpretation: WorkBuddy pushed the $6B AWS commitment and Q2 6% FCF margin toward a heavy-asset / ROIC-deterioration narrative, while Grok Chat correctly keeps Snowflake structurally asset-light and treats the commitment as cloud COGS / take-or-pay / margin risk.
- This strongly suggests the heavy-asset framing is a WorkBuddy runtime behavior, not a core Skill requirement.

## v0.4 observation

Snowflake provides positive evidence that v0.3.3 can switch from Physical Infrastructure / Physical Agent ledgers into Enterprise Software without forcing physical-capital metrics. The recurring cross-case Skill-level gap remains Reverse Expectations: current market value is discussed, but not yet systematically inverted into required sustainable operating and cash-flow outcomes.
