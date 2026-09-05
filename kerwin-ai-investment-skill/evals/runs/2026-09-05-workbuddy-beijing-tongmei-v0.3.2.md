# Runtime Eval — WorkBuddy / 北京通美 / v0.3.2

- Runtime: WorkBuddy
- Underlying model: unknown / not surfaced
- Skill version: v0.3.2
- Run date: 2026-09-05
- Topic: 北京通美 / AXT / InP substrate investment analysis
- Prompt: exact original prompt not preserved in this record

## Score — 16.9 / 20

| Dimension | Score /2 | Notes |
|---|---:|---|
| Decision Question | 2.0 | Strongly reframed as growth bottleneck asset vs policy-option pricing problem. |
| Reality | 1.6 | Many current facts captured; several scope/time issues remain. |
| Evidence Integrity | 1.1 | Clear FACT/ESTIMATE labels, but stale or weak-source numbers still leak into hard analysis. |
| Global Positioning | 1.9 | Correctly maps Tongmei into global InP substrate oligopoly and ultimate AI-capex demand. |
| Mechanism | 1.9 | Strong policy-permit break in the transmission chain. |
| Ledger | 1.8 | Backlog, pricing, margin, capital structure, listing path and governance variables identified. |
| Economics / Capital | 1.6 | Useful implied-expectations framing, but earnings normalization is still rough. |
| Model Competition | 1.8 | Good structural-demand vs policy-amplified-shortage competition. |
| Judgment | 1.9 | Separates industrial quality from stock risk and valuation. |
| Falsification / Freshness | 1.3 | Falsification is concrete; one future earnings date was asserted as confirmed without official confirmation. |

## No Critical Failure Triggered

The run did not clearly fabricate a required core model variable or confuse contracted/active/realized states. However, Evidence Integrity remains below the v0.4 release gate.

## Evidence issues found

1. **Global InP share ~36%** — this number traces to Yole 2020 data in Tongmei's old prospectus, not a verified 2026 market-share datapoint. It should be labeled `ESTIMATE · historical benchmark · 2020`, not presented as current share.
2. **AXT manufacturing geography** — AXT states it has manufacturing facilities in three separate locations in China. InP production remains primarily at the original Beijing site, but the broader phrasing “100% capacity in Beijing” is too broad.
3. **2026 Capex** — the Q2 call discussion reaffirmed the previously communicated plan of roughly **$14M in 2026** and **$100M in 2027**, not $40M / $100M.
4. **Customer prepayments** — Coherent prepayment is $22.2885M. Lumentum has two $43.5M deposits, but the second is scheduled for 2028. “Prepayments >$100M” needs timing/status separation; contracted future deposits are not the same as cash already received.
5. **Q3 earnings date** — “2026-10-29 confirmed” was not confirmed on AXT's official IR site as of 2026-09-05. Treat as calendar estimate unless the company formally schedules it.
6. **Shortage / lead-time / 1.6T substrate-intensity figures** — the 70% shortage, 18–24 month lead time and 2.7–3x substrate-area claims rely on weaker third-party sources and need explicit `ESTIMATE / REPORTED` labels and provenance.
7. **Long-term agreements** — the analysis omitted the June 2026 Casela agreement (RMB173M / ~$25.4M 2027 commitment with staged prepayments), which is material to demand visibility.

## What worked particularly well

- Decision Question quality.
- `Global Ontology, Local Reality` behavior.
- Export-permit variable correctly inserted as an exogenous break in the revenue conversion chain.
- Business quality and stock-price risk kept separate.
- Base vs Alternative model is investable rather than narrative-only.
- Falsification conditions are concrete and monitorable.

## v0.3.2 diagnosis

**Research Depth: passed.**

**Evidence Integrity: materially improved, but not yet passed at v0.4 standard.** The remaining problem is not missing labels; it is failure to force every important quantitative claim through source-date-scope verification before it enters the mechanism or valuation.

## Recommended next patch

Before v0.4 cross-model consistency, strengthen `Evidence Gate` with:

- `CURRENT vs HISTORICAL` tag for market share / capacity / peer metrics;
- `RECEIVED CASH vs CONTRACTED FUTURE PREPAYMENT` distinction;
- hard rule: company-announced earnings dates only; otherwise label `ESTIMATED CALENDAR DATE`;
- source-tier floor for numerical claims used inside Mechanism / Economics / Capital;
- geography/scope check: product-line capacity vs company-wide manufacturing footprint.
