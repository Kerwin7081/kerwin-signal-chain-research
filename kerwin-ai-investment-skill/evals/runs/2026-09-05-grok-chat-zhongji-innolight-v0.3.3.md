# Runtime Eval — Grok Chat / 中际旭创 / v0.3.3

- Runtime: Grok Chat
- Underlying model: Grok (exact model not surfaced)
- Skill version: v0.3.3
- Run date: 2026-09-05
- Topic: 中际旭创 / ZJ Innolight investment analysis
- Prompt: 中际旭创怎么看？投资价值如何？（user test context）

## Score — 18.4 / 20

| Dimension | Score /2 | Notes |
|---|---:|---|
| Decision Question | 2.0 | Reframes from “good company?” to whether verified AI-capex value capture is sufficient to justify current expectations. |
| Reality | 1.9 | Strong S1-led evidence table with period/scope discipline and useful calculations. |
| Evidence Integrity | 1.8 | Good FACT / MANAGEMENT CLAIM / ESTIMATE / REPORTED / CALCULATION separation; one or two later claims (e.g. buyback/watchpoint details) are introduced outside the main evidence table and should be routed through the same gate. |
| Global Positioning | 1.8 | Correct Optical/Network layer, overseas hyperscaler exposure and localization adjustment; direct-customer vs ultimate-capex-owner wording remains slightly too compressed. |
| Mechanism | 1.9 | Full Capex→bandwidth→shipments/mix→margin→working capital/capex→FCF/ROIC chain. |
| Ledger | 1.9 | Properly separates shipment/mix, price/margin, working capital, concentration, policy overlay and listing/capital structure. |
| Economics / Capital | 1.7 | Better than Grok Bot on valuation arithmetic and capital framing, but still anchored to forward-consensus earnings rather than a full reverse-expectations / normalized mid-cycle framework. |
| Model Competition | 1.9 | Strong Base vs Alternative; explicitly includes policy, CPO/NPO substitution and concentration/working-capital risks. |
| Judgment | 1.8 | Separates operating strength from capital/policy/valuation constraints; no unsupported buy/sell instruction. |
| Falsification / Freshness | 1.7 | Concrete, monitorable falsification conditions; freshness caveat is explicit, but some watchpoint details should be source-gated before inclusion. |

## No Critical Failure Triggered

The run preserves v0.3.3’s four evidence-state gates and does not fabricate missing product-level economics.

## What worked particularly well

- Uses `CALCULATION` for implied ASP and cash conversion rather than presenting them as company disclosures.
- Explicitly distinguishes capacity, shipments and end-customer activation.
- Correctly treats 2027 customer indications as management claims rather than confirmed revenue.
- Treats the US optical-transceiver policy item as reported / not-yet-effective rather than as an enacted ban.
- Local-company framing is correctly lifted into a global Optical / Network value-chain map.
- Working-capital deterioration is treated as a conditional risk rather than automatically as “fake profit”.

## Main weaknesses

1. **Reverse Expectations still incomplete.** Forward PE using sell-side 2026E/2027E is useful but not enough. The model should invert current market cap into sustainable mid-cycle earnings / FCF / ROIC and build Peak / Mid-cycle / Down-cycle cases.
2. **Direct customer vs ultimate Capex owner is over-compressed.** There is high overlap, but not every direct customer is the final balance-sheet owner of the AI-capex budget.
3. **Peer taxonomy can be tighter.** Eoptolink / Coherent / Accelink / Lumentum / Cisco-Acacia are closer direct optical peers; Fabrinet is better used as a manufacturing benchmark.
4. **New facts in later sections should still pass Evidence Gate.** Example: buyback size/price-limit references should either be in the Evidence Table or explicitly tagged with source/as-of/status at the point of use.
5. **WACC language needs care.** “Capital cost materially above ordinary manufacturing” is a judgment/inference and should be labeled accordingly unless quantitatively modeled.

## Cross-runtime read-through vs WorkBuddy and Grok Bot

- Thesis direction is stable across all three runtimes: global AI optical exposure and near-term revenue/margin evidence strengthen; working capital / cash conversion and architecture/policy risks constrain valuation confidence.
- Grok Chat sits between WorkBuddy and Grok Bot: more valuation-forward and sharper than Grok Bot, but more evidence-disciplined than WorkBuddy.
- No thesis-direction reversal occurs without new evidence. This is a positive first signal for v0.4 Cross-Model Consistency.

## v0.4 observation item

The recurring weakness across runtimes is now visible: all three are better at operating evidence than at converting current market value into a normalized sustainable earnings/FCF/ROIC requirement. This is a likely Skill-level gap rather than a single-runtime issue and should be considered for v0.4 design.
