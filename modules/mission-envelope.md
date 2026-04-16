# Mission Envelope

## Module Purpose

This module defines the **intended operating envelope** for IX-HfTaZen-Shield v0.1.

The purpose of this module is to prevent scope drift and force all downstream architecture, material, thermal, and validation decisions to stay tied to a **specific problem class** instead of a vague “extreme heat shield” concept.

This module answers five questions:

1. What problem is the system trying to solve?
2. Where on a vehicle is the system intended to be used?
3. What thermal environment is assumed?
4. What performance band is being targeted?
5. What is explicitly outside the design envelope?

---

## v0.1 Mission Definition

IX-HfTaZen-Shield v0.1 is a **localized reusable extreme-heat TPS insert concept** intended for **small-area, high-severity thermal zones** where:

- local heat flux is much higher than adjacent acreage
- oxidation must be treated as a baseline concern
- thermo-structural mismatch is likely to matter
- attachment survivability is part of the problem
- instrumentation is required to understand degradation
- active relief may be justified only in the worst local zones

This is not an all-body TPS concept.  
It is a **hotspot-focused protection architecture**.

---

## Intended Application Class

### Primary target use zones

The architecture is intended for **localized high-severity regions** such as:

- leading-edge-adjacent zones
- nose-adjacent high-heating regions
- stagnation-proximal inserts
- sharp local geometry transitions where heat concentration is elevated
- reusable hot-structure subregions that exceed normal acreage TPS assumptions

### Use-characteristic summary

The concept is intended for situations where the following are all true:

- the exposed area is limited
- the thermal demand is unusually high
- reuse or limited reuse is desirable
- passive TPS may be insufficient at the most severe local peaks
- the structure beneath the thermal surface must be protected from heat and stress
- direct measurement of system condition is valuable

---

## v0.1 Atmospheric Assumption

### Baseline environment
**Oxidizing atmosphere**

All core thermal-protection reasoning in v0.1 assumes an oxidizing environment unless explicitly marked otherwise.

Why this matters:

- oxidation is treated as a first-order threat
- pure melting-point arguments are insufficient
- barrier behavior and scale stability matter
- carbon-rich exposed-face solutions are disfavored
- survivability depends on chemistry, interfaces, joints, and thermal gradients, not just nominal material peak temperature

### Secondary environment
**Low-oxygen / inert / vacuum behavior may be discussed analytically**, but it is not the baseline design case for v0.1.

---

## Coverage Scope

### Included coverage type
**Localized insert architecture**

The concept is intended to cover a **small fraction of a vehicle’s thermal acreage**, specifically the regions where ordinary reusable TPS logic may run out of margin.

### Excluded coverage type

The following are out of scope for v0.1:

- full-body TPS coverage
- broad acreage reusable tile systems
- full blunt-body heat shield replacement
- complete launch vehicle or spacecraft external skin protection
- generalized planetary entry shell design
- complete nose-to-tail thermal architecture

---

## Thermal Severity Bands

These bands are design targets, not validated results.

### Band A — Baseline Passive Target
**500–800 W/cm²**

Interpretation:
- this is the preferred passive-only operating band
- the architecture should be designed to treat this range as the most credible passive target for localized short-duration severe heating

### Band B — Stretched Passive Target
**800–1000 W/cm²**

Interpretation:
- this is an aggressive passive design band
- this band is intended to define the upper end of passive ambition before local-only active relief becomes difficult to avoid

### Band C — Assisted Local Hotspot Target
**1000–1500 W/cm²**

Interpretation:
- this band is not assumed to be comfortably handled by passive reradiation and stack design alone
- if this band is pursued, it must be through local-only assistance such as hotspot intercept, heat spreading, transpiration-like relief, or equivalent high-severity mitigation logic
- this band must not be generalized to full-area coverage

---

## Thermal Objective

The thermal objective of IX-HfTaZen-Shield is not to make the exposed face “cold.”

The thermal objective is to:

1. keep the hot face within a credible survivable regime
2. delay or reduce oxidation-driven loss of function
3. reduce thermal transfer into deeper structure
4. prevent thermally driven structural failure at the interface layers
5. preserve enough margin for measurement and inspection
6. optionally intercept a controlled fraction of heat for downstream secondary use without degrading TPS function

---

## Reuse Assumption

### Baseline reuse posture
**Reusable or limited-reuse localized TPS concept**

The repo assumes the architecture is intended to survive more than one exposure in principle, but v0.1 does **not** claim validated cycle life.

