# IX-HfTaZen-Shield

IX-HfTaZen-Shield is a **test-first thermal protection system (TPS) concept** focused on **localized reusable extreme-heat protection**.

**Current status:** analytical architecture with defined failure modes and planned coupon/subscale validation.  
**Flight-worthiness claim:** none.  
**License:** Apache License 2.0.

---

## What this repo is

This repo defines a **localized extreme-heat TPS insert architecture** for the hardest small-area heat zones rather than a full-vehicle heat shield.

The project focuses on a narrow, disciplined problem:

- localized severe thermal zones
- oxidizing environments as the baseline case
- passive-first protection
- thermo-structural survivability
- oxidation control
- strain-decoupled support logic
- optional local-only active hotspot relief
- optional downstream thermal intercept and recovery
- embedded health-monitoring logic
- staged coupon-to-subscale validation planning

This repo is meant to stand on its own as an original systems concept and validation program structure.

---

## What this repo is not

IX-HfTaZen-Shield is **not**:

- a flight-ready heat shield
- a full-vehicle TPS
- a proven replacement for validated aerospace TPS
- a universal reentry solution
- a passive 4,500–5,000°C oxidizing-wall claim
- a “self-powering shield”
- a baseline radiation-shield package
- a manufacturing or certification package

This repo does **not** claim superiority over NASA, SpaceX, or any validated aerospace TPS.

---

## Core thesis

The program thesis is:

> A credible localized reusable extreme-heat TPS concept is more likely to emerge from a **layered, stress-aware, oxidation-aware, instrumented architecture** than from a single miracle material.

That means the architecture treats the following as first-class problems:

- hot-face chemistry
- oxidation control
- thermal reradiation
- thermo-structural mismatch
- support and attachment survivability
- boundary and seam behavior
- local hotspot relief
- downstream thermal accounting
- observability
- evidence discipline

---

## Mission envelope

### Intended use
Localized severe-heat insert zones such as:

- leading-edge-adjacent regions
- nose-adjacent hot zones
- stagnation-proximal local inserts
- sharp local geometry transitions with elevated heating
- reusable hot-structure subregions that exceed normal acreage-TPS assumptions

### Baseline environment
**Oxidizing atmosphere**

### Thermal target bands
These are **analytical target bands**, not validated operating claims.

- **Band A — Baseline passive local zone:** `500–800 W/cm²`
- **Band B — Stretched passive local zone:** `800–1000 W/cm²`
- **Band C — Assisted local hotspot zone:** `1000–1500 W/cm²` local only

### Coverage scope
This repo targets **small-area severe-heat inserts**, not full-body TPS coverage.

---

## Max-01 reference architecture

The canonical v0.1 reference configuration is `Max-01`.

### Required layers
1. **HTZ-01 Radiative UHTC Face**  
2. **OX-02 Oxidation-Control Transition**  
3. **SD-03 Strain-Decoupling Interlayer**  
4. **TC-04 Thermal Choke Carrier**  
5. **HB-07 Health-Monitoring Backplane**  
6. **SJ-08 Seal & Joint Management Ring**

### Optional layers
7. **AR-05 Active Relief Branch** *(local only, if earned)*  
8. **IR-06 Thermal Intercept & Recovery Cassette** *(downstream only, if earned)*

### Architecture posture
- localized
- segmented
- passive-first
- oxidation-aware
- stress-aware
- instrumented
- active-only-if-needed
- energy-recovery-secondary
- test-first
- evidence-gated

---

## Materials direction for v0.1

The repo is locked at the **candidate-family** level for v0.1.

### Primary candidate directions
- **HTZ-01:** Hf-rich high-entropy carbide / carbonitride in the `Hf–Ta–Zr–W–(C,N)` lane
- **OX-02:** `HfSiCN`-class oxidation-control transition
- **SD-03:** refractory compliant interlayer architecture
- **TC-04:** refractory or ceramic-compatible segmented carrier
- **AR-05:** porous-UHTC local transpiration-style relief
- **IR-06:** TPV-first thermal intercept and recovery
- **HB-07:** high-temperature-compatible sensing backplane
- **SJ-08:** refractory-compatible joint and edge-management architecture

The repo does **not** claim that these families are validated in integrated service.  
They are the locked design direction for v0.1.

---

## Why this architecture exists

The design is built around a simple correction:

A heat shield does not fail only because the surface gets hot.

It can also fail because of:

- oxidation beneath the surface
- crack-assisted oxygen ingress
- thermo-structural mismatch
- rigid support restraint
- heat leakage into deeper structure
- seam or boundary failure
- damage growth from small defects
- optional features that add more complexity than value

So this repo does not chase one “best material.”  
It builds a **system architecture** around the real failure paths.

---

## Optional branch logic

### AR-05 Active Relief Branch
AR-05 is allowed only as a **local severe-hotspot branch**.

