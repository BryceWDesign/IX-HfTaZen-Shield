# Hotspot Active Relief

## Module Purpose

This module defines the **AR-05 Active Relief Branch** for IX-HfTaZen-Shield v0.1.

Its job is to answer:

1. when local active relief is allowed
2. why local active relief exists at all in a passive-first architecture
3. what kinds of active relief are admissible
4. how local thermal burden is estimated and gated
5. what conditions cause the active branch to be rejected, deferred, or isolated from the baseline stack

This module does **not** claim that AR-05 is validated.

It freezes the analytical logic for when and how active local hotspot relief may be included in Max-01.

---

## Governing Rule

AR-05 exists only to solve a **localized severe hotspot problem** that the passive stack cannot carry with credible margin.

AR-05 is **not**:

- a broad cooling shell
- a whole-body thermal-management concept
- a substitute for hot-face quality
- a substitute for oxidation-control quality
- a substitute for stress-decoupling quality
- a justification for weak passive design
- proof that the base stack is mature

The architecture remains passive-first even when AR-05 is present.

---

## Why AR-05 Exists

The Max-01 stack is designed to be credible in:

- **Band A:** 500–800 W/cm²  
- **Band B:** 800–1000 W/cm²  

But once local loading enters:

- **Band C:** 1000–1500 W/cm²  

the passive exposed-face and interface burden can crowd the severe oxidizing survivability cliff too closely.

That does not automatically mean the concept fails.

It means a bounded local mechanism may be justified to:

- shave peak local thermal burden
- protect the exposed face from being driven too far into rapid degradation
- reduce interface penalty beneath the hotspot
- preserve local geometry and measurement opportunity
- stop a small hotspot from dictating the whole stack design

This is the only reason AR-05 exists.

---

## AR-05 Activation Philosophy

AR-05 is governed by **strict local activation criteria**.

The branch may only be considered when all of the following are true:

1. the thermal problem is **localized**
2. the passive stack is analytically too close to its survivability cliff in that local region
3. the local burden is large enough to justify added complexity
4. the active branch can be bounded physically and analytically
5. the active branch does not introduce worse system-level penalties than the hotspot itself
6. the passive architecture underneath remains coherent without AR-05

If any of those conditions are not satisfied, AR-05 stays out.

---

## Allowed AR-05 Roles

AR-05 is allowed to perform only the following functions.

### Role A — Peak local heat interception
Reduce the highest local thermal burden at a hotspot so the exposed stack behaves more like a lower heat-flux band.

### Role B — Local thermal redistribution
Spread thermal burden away from a narrow hotspot into a region that can tolerate it better, provided the redistribution does not simply move failure elsewhere.

### Role C — Hotspot survivability extension
Delay local degradation long enough for the stack to remain coherent and observable.

### Role D — Downstream controlled thermal handoff
Deliver a bounded intercepted thermal stream to downstream architecture if and only if that downstream path does not compromise TPS function.

---

## Forbidden AR-05 Roles

AR-05 must never be used as:

- the main thermal strategy everywhere
- an excuse to stop caring about emissivity and oxidation
- a backdoor to broad active cooling
- a hidden way to admit that the passive stack is not viable
- a marketing mechanism for dramatic claims
- an energy-harvesting gimmick
- a reason to weaken TC-04 or HB-07
- a justification for uncontrolled internal heat routing

---

## AR-05 Candidate Concept Classes

The v0.1 program allows only the following concept classes for AR-05.

### Primary concept class
**Porous-UHTC local transpiration-style relief**

Intent:
- provide local burden reduction at the most severe thermal spots
- stay tightly coupled to the hotspot problem
- preserve the localized nature of the branch

Why primary:
- it directly targets the hotspot rather than trying to cool everything
- it maps cleanly to a localized insert architecture
- it is easier to justify as a zone-specific exception than broad-area cooling logic

---

### Secondary concept class
**Refractory heat-pipe local intercept**

Intent:
- pull heat away from a narrow hotspot and route it to a more manageable downstream or lateral region

Why secondary:
- strong for sharp local peaks
- potentially elegant for bounded thermal transport
- still carries real integration and mismatch challenges that must remain explicit

---

### Reserve concept class
**Tightly bounded local heat-spreading branch**

Intent:
- lower the peak thermal intensity by redistributing it within a limited region

Why reserve:
- may be useful if the primary or secondary concepts prove too integration-heavy
- less attractive if it merely moves the failure from one layer to another

