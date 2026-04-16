# IX-HfTaZen-Shield — Program Charter

## Program Identity

**Project name:** IX-HfTaZen-Shield  
**License:** Apache License 2.0  
**Current maturity target:** TRL 2–3 analytical concept with planned coupon and subscale validation only  
**Program posture:** test-first, evidence-gated, no flight-worthiness claim

---

## Mission

IX-HfTaZen-Shield exists to define and evaluate a **localized reusable extreme-heat thermal protection system (TPS) concept** for the harshest small-area heat zones, with a focus on:

- high local heat flux
- oxidizing environments as the baseline case
- reusable or limited-reuse protection logic
- thermo-structural survivability
- oxidation management
- attachment survivability
- instrumentation-backed validation
- optional secondary thermal energy recovery from **controlled intercepted heat**

This repo is not a general aerospace hype vehicle.  
It is a structured engineering concept intended to mature through defined evidence gates.

---

## Core Objective

Design a TPS architecture that can plausibly support **localized reusable extreme-heat protection** by combining:

1. a radiative ultra-high-temperature hot face
2. an oxidation-control transition strategy
3. a stress-decoupled attachment architecture
4. a thermal choke between hot face and deeper structure
5. an optional local-only active hotspot relief branch
6. an optional downstream thermal intercept and recovery branch
7. embedded health-monitoring logic for validation and fault detection

---

## Hard Scope Boundaries

The v0.1 program scope is intentionally narrow.

### In scope

- localized extreme-heat TPS insert architecture
- oxidizing-environment baseline analysis
- thermal and thermo-structural reasoning
- candidate material-family screening
- passive-first TPS design
- local-only active relief concepts
- controlled thermal intercept and secondary power-recovery concepts
- sensorized validation logic
- coupon-to-subscale validation planning
- claims discipline and evidence gating

### Out of scope

- full-vehicle TPS design
- full spacecraft or launch vehicle integration
- flight certification claims
- production manufacturing claims
- cost or procurement claims
- radiation shielding as a baseline function
- crew system integration
- broad-area cryogenic cooling architecture
- generalized ambient-energy scavenger fields
- claiming superiority over existing NASA or commercial flight TPS systems
- any statement that this concept is flight-ready, proven, or operational

---

## Program Thesis

The program thesis is:

> A credible localized reusable extreme-heat TPS concept is more likely to emerge from a **layered, stress-aware, oxidation-aware, instrumented architecture** than from a single miracle material.

This means the project treats the following as first-class problems:

- hot-face chemistry
- oxidation control
- thermal reradiation
- differential expansion and mismatch stress
- segmentation and joint survivability
- hotspot-only active relief
- backface thermal containment
- evidence quality
- failure observability

---

## Design Philosophy

### 1. Passive-first
The architecture starts with a passive thermal-protection basis.  
Active measures are only added where passive margins become too thin.

### 2. Localized, not universal
This concept is aimed at the hardest **small-area** heat zones, not the entire vehicle outer mold line.

### 3. Secondary power recovery only
Any energy conversion branch is subordinate to TPS survival.  
The shield must not depend on energy recovery to remain a shield.

### 4. Measurement over mythology
If the concept cannot be measured, bounded, and compared against explicit assumptions, it does not count as progress.

### 5. Failure-first development
The repo prioritizes identifying how the architecture fails before making ambitious claims about how it succeeds.

---

## Initial Technical Direction

The initial architecture direction for v0.1 is:

- **Hot face:** Hf-rich UHTC / carbonitride candidate family
- **Barrier:** oxidation-control transition layer
- **Interface:** high-temperature strain-decoupling interlayer
- **Carrier:** thermally conservative structural support
- **Optional branch A:** local-only active hotspot relief
- **Optional branch B:** controlled thermal intercept and recovery
- **Backside:** health-monitoring and fault-awareness backplane

This direction is analytical and provisional until evidence supports it.

---

## Program Non-Goals

IX-HfTaZen-Shield does **not** attempt to prove any of the following in v0.1:

- “ultimate heat shield”
- “best heat shield in the world”
- “better than NASA”
- “better than SpaceX”
- “4,500–5,000°C passive oxidizing wall”
- “energy-positive thermal protection”
- “drop-in replacement for existing flight TPS”
- “complete reentry solution”
- “broad-area reusable orbital TPS”
- “radiation shield and heat shield in one baseline stack”

Any future claim beyond the current scope must be earned through later evidence gates.

---

## Evidence Standard

A claim only becomes part of program truth when it is supported by one of the following:

1. analytical derivation with explicit assumptions
2. comparative material-family rationale grounded in literature
3. controlled bench or coupon evidence
4. subscale integrated test evidence
5. repeated, instrumented test agreement with declared expectations

Statements that are imaginative but unevidenced remain hypotheses.

---

## v0.1 Allowed Program Claim

The repo may state the following:

> IX-HfTaZen-Shield is a test-first TPS concept focused on localized reusable extreme-heat protection. Current status: analytical architecture with defined failure modes and planned coupon/subscale validation. No flight-worthiness claim.

This is the maximum allowed summary claim for v0.1.

---

## v0.1 Forbidden Program Claims

The repo must not claim any of the following:

- flight readiness
- mission readiness
- operational reuse capability
- superiority over validated NASA or commercial TPS
- validated manufacturability
- validated cost viability
- proven oxidation resistance in service
- proven active cooling performance
- proven thermal energy recovery performance in an aerospace environment
- proven survivability in real reentry or hypersonic flight
- baseline radiation-shield function

---

## Development Priorities

The order of importance for the program is:

1. scope discipline
2. architecture clarity
3. materials-family screening
4. thermal budget realism
5. stress and attachment survivability
6. validation design
7. instrumentation and observability
8. optional active relief
9. optional energy recovery

If any lower-priority feature compromises a higher-priority requirement, the lower-priority feature gets cut.

---

## Kill Criteria

The concept must be reconsidered or narrowed if any of the following occur during development:

- the architecture requires broad active cooling to stay plausible
- the stress-decoupling logic cannot be made coherent
- the thermal budget depends on unrealistic leakage into interior layers
- the energy-recovery branch materially harms TPS function
- the joint/seam logic becomes the dominant unsolved failure mode
- the concept cannot be expressed as a measurable coupon-to-subscale program
- the repo starts making claims that exceed its evidence tier

---

## Success Criteria for v0.1

v0.1 is successful if the repo establishes:

- a frozen mission envelope
- a frozen architecture stack
- explicit scope boundaries
- explicit allowed/forbidden claims
- a candidate materials direction
- a credible first-pass thermal and thermo-structural logic
- a defined failure register
- a staged first validation sequence

That is enough for v0.1.  
Anything beyond that belongs to later commits and later evidence.

---

## Program Rule

IX-HfTaZen-Shield stands on its own.  
The public repo must read as a coherent original system with native modules, native logic, and native validation structure.

No hidden or external concept lineage is required for the repo to make sense.

---

## Status

**Status:** Locked program charter for v0.1  
**Change policy:** Any change to scope, claim boundaries, or mission identity must be explicit and versioned.