It exists only if:
- the hotspot is local
- passive margin is too thin
- the branch reduces a meaningful local burden
- the branch does not create worse oxidation or structural harm
- the branch remains optional

AR-05 is not broad active cooling.

### IR-06 Thermal Intercept & Recovery Cassette
IR-06 is allowed only as a **secondary downstream branch**.

It exists only if:
- a controlled intercepted thermal stream already exists for protection reasons
- the cassette stays downstream and removable
- the cassette does not reward harmful heat leakage
- the cassette remains secondary to TPS survival

IR-06 is not the primary cooling mechanism.

---

## Health monitoring

IX-HfTaZen-Shield is not allowed to be a blind stack.

The architecture includes a health-monitoring backplane to support:

- backface temperature awareness
- interface thermal awareness
- strain or displacement trend awareness
- anomaly logging
- comparison between analytical expectations and later measured behavior

Monitoring is included to improve truth, not hype.

---

## Allowed claim ceiling for v0.1

The maximum allowed public summary for this repo is:

> IX-HfTaZen-Shield is a test-first TPS concept focused on localized reusable extreme-heat protection. Current status: analytical architecture with defined failure modes and planned coupon/subscale validation. No flight-worthiness claim.

Anything stronger than that exceeds the repo’s current evidence tier.

---

## Validation path

The repo is structured around a staged validation campaign.

### Validation stages
- **V0** — Analytical Freeze
- **V1** — Chemistry-Screening Coupons
- **V2** — Oxidation-Control Coupons
- **V3** — Thermal Shock / Cycle Coupons
- **V4** — Attachment / Mismatch Stack Coupons
- **V5** — High-Heat Coupon Exposure
- **V6** — Deliberate Damage Coupons
- **V7** — Local Active-Relief Demonstrator
- **V8** — Thermal Intercept & Recovery Demonstrator
- **V9** — Integrated Subscale Insert

The order is intentional.  
The repo does not skip from concept framing to grand claims.

---

## Evidence posture

The repo is currently locked to:

- **E0** — concept framing
- **E1** — analytical reasoning
- **E2** — literature-informed material screening

It does **not** claim coupon evidence, integrated evidence, or operational evidence yet.

That means the repo is best understood as a **structured technology concept and validation framework**, not a completed engineering proof.

---

## Repo structure

```text
.
├── LICENSE
├── PROJECT_CHARTER.md
├── README.md
├── REPO_METADATA.md
├── assets/
├── bom/
├── modules/
│   ├── claims-evidence-ladder.md
│   ├── hotspot-active-relief.md
│   ├── materials-screening.md
│   ├── mission-envelope.md
│   ├── oxidation-recession.md
│   ├── risk-failure-register.md
│   ├── shield-health-monitoring.md
│   ├── stack-architecture.md
│   ├── thermo-structural-budget.md
│   ├── thermal-intercept-recovery.md
│   └── validation-campaign.md
├── reference-configs/
│   └── max-01.md
└── validation/
    ├── v0-analytical-freeze.md
    ├── v0-freeze-checklist.md
    ├── v1-candidate-matrix.md
    ├── v1-chemistry-screening.md
    ├── v2-oxidation-control.md
    ├── v2-pairing-matrix.md
    ├── v3-cycle-comparison-matrix.md
    ├── v3-thermal-shock-cycle.md
    ├── v4-attachment-mismatch.md
    ├── v4-stack-comparison-matrix.md
    ├── v5-exposure-comparison-matrix.md
    ├── v5-high-heat-exposure.md
    ├── v6-damage-comparison-matrix.md
    ├── v6-deliberate-damage.md
    ├── v7-local-active-relief.md
    ├── v8-thermal-intercept-recovery.md
    ├── v7-v8-demonstrator-matrix.md
    └── v9-integrated-subscale-insert.md

Development priorities

The repo prioritizes the following in order:

scope discipline
claims discipline
architecture clarity
material-family screening
oxidation and interface realism
thermo-structural realism
damage honesty
optional-branch keep / cut discipline
integrated insert coherence

If a lower-priority feature hurts a higher-priority requirement, the lower-priority feature loses.

Kill criteria

The concept must be narrowed, revised, or branched if any of the following become true:

the architecture requires broad active cooling to stay plausible
the decoupling logic cannot be made coherent
the energy-recovery branch harms protection
seams and boundaries dominate the insert uncontrollably
the stack depends on perfection to survive
the concept cannot be validated in stages
claims start outrunning evidence
Why this repo may still matter

This repo does not claim that it has already built a better heat shield than validated aerospace programs.

What it does claim is narrower and more honest:

it frames a serious localized extreme-heat TPS problem correctly
it separates hot-face ambition from oxidation control
it treats mismatch and boundaries as core architecture problems
it refuses to let optional complexity hide weak fundamentals
it gives the concept a real path from analytical architecture to staged evidence

That is the point of v0.1.

License

This project is licensed under the Apache License 2.0.
See LICENSE.