### What v0.1 does not assume
- unlimited reuse
- airline-like turnaround
- broad-area orbital TPS reuse
- field-proven refurbishment logic
- flight-demonstrated repeatability

---

## Active Relief Assumption

### Baseline
**Passive-first**

The architecture starts from a passive thermal-protection basis.

### Exception
**Local-only active relief is allowed** if it is clearly justified by the severity of the local hotspot and if it does not turn the entire architecture into a broad active-cooling system.

### v0.1 rule
If broad active cooling becomes necessary across large areas, the concept has moved outside its intended mission envelope.

---

## Energy Recovery Assumption

### Allowed role
**Secondary downstream function only**

A controlled thermal intercept and recovery branch is allowed only if:

- TPS function remains primary
- energy conversion occurs downstream of the main protective stack
- the recovery branch does not require harmful heat leakage into protected structure
- the recovery branch can be removed without collapsing the core TPS concept

### Disallowed role
The energy-recovery branch must not be treated as:

- the main heat-relief mechanism
- proof that the shield is energy-positive
- a justification for worse insulation
- a reason to allow uncontrolled heat penetration

---

## Geometric Assumption

### v0.1 geometry posture
The concept assumes **segmented local inserts** are more credible than monolithic large-area slabs for the targeted use case.

This means the mission envelope assumes the architecture must be coherent under:

- edges
- joints
- seams
- local attachment points
- thermal expansion mismatch
- localized damage

If the system only works in a perfect monolithic sample with no interfaces, it does not satisfy the intended use envelope.

---

## Structural Assumption

The mission envelope assumes the thermal problem is inseparable from the structural problem.

This means the design must tolerate or explicitly address:

- differential thermal expansion
- interface stress
- local restraint
- crack initiation
- interlayer debond risk
- edge chipping or spall risk
- attachment degradation
- vibration and handling sensitivity at the insert level

---

## Validation Assumption

The mission envelope assumes the concept must be capable of progressing through:

1. analytical freeze
2. coupon screening
3. oxidation-control testing
4. thermal cycling
5. attachment / mismatch testing
6. high-heat coupon exposure
7. damage tolerance checks
8. subscale integrated insert testing

If the concept cannot be expressed in this staged way, the mission envelope is considered too vague and must be narrowed.

---

## Measurement Assumption

The mission envelope assumes that **observability is part of the design**.

At minimum, the concept should eventually be capable of supporting:

- surface temperature estimation
- backface temperature measurement
- interface temperature awareness
- strain or displacement awareness
- damage logging
- pre/post test inspection comparison
- measured comparison between expectation and result

A design that only “looks strong on paper” but cannot be instrumented is outside the desired program posture.

---

## Out-of-Scope Environments

The following are explicitly outside the v0.1 mission envelope unless added in a later version:

- deep-space radiation shielding as a core requirement
- cryogenic tank wall integration
- long-duration broad-area hot-soak management across whole vehicles
- underwater thermal protection
- engine hot-section internal hardware
- terrestrial furnace insulation products
- general-purpose armor or ballistic systems
- large-area power-generation skins
- civilian building thermal materials
- non-aerospace heat management applications

---

## Out-of-Scope Claims

The mission envelope does not support claims such as:

- “works for any spacecraft”
- “works for any hypersonic vehicle”
- “full reentry solution”
- “better than all existing TPS systems”
- “proven for orbital reuse”
- “proven at flight scale”
- “universal extreme-environment shield”
- “integrated radiation shield by default”

---

## Success Condition for This Module

This module is successful if it forces every future technical decision to answer:

- Does this improve localized extreme-heat protection?
- Does this remain within the defined thermal bands?
- Does this preserve passive-first logic?
- Does this avoid uncontrolled broad-area complexity?
- Does this remain testable at coupon and subscale levels?
- Does this stay inside the declared scope boundaries?

If the answer is no, the decision belongs outside v0.1.

---

## v0.1 Mission Envelope Summary

**Identity:** localized reusable extreme-heat TPS insert concept  
**Baseline environment:** oxidizing atmosphere  
**Primary target band:** 500–800 W/cm²  
**Stretched passive band:** 800–1000 W/cm²  
**Assisted hotspot band:** 1000–1500 W/cm² local only  
**Coverage:** small-area severe-heat regions, not full-vehicle TPS  
**Architecture posture:** passive-first, local-active-if-necessary  
**Energy posture:** secondary downstream recovery only  
**Validation posture:** analytical-to-coupon-to-subscale  
**Claim posture:** no flight-worthiness claim
