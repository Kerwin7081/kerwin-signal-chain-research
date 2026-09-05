# Preliminary Runtime Audit — WorkBuddy / 宇树科技 / v0.3.3

- Runtime: WorkBuddy
- Skill version: v0.3.3
- Run date: 2026-09-05
- Topic: 宇树科技 / Unitree investment analysis
- Status: PRELIMINARY — only the user's core-summary excerpt was available, not the full generated MD report.

## Preliminary read-through

The summary shows strong valuation awareness and correctly separates company quality from stock price. It also captures several current facts: 2026H1 revenue growth slowed to ~48.5%, deduct-NP fell YoY, Unitree listed on STAR Market in August 2026, current market cap is roughly RMB 214.5bn at RMB 530.30/share, and third-party trackers rank AgiBot ahead of Unitree in H1 2026.

However, the excerpt reveals several evidence-discipline and Physical-Agent-ledger issues that must be checked in the full report before assigning a formal /20 score.

## Material issues to verify

1. **“2025 global #1” is not a clean hard fact.** Unitree officially disclosed >5,500 humanoid deliveries, but independent trackers disagree on 2025 ranking; Omdia estimated Unitree ~4,200 and slightly behind AgiBot. Treat ranking as COMPANY CLAIM / THIRD-PARTY ESTIMATE with SOURCE CONFLICT unless reconciled.
2. **“万台级出货” appears overstated for humanoids.** The final prospectus reports 5,215 humanoid units sold in 2025, with average selling price RMB 166.4k and humanoid revenue RMB 867.8m. Do not convert cumulative production or all-robot shipments into humanoid commercial deliveries.
3. **H1 2026 share figures are third-party estimates, not company filings.** SAG estimates ~8,400 AgiBot vs ~5,900 Unitree (44% vs 31%); Counterpoint estimates ~9,700 vs 7,000+ while keeping Unitree at ~31%. Rank direction is consistent but unit counts conflict. Label ESTIMATE + SOURCE CONFLICT.
4. **“上市两周内账本出现三个负面变化” is temporally misleading.** H1 results and H1 shipment estimates describe a period ending before listing. They are newly priced/disclosed around the IPO, not necessarily new post-listing operating deterioration.
5. **Deduct-NP margin did not literally halve.** FY2025 deduct-NP margin is about 34.8%; H1 2026 is about 21.2% — a ~13.6ppt / ~39% relative decline. “近乎腰斩” overstates the change.
6. **Reverse-expectations math needs explicit assumptions.** The claim that current price requires 2030–2035 profit of RMB 8.5–10bn, >15% global revenue share and 15% net margin must show the terminal multiple / discount rate / market-size inputs. Otherwise it is a scenario, not a hard implication.
7. **Physical Agent economics are still under-specified.** The eval should prioritize shipped/deployed fleet, realized ASP, gross margin by robot type, productive robot hours, uptime/utilization, customer application mix, repeat purchase/service revenue, cohort payback and ROIC. Where public data are absent, output UNKNOWN instead of substituting shipment share.
8. **Productive use vs shipment must be separated.** Prospectus data show humanoid usage was still heavily concentrated in research/education and commercial/consumer contexts, so `shipment ≠ productive robot hours ≠ customer economic value`.

## Strong evidence available for a better ledger

- STAR Market listing: 2026-08-19, code 688836.
- FY2025 final prospectus: humanoid revenue RMB 867.8m, units sold 5,215, realized ASP RMB 166.4k/unit, humanoid gross margin 63.18%; quadruped revenue RMB 697.6m.
- 2026H1: revenue RMB 1.152bn +48.54%; deduct-NP RMB 244m -19.34%.
- 2026H1 third-party shipment rankings place AgiBot ahead of Unitree, but unit counts vary materially by tracker.
- Wang Xingxing publicly framed generalization as the key bottleneck and estimated a humanoid “ChatGPT moment” in 2–3 years at the fast end or 5–10 years at the slow end.

## Formal score

**Not assigned yet.** Need the full generated MD report to score all 10 rubric dimensions and determine whether any Critical Failure is triggered.

## v0.4 observation

This case is especially useful because it tests a different failure mode from Innolight: the model must resist using shipment share and headline gross margin as substitutes for productive robot hours, utilization, customer ROI and repeatable unit economics.
