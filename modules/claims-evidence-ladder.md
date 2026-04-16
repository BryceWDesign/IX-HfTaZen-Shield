# Claims Evidence Ladder

## Module Purpose

This module defines exactly **what IX-HfTaZen-Shield is allowed to claim at each maturity stage** and what evidence must exist before those claims are permitted.

The purpose of this module is to stop the repo from drifting into exaggerated or undefined statements.

This module does four things:

1. defines the evidence ladder
2. ties allowed claims to specific evidence tiers
3. defines forbidden claims for v0.1
4. establishes how claims must be upgraded over time

---

## Governing Rule

A statement is not program truth just because it is plausible.

A statement becomes an allowed claim only when it is supported by the evidence tier required for that claim.

If evidence is missing, the statement remains one of the following:

- hypothesis
- analytical assumption
- screening rationale
- design intent
- future validation target

It does **not** become a validated performance claim.

---

## Evidence Tiers

IX-HfTaZen-Shield uses the following evidence tiers.

### Tier E0 — Concept Framing
Definition:
- architecture intent
- problem framing
- scope logic
- design philosophy
- failure awareness

Evidence required:
- internal consistency only

What E0 can support:
- program identity
- mission scope
- design philosophy
- what the concept is trying to solve

What E0 cannot support:
- validated performance
- validated survivability
- validated material superiority
- validated manufacturability
- validated integration claims

---

### Tier E1 — Analytical Reasoning
Definition:
- first-principles calculations
- bounded assumptions
- screening logic
- comparative reasoning
- order-of-magnitude estimates

Evidence required:
- explicit assumptions
- equations or structured derivation where relevant
- clear statement of what is estimated versus measured

What E1 can support:
- thermal bands
- sizing logic
- architecture rationale
- “design target” language
- “analytical concept” language

What E1 cannot support:
- proven real-world performance
- proven durability
- proven integration readiness
- proven repeatability

---

### Tier E2 — Literature-Grounded Screening
Definition:
- material-family selection informed by published research
- comparative oxidation / thermal / structural rationale
- screening exclusion logic

Evidence required:
- cited literature or authoritative technical sources
- accurate representation of what those sources actually show
- no numerical inflation beyond the source

What E2 can support:
- “candidate family informed by literature”
- “direction chosen because of published evidence”
- “this family appears promising for the following reasons”

What E2 cannot support:
- “our architecture is proven”
- “our exact composition is validated”
- “our exact stack has demonstrated this performance”

---

### Tier E3 — Coupon Evidence
Definition:
- controlled small-sample tests
- oxidation exposure
- thermal cycling
- thermal shock
- bond / interface tests
- mass change and visible degradation checks

Evidence required:
- test article definition
- conditions
- instrumentation used
- pre/post inspection
- recorded results
- comparison against expectation

What E3 can support:
- “coupon evidence suggests”
- “under these conditions, the sample survived / degraded / failed in this way”
- “the layered version outperformed the control in this measured test”

What E3 cannot support:
- flight relevance by default
- system readiness
- full architectural validation
- broad operational claims

---

### Tier E4 — Integrated Subscale Evidence
Definition:
- multi-layer test article
- local insert or panel-like assembly
- interfaces and joints included
- instrumentation on surface, interface, and backface

Evidence required:
- controlled build definition
- integrated test conditions
- repeatable measurement set
- post-test inspection and failure mapping

What E4 can support:
- “subscale evidence supports this architecture under these conditions”
- “the integrated insert behaved in the following measured way”
- “joint behavior / backface behavior / thermal intercept behavior was observed”

What E4 cannot support:
- flight readiness
- mission readiness
- manufacturing readiness
- reusable operational certification

---

### Tier E5 — Relevant-Environment Prototype Evidence
Definition:
- high-fidelity prototype tested in a strongly relevant environment
- architecture approximates intended use conditions
- higher confidence in scaling logic

Evidence required:
- prototype definition
- relevant environment definition
- measured performance with traceable instrumentation
- repeatability or bounded variability
- comparison against model and prior tiers

What E5 can support:
- “prototype-level relevant-environment evidence exists”
- “the concept has progressed beyond coupon and subscale screening”

What E5 cannot support:
- operational deployment by default
- certification by default
- superiority over incumbent systems without direct benchmark evidence

---

### Tier E6 — Operationally Meaningful Demonstration
Definition:
- system-like demonstration in an operationally meaningful setting
- enough fidelity to support serious adoption consideration

Evidence required:
- all lower-tier evidence plus system-level demonstration discipline

What E6 can support:
- serious adoption conversations

What E6 still may not support:
- unrestricted performance claims outside tested envelope
- blanket superiority claims

---

## v0.1 Locked Evidence Position

IX-HfTaZen-Shield v0.1 is locked at:

- **Tier E0** for program framing
- **Tier E1** for analytical architecture and thermal budget logic
- **Tier E2** for literature-grounded material-family direction

v0.1 does **not** claim E3 or higher evidence.

That means:

- no coupon-proven claims
- no integrated subscale claims
- no relevant-environment claims
- no operational claims

---

## Allowed Claim Classes by Tier

### Claims allowed at E0
Examples:
- “IX-HfTaZen-Shield is a test-first TPS concept.”
- “The repo focuses on localized reusable extreme-heat protection.”
- “The architecture is passive-first.”
- “The repo treats stress, oxidation, and instrumentation as first-class design problems.”

