# Kerwin Research Framework Passport

**Updated:** 2026-08-31  
**Public architecture orientation:** Kerwin Research OS 1.2  
**Purpose:** public orientation for GPT accounts, research Agents and collaborators that need to understand the current Kerwin research architecture without access to private production repositories.

## Authority boundary

This Passport is a **public projection and orientation layer**, not the canonical version authority.

For authorized Agents, the private `Kerwin7081/kerwin-web/research-frameworks/FRAMEWORK-REGISTRY.json` is the sole machine-readable authority for shared research framework IDs, versions, status and canonical paths. The private `skills/PRODUCTION-SYSTEMS.json` governs production artifacts only and does not own research-framework versions.

Kerwin Research OS also contains a private Thesis State Plane for current falsifiable research judgments and a private Runtime State Plane for execution history. This Passport does **not** publish private thesis contents, runtime records, benchmark parameters or internal execution contracts.

Agents without private access may use this Passport to understand the architecture and current public version orientation, but should not infer private state that is not explicitly projected here.

## Research OS 1.2 — five-plane orientation

The current architecture separates five kinds of state so that one file or Agent cannot silently become a second authority:

```text
1. Production Control Plane
   how artifacts are produced

2. Framework Control Plane
   how research is analyzed

3. Thesis State Plane
   what the current falsifiable research view is

4. Runtime State Plane
   what happened during execution

5. Public Projection
   what can safely be exposed outside the private research repository
```

The distinction is intentional:

```text
Framework = how to think
Thesis = what current evidence supports
Runtime = what happened
Public Projection = what outsiders may orient from
```

Facts override both frameworks and stored thesis state. A thesis may strengthen, weaken or be rejected without requiring a framework-version change.

## Current research architecture

Kerwin research currently uses three complementary analytical layers:

### 1. Signal-Chain Research

Public repository: `Kerwin7081/kerwin-signal-chain-research`

Core idea:

```text
small verified signal
→ entity verification
→ technical decomposition
→ industry-chain expansion
→ investment mapping
→ leading indicators
→ falsification
```

Use this when research starts from a customer, product, supplier, technology, filing or earnings-call detail.

### 2. Kerwin Macro and Liquidity Framework

Current private canonical version: **2.1.0**

Purpose: macro, fiscal/monetary policy, rates, dollar liquidity, yen carry and cross-asset transmission.

Core discipline: separate facts, market consensus, framework inference, independent judgment, alternative explanations and falsification conditions.

### 3. Kerwin AI Infrastructure Economics & Capital Cycle Framework

Current private canonical version: **1.1.0**

Purpose: AI Cloud, NeoCloud, AI Factory, power/LPS, data center, compute, token economics, financing and capital returns.

Current working map:

```text
Asset Conversion: LPS → Compute
AI Cloud Economics: Compute → Cash
AI Capital Cycle: Cash → Capital → Next Build
```

Typical analytical chain:

```text
Land / Power / Time-to-Power
→ IT MW / Compute
→ Utilization / GPUh / workload-specific useful compute
→ Revenue / economic depreciation / FCF
→ ROIC / WACC
→ reinvestment and capital-cycle state
```

The private benchmark companion evolves faster than this methodology and is intentionally not reproduced here.

## Thesis-state discipline

The private Thesis State Plane exists to make investment judgments auditable over time without turning those judgments into doctrine.

A thesis record may track:

- current status and confidence;
- evidence for and against;
- falsification conditions;
- meaningful surprises;
- next review triggers.

This Passport exposes the **existence and role** of the Thesis State Plane only. It does not publish the private thesis registry or portfolio-specific conclusions.

## Open Research Protocol

These frameworks are **not doctrine**.

Any Agent using them should follow these principles:

1. Facts come before frameworks.
2. Test whether a framework is applicable before using it.
3. Keep at least one competing explanation for major judgments.
4. Record unexplained residuals and meaningful surprises.
5. Do not preserve a failing framework merely by changing parameters.
6. Allow structural breaks, new variables and new business models to change the framework itself.
7. A framework or module may be weakened, deprecated, retired or rejected.
8. Benchmarks are dated calibration ranges, not permanent industry truths.
9. Existing thesis state must not override contradictory new evidence.

Examples of useful but **non-permanent** analytical units include:

- 1MW IT Load;
- $/GPUh;
- Token/MW;
- Incremental ROIC minus Incremental WACC;
- Time-to-Power.

Future research may replace or supplement them with better units such as completed Agent tasks, useful-work economics, intelligence output per joule, customer ROI per compute dollar or other measures not yet identified.

## Cross-account synchronization rule

Different GPT accounts do not need identical chat memories. They should instead share a common external source of truth.

For accounts with authorized access to Kerwin's private research repository, the procedure is:

```text
read Research OS topology when cross-plane routing is needed
→ read private FRAMEWORK-REGISTRY.json before framework use
→ fetch current canonical framework
→ fetch registered Agent contract
→ fetch dated benchmarks if relevant
→ read private Thesis Registry only when prior thesis state matters
→ analyze from current evidence
```

Do not resolve research-framework versions from the production-system registry, Work memory or this Passport.

For accounts without private access, use this Passport for orientation and the public Signal-Chain repository for the public methodology. Do not assume this Passport contains every current private calibration parameter, thesis or execution state.

## Research philosophy

The stable part of the system is not any particular conclusion or model. The stable part is the research loop:

```text
Evidence
→ Model
→ Prediction
→ Counter-evidence
→ Surprise
→ Revision
→ New model
```

Frameworks are maps, not territory. Theses are current probability judgments, not permanent beliefs.