---

## Excluded AR-05 Concepts

The following are excluded from v0.1.

### Excluded X1
**Broad-area active cooling**

Reason:
- outside the mission envelope
- destroys passive-first discipline

### Excluded X2
**Peltier-style front-line cooling**

Reason:
- wrong scale for the targeted thermal burden
- analytically incoherent for the severe hotspot regime

### Excluded X3
**Ambient harvester networks as thermal relief**

Reason:
- not serious for local extreme-heat burden reduction
- violates the thermal logic of the stack

### Excluded X4
**Cryogenic whole-body undercooling**

Reason:
- outside v0.1 scope
- overcomplicates a localized insert problem

### Excluded X5
**Undefined “advanced cooling” placeholders**

Reason:
- if the branch has no physical job and no measurable target, it does not belong in the architecture

---

## AR-05 Thermal Gating Logic

AR-05 enters the discussion only when a local region crosses from aggressive passive conditions into analytically thin passive margin.

### Gating Band Rule

#### No AR-05 by default
**500–800 W/cm²**

Interpretation:
- passive-first region
- no active relief required by default

#### AR-05 normally deferred
**800–1000 W/cm²**

Interpretation:
- still a passive-first region
- AR-05 may only be considered if a highly localized geometry or boundary condition analytically pushes the insert beyond safe margin

#### AR-05 allowed and likely justified
**1000–1500 W/cm²**

Interpretation:
- severe local hotspot band
- AR-05 becomes a legitimate option
- use must still be localized and bounded

---

## AR-05 Sizing Logic

The first-pass local intercept burden is estimated as:

**Δq = q_hotspot − q_target**

Where:
- `q_hotspot` = estimated local hotspot heat flux
- `q_target` = desired effective local burden after relief

For local hotspot area `A`, the required intercepted thermal burden is:

**Q_intercept = Δq × A**

This relation is analytical only, but it forces discipline.

AR-05 must be able to answer:

- what burden is being removed
- over what area
- toward what thermal target
- by what local mechanism
- with what side effects

---

## Example AR-05 Burden Cases

These examples are analytical only.

### Case 1
Local hotspot:
**1200 W/cm²**

Desired effective target:
**1000 W/cm²**

Intercept burden:
**200 W/cm²**

For:
- **25 cm²** → **5 kW**
- **50 cm²** → **10 kW**
- **100 cm²** → **20 kW**

---

### Case 2
Local hotspot:
**1500 W/cm²**

Desired effective target:
**1000 W/cm²**

Intercept burden:
**500 W/cm²**

For:
- **10 cm²** → **5 kW**
- **25 cm²** → **12.5 kW**
- **50 cm²** → **25 kW**

These examples show the real point:

AR-05 is a **kilowatt-class local thermal-management branch**, not a decorative enhancement.

---

## AR-05 Integration Rules

The active branch is only coherent if its integration is coherent.

### Rule A1 — Locality
AR-05 must remain spatially local to the hotspot it is meant to relieve.

### Rule A2 — Passive-stack preservation
The passive stack must remain logically complete even if AR-05 is removed.

### Rule A3 — Oxidation awareness
AR-05 must not create a worse oxidation-access path than the passive design it is trying to improve.

### Rule A4 — Structural awareness
AR-05 must not introduce a more dangerous local weakness in SD-03, TC-04, or SJ-08 than the thermal burden it removes.

### Rule A5 — Boundary awareness
If AR-05 changes local movement, seams, or support paths, that effect must be treated as part of the architecture, not as a side note.

### Rule A6 — Measurement compatibility
AR-05 must remain compatible with HB-07 observability and later validation.

### Rule A7 — Downstream discipline
If AR-05 feeds a controlled intercepted heat stream into IR-06 or other downstream logic, that stream must remain bounded and secondary.

---

## AR-05 by Concept Class

## Primary: Porous-UHTC Local Transpiration-Style Relief

### Role
Relieve only the most severe local hotspot by allowing bounded cooling action directly where the passive stack is most threatened.

### Advantages
- targets the actual hotspot
- stays physically tied to the extreme local zone
- can reduce peak local thermal burden instead of merely moving heat laterally

### Risks
- flow-path integration complexity
- local oxidation consequences if poorly integrated
- added local vulnerability if the porous region becomes a weakness
- seam or edge complications at the relief boundary

### Gating posture
Allowed only in Band C or very near the upper edge of Band B with explicit justification.

