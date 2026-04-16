# Max-01 Reference Configuration

## Configuration Identity

**Configuration name:** Max-01  
**Program:** IX-HfTaZen-Shield  
**Configuration status:** frozen analytical reference for v0.1  
**Maturity class:** analytical architecture only  
**Flight-worthiness claim:** none  
**Purpose:** provide the canonical reference stack and design assumptions used by all downstream v0.1 reasoning and validation planning

---

## Configuration Role

Max-01 is the baseline reference configuration for IX-HfTaZen-Shield v0.1.

It exists to stop architecture drift.

Any later module that discusses:
- thermal behavior
- material direction
- stress logic
- active hotspot relief
- energy recovery
- instrumentation
- validation

must map back to Max-01 unless it explicitly declares itself a variant.

---

## Configuration Scope

Max-01 is intended for:

- localized reusable extreme-heat TPS inserts
- small-area high-severity thermal zones
- oxidizing environments as the baseline case
- passive-first operation
- local-only active relief if required
- secondary downstream energy recovery only if it does not compromise TPS function

Max-01 is not intended for:

- full-vehicle TPS
- large-area acreage coverage
- broad active-cooling shells
- radiation shielding by default
- production hardware claims
- flight hardware claims

---

## Locked Design Posture

Max-01 is frozen to the following posture:

- **localized**
- **segmented**
- **passive-first**
- **oxidation-aware**
- **stress-aware**
- **instrumented**
- **active-only-if-needed**
- **energy-recovery-secondary**
- **test-first**
- **evidence-gated**

These posture rules are part of the configuration and must not be silently changed.

---

## Locked Severity Bands

Max-01 is defined around the following thermal severity bands.

### Band A — Baseline Passive Local Zone
**500–800 W/cm²**

Interpretation:
- preferred passive operating target for the localized insert concept
- no active branch required by default

### Band B — Stretched Passive Local Zone
**800–1000 W/cm²**

Interpretation:
- aggressive passive range
- stronger sensitivity to oxidation, interface behavior, and thermo-structural margin

### Band C — Assisted Local Hotspot Zone
**1000–1500 W/cm²**

Interpretation:
- local-only severe hotspot band
- active relief is allowed and may be necessary
- this band must not be generalized to broad-area use

These bands are analytical targets, not validated operating results.

---

## Locked Layer Stack

Max-01 uses the following canonical layer stack.

### Required layers
1. **HTZ-01 Radiative UHTC Face**
2. **OX-02 Oxidation-Control Transition**
3. **SD-03 Strain-Decoupling Interlayer**
4. **TC-04 Thermal Choke Carrier**
5. **HB-07 Health-Monitoring Backplane**
6. **SJ-08 Seal & Joint Management Ring**

### Optional layers
7. **AR-05 Active Relief Branch**
8. **IR-06 Thermal Intercept & Recovery Cassette**

Optional layers may only be used under their defined gating rules.

---

## Locked Layer Intent

### HTZ-01 Radiative UHTC Face
Role:
- primary exposed hot face
- high-severity thermal encounter surface
- reradiative first defense boundary

Configuration rule:
- HTZ-01 must not be treated as a miracle monolith that solves oxidation, attachment, and deep heat rejection by itself

### OX-02 Oxidation-Control Transition
Role:
- buried chemistry and oxidation-control transition
- protects deeper interfaces from direct oxidation-driven degradation

Configuration rule:
- OX-02 exists to support survivability, not to replace HTZ-01 as the primary exposed truth layer

### SD-03 Strain-Decoupling Interlayer
Role:
- reduce thermal mismatch stress
- limit crack-driving restraint between upper hot layers and deeper support

Configuration rule:
- Max-01 assumes stress decoupling is required for credibility

### TC-04 Thermal Choke Carrier
Role:
- structural support
- thermal-flow moderation
- stable base for segmented insert logic

Configuration rule:
- TC-04 must not become a hidden thermal short

### HB-07 Health-Monitoring Backplane
Role:
- measurement, logging, anomaly awareness, and post-test comparison support

