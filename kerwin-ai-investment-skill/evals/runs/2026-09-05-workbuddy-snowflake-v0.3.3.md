# Runtime Eval — WorkBuddy / Snowflake / v0.3.3

- Runtime: WorkBuddy
- Underlying model: not surfaced
- Skill version: v0.3.3
- Run date: 2026-09-05
- Topic: Snowflake / Enterprise AI Data Platform / earnings analysis
- Prompt: Snowflake 怎么看？投资价值如何？（user test context）

## Score — 15.6 / 20

| Dimension | Score /2 | Notes |
|---|---:|---|
| Decision Question | 2.0 | Strong reframing around whether AI growth is high-quality consumption or lower-margin cloud/AI pass-through, and what current valuation requires. |
| Reality | 1.6 | Core Q2 FY27 facts are mostly current and correct, but the acceleration sequence is misstated and some RPO/market/peer facts are not fully source-reconciled. |
| Evidence Integrity | 1.3 | FACT / MANAGEMENT CLAIM / REPORTED labels are present, but later inference outruns evidence: Q2 adjusted FCF margin is used as if it were structural, and the $6B AWS minimum-spend commitment is treated as evidence of ‘heavy-assetization’. |
| Global Positioning | 1.6 | Correctly places Snowflake in enterprise data / cloud software rather than physical compute, but the Enterprise Agent Control Plane / governance role is underdeveloped and peer taxonomy omits important enterprise-software comparables such as Salesforce and ServiceNow. |
| Mechanism | 1.6 | Good `enterprise AI usage → consumption → product revenue → gross margin → opex → FCF` chain, but cloud procurement commitments are incorrectly pushed into a capital-intensity narrative instead of gross-margin / take-or-pay risk. |
| Ledger | 1.6 | Tracks revenue growth, AI monetization, gross margin, RPO and cash generation; however FCF interpretation and RPO trend treatment need tighter source/seasonality discipline. |
| Economics / Capital | 1.0 | Basic valuation arithmetic is useful, but the capital analysis is materially distorted by using a single-quarter 6% adjusted FCF margin while full-year guidance remains 23%, and by describing AWS cloud spend as ‘重资产化’. Reverse-expectations analysis remains incomplete. |
| Model Competition | 1.8 | Strong AI-flywheel vs lower-margin consumption / contract-burn alternative model with clear competitive risks. |
| Judgment | 1.4 | Demand/AI monetization strengthening is well supported, but ‘capital efficiency weakens’ and ‘growth is bought with real money’ are too strong given FY27 operating-margin expansion and 23% adjusted FCF guidance. |
| Falsification / Freshness | 1.7 | Q3 date is correctly estimated; product-revenue, gross-margin, NRR and RPO watchpoints are useful, though some thresholds ignore consumption-model seasonality and annual cash-flow guidance. |

## No Critical Failure Triggered

The run does not force MW / GPU-hour metrics onto a software company and correctly recognizes Snowflake as a consumption-based enterprise data/AI platform. However, it makes a material conceptual error in the capital layer by conflating cloud procurement commitments and a seasonally low single-quarter FCF margin with ‘heavy-assetization’.

## Material issues

1. **Product-revenue acceleration sequence is wrong.** Official filings show Q3 FY26 +29%, Q4 FY26 +30%, Q1 FY27 +34%, Q2 FY27 +37%, which is the actual three-consecutive-quarter acceleration. The report’s `31.5%→27%→34%→37%` sequence is not the clean official series.
2. **Q2 adjusted FCF margin 6% is real, but not a structural FY27 margin.** Snowflake simultaneously reiterated FY27 non-GAAP adjusted FCF margin guidance of **23%**. A single-quarter 6% margin should not be used by itself to infer a permanent deterioration in capital efficiency.
3. **$6B AWS commitment is cloud COGS / minimum-spend risk, not owned capex.** Snowflake committed to $6B of AWS spend over five years. This affects gross margin, take-or-pay risk and operating leverage, but does not mean Snowflake is becoming a balance-sheet-heavy infrastructure owner.
4. **‘ROIC delayed to FY28–29’ is unsupported.** No explicit invested-capital reconstruction is provided, and the premise partly rests on the incorrect heavy-asset framing.
5. **Gross-margin interpretation needs precision.** FY27 non-GAAP product gross-margin guidance fell from 75% to 74%, and management explicitly attributed this to a higher mix of fast-growing AI workloads with lower contribution margins today. That supports ‘AI mix dilutes product gross margin’, but not necessarily ‘low-margin compute resale’ as the sole mechanism.
6. **RPO trend can be sourced directly from S1.** Q4 FY26 RPO was $9.77B, Q1 FY27 $9.21B, Q2 FY27 $9.00B. This is a valid sequential decline, but Snowflake itself warns RPO is affected by renewal timing, contract length, seasonality, FX and rollover; it should not be read alone as bookings deterioration.
7. **Peer/control-plane framing is incomplete.** The case should include Databricks / Microsoft Fabric for data-platform competition and Salesforce / ServiceNow for enterprise agent/control-plane competition, while distinguishing their economic functions.

## What worked well

- Correctly distinguishes actual Q2 product revenue from FY27 guidance.
- Correctly identifies AI as a measurable contributor to growth acceleration while keeping the exact revenue contribution as management commentary rather than hard segment disclosure.
- Correctly leaves AI absolute revenue and CoCo standalone pricing undisclosed/unknown.
- Correctly avoids physical-infrastructure ledgers such as MW or GPU-hours.
- Good base-vs-alternative structure around enterprise AI demand, lower AI contribution margins and platform competition.

## v0.4 read-through

This case exposes a software-specific runtime failure mode: WorkBuddy understands the revenue mechanism but tends to force cloud minimum-spend commitments into a physical-capital framework. The Skill should preserve the distinction between **cloud COGS / take-or-pay commitments** and **owned capex / invested capital** when moving from AI infrastructure to enterprise software.
