# Runtime Eval — Grok Bot / Snowflake / v0.3.3

- Runtime: Grok Bot
- Underlying model: Grok (exact model not surfaced)
- Skill version: v0.3.3
- Run date: 2026-09-05
- Topic: Snowflake / Enterprise Data & AI Platform
- Source file: `KR-20260905-SNOW-kerwin-ai-investment-STANDARD.md`

## Score — 18.4 / 20

| Dimension | Score /2 | Notes |
|---|---:|---|
| Decision Question | 2.0 | Correctly asks whether +37% product growth is durable consumption, whether RPO or consumption is the tighter constraint, and whether non-GAAP expansion can become FCF / eventual GAAP profit. |
| Reality | 1.9 | Strong current Q2 FY27 evidence table with correct separation of product revenue, RPO, NRR, GAAP/non-GAAP, SBC, OCF/FCF and guidance. |
| Evidence Integrity | 1.9 | FACT / MANAGEMENT CLAIM / CALCULATION / INSUFFICIENT_EVIDENCE are handled cleanly; AI account metrics are not upgraded into AI revenue. |
| Global Positioning | 1.7 | Correctly places Snowflake in Cloud/Data Platform rather than physical infrastructure; however the Enterprise Agent Control Plane / governance layer and peers such as Salesforce / ServiceNow / Microsoft are underdeveloped. |
| Mechanism | 1.9 | Correct software mechanism: bookings/RPO → consumption → product revenue → cloud cost / gross margin → opex → OCF / FCF. Avoids MW/GPU-hour and owned-capex errors. |
| Ledger | 1.9 | Tracks consumption acceleration, NRR, large customers, RPO, margin mix, GAAP path and AI monetization gap. |
| Economics / Capital | 1.5 | Correctly avoids heavy-asset framing and refuses to invent ROIC/WACC, but does not use current valuation at all and therefore leaves the investment-value question underdeveloped. Reverse expectations are absent. |
| Model Competition | 1.9 | Strong durable-consumption base case versus AI trial pulse, bookings gap, AI margin trap and cloud-native displacement alternatives. |
| Judgment | 1.9 | Separates strong demand/execution from RPO/margin/cash-quality constraints without declaring structural capital deterioration. |
| Falsification / Freshness | 1.8 | Clear product-growth, NRR, RPO, gross-margin and FCF tests; dates/status are generally disciplined. |

## No Critical Failure Triggered

This run passes the software-layer migration test. It does not treat Snowflake's cloud infrastructure costs/commitments as owned capex, and it does not apply physical-infrastructure metrics to an enterprise software business.

## What worked particularly well

1. **Correct capital taxonomy.** Cloud infrastructure cost appears as gross-margin / contribution-margin risk, not as Snowflake-owned data-center capex.
2. **Quarterly FCF discipline.** Q2 5–6% FCF margin is explicitly described as non-annualizable; FY27 23% adjusted FCF guidance remains the real full-year test.
3. **AI adoption vs monetization.** CoCo / CoWork account counts remain management adoption metrics; AI dollar revenue is explicitly INSUFFICIENT_EVIDENCE.
4. **Consumption model is preserved.** RPO is useful but not equated with realized product revenue.
5. **SBC is recognized as an owner-economics issue.** GAAP/non-GAAP divergence and dilution are kept visible.

## Main weaknesses

1. **Valuation is largely omitted.** The report says the current market value was not locked, so Economics / Capital stops before answering what the current price requires. For an investment-value prompt, this is a material gap.
2. **Reverse Expectations is absent.** Current equity value should be inverted into required sustainable revenue growth, product gross margin, FCF margin, SBC/dilution and terminal cash economics.
3. **Agent Control Plane framing is incomplete.** Databricks / BigQuery / Redshift cover data-platform competition, but Salesforce / ServiceNow / Microsoft should enter when asking who controls enterprise agent data, context, model, tool and action layers.
4. **'Ultimate Demand' wording can be sharper.** The real economic spender is enterprise IT/AI budget; hyperscalers are suppliers and sometimes competitors, not final demand owners.
5. **Falsification can include per-share owner economics.** Because SBC is large, future tests should track dilution-adjusted FCF/share in addition to company-level FCF margin.

## Cross-runtime read-through vs WorkBuddy and Grok Chat

- All three agree that product consumption is reaccelerating and AI workloads are a real incremental demand driver.
- WorkBuddy incorrectly pushed cloud commitments + a seasonally low Q2 FCF margin toward a heavy-asset / ROIC-deterioration narrative.
- Grok Bot and Grok Chat both keep Snowflake structurally asset-light and treat cloud spend as COGS / contribution-margin / take-or-pay risk.
- Grok Chat is stronger on valuation and market context; Grok Bot is slightly more conservative on evidence and willing to leave valuation incomplete rather than overstate it.

## v0.4 observation

This case reinforces that the core Skill can switch capital ledgers across business models. The persistent cross-runtime weakness is still Reverse Expectations: market value is discussed inconsistently or omitted, rather than systematically back-solved into required sustainable economics.