Configuration rule:
- Max-01 is not allowed to become a blind stack

### SJ-08 Seal & Joint Management Ring
Role:
- seam, edge, and boundary control
- insert-perimeter survivability support

Configuration rule:
- joints are treated as core architecture, not a finishing detail

### AR-05 Active Relief Branch
Role:
- local-only heat interception or hotspot burden reduction

Configuration rule:
- AR-05 may only appear in Band C or analytically justified edge cases near the top of Band B

### IR-06 Thermal Intercept & Recovery Cassette
Role:
- downstream secondary energy conversion from controlled intercepted heat

Configuration rule:
- IR-06 must never dictate the upstream thermal-protection architecture

---

## Locked Material Direction

Max-01 is frozen at the **candidate family level**.

It does not claim final supplier-grade or fabrication-grade materials in v0.1.

### HTZ-01 candidate family
**Hf-rich high-entropy carbide / carbonitride**
within the **Hf–Ta–Zr–W–(C,N)** design lane

Intent:
- push the exposed face toward the strongest currently credible oxidizing-UHTC direction available to this repo

### OX-02 candidate family
**HfSiCN-class oxidation-control transition**

Intent:
- support more stable oxidation behavior and reduce deeper interfacial damage risk

### SD-03 candidate family
**high-temperature compliant interlayer concept**

Intent:
- reduce transmitted thermal-mismatch stress
- allow segmented hot-face survivability to remain plausible

### TC-04 candidate family
**refractory or ceramic-compatible segmented carrier concept**

Intent:
- provide support without undermining the thermal role of the upper stack

### AR-05 candidate family
One of:
- porous-UHTC local relief concept
- refractory heat-pipe local intercept concept
- other tightly bounded local thermal-relief concept

### IR-06 candidate family
**TPV-first thermal recovery cassette**
with optional **TEG tail stage**

### HB-07 candidate family
**high-temperature-compatible sensorized backplane**

### SJ-08 candidate family
**refractory-compatible joint / seam / edge management architecture**

---

## Locked Geometric Posture

Max-01 assumes:

- localized insert geometry
- segmented architecture
- explicit edges and seams
- attachment-sensitive behavior
- nontrivial local mismatch strain
- localized boundary failure risk

Max-01 does not assume:
- perfect monolithic slabs
- seam-free behavior
- uniform whole-body heating
- geometry-free material performance

---

## Locked Thermal Logic

The thermal path of Max-01 is frozen as follows:

1. HTZ-01 receives the direct local heat load
2. HTZ-01 reradiates a major share of the thermal burden
3. OX-02 protects deeper chemistry and helps manage oxidation-driven interfacial damage
4. SD-03 reduces structural penalty from thermal gradients and mismatch
5. TC-04 slows deeper heat penetration while maintaining support
6. AR-05, if present, intercepts or redistributes heat only in severe local hotspots
7. IR-06, if present, accepts only controlled intercepted heat after the protective logic has already done its job
8. HB-07 measures surviving thermal behavior at the backside and interfaces
9. SJ-08 protects the boundary from becoming the dominant failure path

No module may contradict this logic without declaring a new reference configuration.

---

## Locked Structural Logic

The structural logic of Max-01 is:

- thermal protection and structural survivability are inseparable
- interface damage is treated as a primary failure class
- decoupling is required because high local heat creates large expansion mismatch risk
- segmentation is favored over naive monolithic scaling
- joints and edges are high-risk design zones by default

This means Max-01 assumes failure is just as likely to begin:
- beneath the hot face
- at the joint ring
- at the decoupling interface
- at a restrained attachment point

as it is at the exposed face itself.

---

## Locked Active-Relief Rules

AR-05 may only be enabled in Max-01 when all of the following are true:

1. the region is a **localized severe hotspot**
2. passive behavior in that local zone is analytically too close to the survivability cliff
3. the active branch is confined to the local zone
4. the active branch does not create broad-area cooling dependence
5. removing the active branch still leaves a coherent passive architecture underneath
6. the active branch has a clear thermal job that can be measured

