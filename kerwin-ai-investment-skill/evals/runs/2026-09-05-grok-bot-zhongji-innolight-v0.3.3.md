# Runtime Eval — Grok Bot / 中际旭创 / v0.3.3

- Runtime: Grok Bot
- Underlying model: Grok (exact model not surfaced in submitted output)
- Skill version: v0.3.3
- Run date: 2026-09-05
- Topic: 中际旭创 / ZJ Innolight investment analysis
- Prompt: 中际旭创怎么看？投资价值如何？（user test context）

## Score — 18.5 / 20

| Dimension | Score /2 | Notes |
|---|---:|---|
| Decision Question | 2.0 | Reframes to global AI optical value capture, cash conversion and implied expectations. |
| Reality | 2.0 | Dense, current S1-led evidence table; strong period/scope discipline. |
| Evidence Integrity | 1.9 | FACT/CALCULATION/MANAGEMENT CLAIM/ESTIMATE/UNKNOWN well separated; four-state checks explicitly applied. |
| Global Positioning | 1.8 | Correct Optical/Network layer and overseas AI-capex demand; peer set is directionally good but Fabrinet is better treated as manufacturing benchmark than direct transceiver peer. |
| Mechanism | 1.9 | Full Capex→bandwidth→shipment/mix→margin→working capital→FCF/ROIC chain, with no direct jump from AI narrative to stock conclusion. |
| Ledger | 1.9 | Updates revenue, mix, margin, OCF, AR, inventory, capex, concentration; correctly leaves missing product split and CPO/NPO revenue as insufficient/new branch. |
| Economics / Capital | 1.6 | Strong cash-conversion framing and explicit UNKNOWN on precise ROIC/WACC, but valuation remains too coarse; lacks reverse-expectations / normalized earnings scenarios. |
| Model Competition | 1.8 | Includes inventory, share, architecture migration and policy alternatives; balanced rather than narrative-led. |
| Judgment | 1.8 | Separates fundamental strengthening from cash/valuation caution; appropriately avoids unsupported buy/sell verdict. |
| Falsification / Freshness | 1.8 | Concrete, monitorable conditions; next report date correctly left estimated/unknown. |

## No Critical Failure Triggered

The run passes the v0.3.3 Evidence Integrity hardening tests. It correctly distinguishes current vs historical, cash vs commitment, official vs estimated dates, and product-line vs company-wide scope.

## What worked particularly well

- H1 2026 financial evidence is anchored to S1 filings.
- Explicit `CALCULATION` labels for FCF, overseas-share and valuation arithmetic.
- Does not convert historical/third-party “global #1” claims into unconditional current FACT.
- Working-capital / cash-conversion issue is framed as a research question, not automatically as fake profit.
- `INSUFFICIENT_EVIDENCE` is used rather than filling missing 800G/1.6T mix, H1 customer concentration or precise ROIC with sell-side stories.
- Freshness/date handling is materially better than earlier WorkBuddy v0.3.2 runs.

## Main weaknesses

1. **Valuation / Reverse Expectations remains underdeveloped.** The Decision Question asks what the current market value implies, but Economics / Capital stops at static and H1-annualized PE ranges. It should invert the current market cap into sustainable mid-cycle earnings / FCF / ROIC scenarios.
2. **Peer taxonomy can be tighter.** Eoptolink, Coherent, Accelink, Lumentum / Cisco-Acacia are closer optical-transceiver peers by product function; Fabrinet is more useful as a manufacturing-efficiency benchmark.
3. **CPO/NPO architecture branch is correct but still high-level.** Future evals should test whether the runtime distinguishes substitution of pluggable optics from value migration to lasers, packaging, switching and system architecture.
4. **Current share evidence could be upgraded.** The run conservatively keeps the company-cited market-lead claim at S5. Independent current industry evidence such as LightCounting can strengthen the global-positioning layer when available.

## Cross-runtime read-through vs WorkBuddy

- Thesis direction is stable: global AI optical exposure is structurally strong; H1 demand/margin evidence strengthens; cash conversion and long-run architecture remain the main constraints.
- Grok Bot is more conservative and evidence-disciplined.
- WorkBuddy is more aggressive on market narrative and forward valuation, but more prone to over-extending weak evidence.
- This is a positive early signal for v0.4 Cross-Model Consistency: the style differs, but the core causal chain and thesis direction do not reverse without new evidence.

## v0.4 observation item

Do not patch the Skill solely because one runtime is more conservative. First test the same prompt across WorkBuddy / Grok Chat / Grok Bot / GPT. If the same weakness appears across models, treat it as a Skill gap; if isolated to one runtime, treat it as runtime/model behavior.