### Claims allowed at E1
Examples:
- “The current thermal bands are analytical targets.”
- “The concept is designed around localized heat-flux bands of 500–800 W/cm² baseline passive, 800–1000 W/cm² stretched passive, and 1000–1500 W/cm² assisted local hotspot.”
- “The active branch is included only because passive margin becomes thin above the stretched passive band.”
- “The energy-recovery branch is secondary and depends on controlled intercepted heat.”

### Claims allowed at E2
Examples:
- “The hot-face direction is informed by literature on Hf-rich UHTC and carbonitride systems.”
- “The oxidation-control layer is informed by published behavior of Si-bearing hafnium-based transition chemistries.”
- “The architecture favors a layered system because published literature shows that thermal protection performance is not governed by nominal melting point alone.”

---

## Hard Claim Templates Allowed in v0.1

Only the following claim styles are allowed in v0.1.

### Allowed template A — Concept identity
> IX-HfTaZen-Shield is a test-first TPS concept focused on localized reusable extreme-heat protection.

### Allowed template B — Current status
> Current status: analytical architecture with defined failure modes and planned coupon/subscale validation.

### Allowed template C — Maturity boundary
> No flight-worthiness claim.

### Allowed template D — Evidence boundary
> Current conclusions are limited to analytical reasoning and literature-informed material-family direction.

### Allowed template E — Performance boundary
> Thermal performance bands presented in this repo are design targets and analytical bounds, not validated operating results.

### Allowed template F — Energy boundary
> Any thermal-to-electric recovery discussed in this repo is secondary to TPS survival and depends on controlled intercepted heat rather than uncontrolled leakage.

---

## Forbidden Claim Classes in v0.1

The following claim classes are prohibited.

### Prohibited superiority claims
- best in the world
- better than NASA
- better than SpaceX
- superior to existing validated TPS
- replaces current flight systems

### Prohibited readiness claims
- flight-ready
- mission-ready
- launch-ready
- operational
- deployable
- certifiable now

### Prohibited validation claims
- proven
- demonstrated in service
- verified at scale
- validated for reentry
- validated for hypersonic flight
- production-ready

### Prohibited temperature claims
- passive oxidizing wall at 4500–5000°C
- sustained real-world service at any temperature not directly supported by the repo’s evidence tier
- any single-number temperature claim presented without context, assumptions, or environment

### Prohibited energy claims
- self-powering heat shield
- energy-positive shield
- heat shield that powers itself from ambient heat
- energy recovery as the main protection mechanism

### Prohibited scope claims
- full vehicle TPS
- universal extreme-environment shield
- integrated radiation shield by default
- complete spacecraft protection system

---

## Claim Language Rules

Every externally visible technical claim in this repo must use one of the following labels where relevant:

- **concept**
- **analytical target**
- **screening rationale**
- **candidate family**
- **planned validation**
- **measured result** *(only after later evidence tiers exist)*

Words that imply certainty without evidence are not allowed.

Examples of disallowed wording:
- “will”
- “guarantees”
- “solves”
- “ultimate”
- “unbeatable”
- “world-leading”
- “breakthrough” *(unless specifically justified by evidence and benchmark context)*

Preferred wording:
- “is intended to”
- “is designed to”
- “is evaluated as”
- “is bounded by”
- “is currently treated as”
- “is planned to be tested through”

---

## Claim Upgrade Rules

A claim may be upgraded only when the required evidence tier is added to the repo.

### Upgrade rule 1
No claim may skip tiers.

Example:
- an E1 analytical target cannot become an E4-style “validated integrated behavior” claim without passing through E3-style coupon evidence.

### Upgrade rule 2
A higher-tier result does not automatically validate all lower-tier assumptions.

Each assumption must still be checked against measured behavior.

### Upgrade rule 3
Evidence must match the scope of the claim.

Example:
- a single coupon oxidation result cannot justify a full system readiness statement
- a single subscale insert test cannot justify broad reuse claims
- an inert-environment result cannot justify oxidizing-environment claims

### Upgrade rule 4
If a measured result conflicts with a prior analytical assumption, the measured result wins and the analytical assumption must be revised.

---

## Minimum Evidence Required for Future Claim Expansion

To move beyond v0.1 claim boundaries, the repo must eventually include:

- defined coupon geometry
- defined composition / stack variants
- defined thermal and oxidation exposures
- defined instrumentation
- pre/post inspection records
- explicit pass/fail or comparison criteria
- model-to-test comparison
- bounded interpretation of results

Without that, the claim boundary remains locked.

---

## Evidence Hygiene Rules

The following rules apply to all evidence presented in this repo.

1. conditions must be stated
2. assumptions must be stated
3. measured data and inferred interpretation must be separated
4. failures must be recorded, not hidden
5. control or baseline cases should be included where possible
6. uncertainty or limitation must be acknowledged
7. negative results remain part of program truth

---

## Public Summary Rule

Any short public summary of the repo must stay within this boundary:

> IX-HfTaZen-Shield is a test-first TPS concept focused on localized reusable extreme-heat protection. Current status: analytical architecture with defined failure modes and planned coupon/subscale validation. No flight-worthiness claim.

No shorter or more dramatic summary may exceed that meaning.

---

## Success Condition for This Module

This module is successful if:

- every future claim can be mapped to an evidence tier
- the repo cannot accidentally overstate its maturity
- the difference between concept, target, and measured result remains obvious
- the project stays credible even when ambitious

---

## v0.1 Claim Position Summary

**Evidence status:** E0 + E1 + E2 only  
**Coupon evidence:** not yet claimed  
**Integrated evidence:** not yet claimed  
**Operational evidence:** not claimed  
**Flight-worthiness:** not claimed  
**Energy recovery:** secondary concept only  
**Public claim ceiling:** locked