If these conditions are not met, AR-05 stays disabled.

---

## Locked Energy-Recovery Rules

IR-06 may only be enabled in Max-01 when all of the following are true:

1. there is a **controlled intercepted heat stream**
2. the recovery path sits downstream of the main TPS function
3. the stack does not leak extra harmful heat just to feed recovery
4. the energy branch is secondary to survival
5. removing IR-06 does not invalidate the base thermal stack
6. the claimed electric output is explicitly bounded and labeled as analytical unless measured later

IR-06 must never be used to justify:
- weaker insulation
- higher backface heat leakage
- claims of self-powering TPS
- claims of net-positive thermal protection

---

## Locked Measurement Requirements

Max-01 requires the architecture to remain compatible with:

- surface temperature estimation
- backface temperature measurement
- interface thermal awareness
- strain or displacement awareness
- test logging
- pre/post inspection comparison
- damage localization
- comparison between analytical expectation and later measured behavior

A variant that removes observability is not Max-01.

---

## Locked Failure Focus

Max-01 is explicitly shaped around the following failure classes:

- hot-face oxidation degradation
- exposed-face cracking and spall initiation
- brittle interface failure
- thermal mismatch damage
- deep thermal leakage
- joint/seam failure
- local hotspot escalation
- instrumentation blindness
- optional-feature overcomplexity
- architectural self-contradiction

Any later work that ignores these failure classes is outside Max-01 discipline.

---

## Locked Exclusions

Max-01 excludes the following by default:

- radiation shielding pack
- full-spacecraft TPS coverage
- broad active cooling
- broad-area energy-harvesting skins
- cryogenic whole-body thermal management
- full production BOM claims
- supplier lock-in
- cost optimization
- manufacturing process optimization
- operational refurbishment strategy
- broad aerodynamic integration claims

These may become separate future branches, but they are not part of Max-01.

---

## Allowed Max-01 Summary Statement

The configuration may be summarized as follows:

> Max-01 is the frozen v0.1 reference configuration for IX-HfTaZen-Shield: a segmented, passive-first, localized extreme-heat TPS insert architecture with an Hf-rich UHTC hot-face direction, oxidation-control transition, strain-decoupled support stack, optional local-only active relief, and optional downstream thermal intercept and recovery.

This summary must remain bounded by the repo’s claims-evidence rules.

---

## Forbidden Max-01 Summary Statements

The following are forbidden:

- “Max-01 is proven”
- “Max-01 is flight ready”
- “Max-01 outperforms NASA systems”
- “Max-01 is the best heat shield”
- “Max-01 survives any reentry”
- “Max-01 is self-powering”
- “Max-01 integrates radiation shielding by default”

---

## Configuration Freeze Rules

Max-01 may only be changed if one of the following occurs:

1. a later commit explicitly versions a new reference configuration
2. a contradiction is discovered between layers or mission envelope
3. a future evidence tier forces a design correction
4. a locked rule is shown to be incoherent

Any silent drift away from this file is a repo error.

---

## Exit Criteria for Max-01 v0.1

Max-01 v0.1 is considered properly frozen when all of the following exist:

- mission envelope
- claims evidence ladder
- canonical stack architecture
- material screening direction
- oxidation and thermo-structural budget logic
- validation sequence
- failure register

At that point, Max-01 becomes the reference against which all later v0.1 analysis is judged.

---

## Max-01 Summary

**Identity:** localized reusable extreme-heat TPS insert reference configuration  
**Environment:** oxidizing baseline  
**Architecture posture:** passive-first, segmented, instrumented  
**Thermal target bands:** 500–800 W/cm² baseline passive, 800–1000 W/cm² stretched passive, 1000–1500 W/cm² assisted local hotspot  
**Required layers:** HTZ-01, OX-02, SD-03, TC-04, HB-07, SJ-08  
**Optional layers:** AR-05, IR-06  
**Energy posture:** secondary downstream only  
**Status:** frozen analytical reference for v0.1  
**Claim ceiling:** no flight-worthiness claim