---

## Secondary: Refractory Heat-Pipe Local Intercept

### Role
Remove heat from a narrow hotspot and transport it away from the most severe location.

### Advantages
- strong local-intercept logic
- more bounded than broad cooling
- potentially useful for sharply localized extreme points

### Risks
- thermal expansion mismatch at integration points
- support complexity
- routing complexity
- possibility of moving failure to a new region if not bounded

### Gating posture
Allowed as a comparison lane or alternate AR-05 implementation.

---

## Reserve: Local Heat-Spreading Branch

### Role
Flatten a narrow local peak by spreading heat into nearby structure that retains margin.

### Advantages
- conceptually simple
- may reduce local peak severity without full fluid-path complexity

### Risks
- may simply move the problem
- can worsen deeper-structure burden if not carefully bounded
- can harm thermal-choke logic if overused

### Gating posture
Reserve only; not a preferred first active concept.

---

## AR-05 Failure Modes

AR-05 is useful only if it avoids turning into its own dominant failure source.

Primary active-branch failure modes include:

### AF-01 — Active branch not actually needed
Complexity is added to solve a problem that the passive stack could have handled.

### AF-02 — Oxidation-access penalty
The active branch opens a worse chemistry path than the hotspot it was meant to relieve.

### AF-03 — Structural penalty
The active branch weakens the local stack or creates a new crack-initiation zone.

### AF-04 — Thermal relocation failure
The branch removes a local peak only by causing unacceptable downstream or lateral thermal overload.

### AF-05 — Integration drift
The branch grows from a local exception into a hidden whole-architecture dependence.

### AF-06 — Measurement blindness
The branch changes the local thermal regime without preserving observability.

### AF-07 — Energy-recovery contamination
AR-05 becomes shaped around feeding IR-06 rather than protecting the stack.

---

## AR-05 Keep / Cut Decision Logic

AR-05 stays in the configuration only if it satisfies all of the following:

- solves a clearly defined local hotspot problem
- removes a meaningful amount of burden
- remains localized
- does not defeat oxidation logic
- does not defeat structural logic
- preserves passive-first coherence
- preserves measurement compatibility
- can be described in a coupon-to-subscale validation path

AR-05 gets cut if:

- it is added only because it sounds advanced
- it has no bounded thermal job
- it undermines the stack
- it creates broad active dependence
- it exists mainly to support energy recovery
- it makes the configuration harder to validate than to understand

---

## AR-05 Interaction with IR-06

AR-05 may hand off a controlled intercepted thermal stream to IR-06 only if:

1. thermal protection remains the reason AR-05 exists
2. the intercepted stream already exists because protection required it
3. IR-06 is downstream and secondary
4. removing IR-06 leaves AR-05 still justified on thermal grounds alone

If those conditions are not satisfied, AR-05 and IR-06 must remain separate.

---

## What Later Validation Must Prove

Future validation for AR-05 must eventually answer:

- how much local burden reduction actually occurred
- over what area
- at what thermal cost elsewhere
- whether the exposed-face and interface temperatures improved
- whether oxidation behavior improved or worsened
- whether boundary and joint behavior stayed acceptable
- whether the branch remained mechanically stable
- whether the branch stayed local in effect
- whether any downstream handoff remained controlled

Until then, AR-05 remains analytical.

---

## What This Module Does Not Claim

This module does **not** claim:

- validated active-relief performance
- validated transpiration effectiveness
- validated heat-pipe effectiveness in the IX-HfTaZen-Shield stack
- validated durability of AR-05 under repeated exposure
- validated oxidation compatibility
- validated recovery compatibility
- validated manufacturability
- validated operability

---

## Relationship to Other Modules

This module depends on:
- `stack-architecture.md`
- `materials-screening.md`
- `oxidation-recession.md`
- `thermo-structural-budget.md`

This module informs:
- `thermal-intercept-recovery.md`
- `risk-failure-register.md`
- `validation-campaign.md`
- later AR-05-specific test packages

---

## v0.1 Hotspot Active Relief Summary

AR-05 is a **local-only severe-hotspot exception branch**.

It exists because:

- the passive stack has a credible operating region
- that region is not unlimited
- some small severe hotspots may justify added local intervention
- the burden to be removed is often in the multi-kilowatt class
- any such intervention must remain bounded, secondary, measurable, and removable

That is the locked AR-05 logic for v0.1.
