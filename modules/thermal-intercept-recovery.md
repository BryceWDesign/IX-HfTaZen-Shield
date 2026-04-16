# Thermal Intercept Recovery

## Module Purpose

This module defines the **IR-06 Thermal Intercept & Recovery Cassette** for IX-HfTaZen-Shield v0.1.

Its job is to answer:

1. why thermal recovery exists in this repo at all
2. where the recovery branch sits in the architecture
3. what kinds of recovery are allowed
4. what thermal source is admissible
5. how recovery is sized analytically
6. what rules prevent the recovery branch from corrupting the TPS mission

This module does **not** claim validated electrical performance.

It freezes the analytical logic for a secondary downstream thermal-recovery branch in Max-01.

---

## Governing Rule

IR-06 exists only as a **secondary downstream function**.

It is not part of the shield’s core right to exist.

The stack must remain a coherent localized extreme-heat TPS concept even if IR-06 is removed entirely.

If the recovery branch becomes necessary for the thermal architecture to make sense, the design has drifted into a self-defeating state.

---

## Why IR-06 Exists

The repo is already forced to think about controlled local thermal interception because:

- severe local hotspots can push passive margin too thin
- AR-05 may intercept a bounded local thermal burden
- any intercepted burden has to go somewhere
- a controlled intercepted stream may have enough quality to support bounded secondary energy conversion

That opens the door to a legitimate secondary question:

> If heat is already being intercepted for protection reasons, can a bounded downstream cassette recover some of that thermal power without harming the shield?

IR-06 exists to explore that answer.

It does **not** exist to justify extra heat leakage into protected structure.

---

## IR-06 Mission Posture

The thermal-recovery branch is locked to the following posture:

- **secondary**
- **downstream**
- **bounded**
- **nonessential to core protection**
- **dependent on controlled intercepted heat**
- **analytical in v0.1**
- **cuttable if it compromises the TPS**

These posture rules are part of Max-01 discipline.

---

## Allowed Thermal Source for IR-06

IR-06 may only consume thermal power from a **controlled intercepted stream**.

Acceptable sources include:

- thermal power intentionally intercepted by AR-05
- thermal power intentionally routed from a bounded hotspot-management path
- thermal power already captured for protection reasons by a thermal intercept manifold or equivalent local transport branch

IR-06 may **not** consume:

- random uncontrolled heat leakage through the stack
- broad-area interior soak
- heat intentionally leaked deeper just to improve electric output
- thermal damage that the stack failed to stop

If the heat source is not controlled, it is not admissible.

---

## Architectural Position of IR-06

IR-06 sits **downstream of the protective stack**.

That means:

1. HTZ-01, OX-02, SD-03, and TC-04 must retain their primary jobs
2. AR-05, if present, may create a controlled intercepted stream
3. only after that protective logic is satisfied may IR-06 be considered
4. HB-07 must remain able to monitor the consequences of thermal routing
5. SJ-08 must not be weakened to support IR-06 routing

IR-06 is downstream by definition, not by marketing language.

---

## Why “Ambient Harvesters Under the Shield” Are Rejected

The repo rejects the idea of broad ambient harvesters under the shield as a primary thermal strategy because the logic is backwards.

A TPS wants to:
- keep heat out of deeper structure
- reduce harmful thermal penetration
- preserve the thermal choke

A buried harvester needs:
- heat to cross a conversion device
- sufficient gradient to sustain conversion
- a downstream rejection path for unrecovered heat

Those goals conflict if harvesting is treated as the primary plan.

The only coherent role for energy conversion here is:

- intercept heat **after** protection logic has already captured it
- convert **part** of that bounded stream
- never depend on uncontrolled leak-through to feed the converter

That is the correction.

---

## IR-06 Candidate Concept Classes

The v0.1 program allows the following concept classes for IR-06.

### Primary concept class
**TPV-first thermal recovery cassette**

Intent:
- use a controlled high-temperature intercepted thermal stream
- convert a bounded fraction of that stream into electricity
- keep the recovery branch downstream and modular

Why primary:
- strongest conceptual fit for high-temperature intercepted thermal streams
- more serious than vague ambient scavenger logic
- better aligned with a local severe-heat architecture than low-grade-only conversion

---

### Secondary concept class
**TEG tail-stage recovery**

Intent:
- capture lower-grade residual thermal energy downstream of the hotter primary conversion region

Why secondary:
- useful as a lower-temperature tail stage
- not preferred as the main high-temperature conversion branch

---

### Reserve concept class
**Bench-only comparative thermal engine branch**

Intent:
- compare alternate recovery logic in non-integrated analytical or test contexts

Why reserve:
- may be useful for comparison work
- not part of the baseline integrated Max-01 stack

---

## Excluded IR-06 Concepts

### Excluded X1
**Ambient harvester field under the shield**

Reason:
- not coherent with the thermal choke logic
- encourages harmful heat leakage

### Excluded X2
**Energy-first TPS architecture**

Reason:
- the shield protects first and converts second

### Excluded X3
**Recovery branch that requires deliberate extra heating of protected layers**

Reason:
- self-defeating for TPS

### Excluded X4
**Mechanical-energy harvesting presented as major heat-relief**

Reason:
- does not address the central thermal burden in a serious way

### Excluded X5
**Unbounded generic “power generation” claim**

Reason:
- if the source stream is not defined, the branch is not engineering

---

## IR-06 Functional Roles

IR-06 is allowed to perform only the following roles.

### Role A — Secondary electric generation
Convert a bounded share of an already-controlled intercepted thermal stream into electricity.

### Role B — Sensor power support
Provide partial self-power for instrumentation, logging, health monitoring, or bounded local subsystem loads.

### Role C — Thermal accounting aid
Make the intercepted thermal stream explicit rather than letting it remain an undefined sink.

### Role D — Multifunction comparison branch
Support analysis of whether bounded secondary value can be extracted without harming the primary mission.

---

## Forbidden IR-06 Roles

IR-06 must never be framed as:

- the main survival mechanism
- proof that the shield is “self-powering”
- proof that the stack is net-positive
- a replacement for thermal isolation
- a justification for weaker passive performance
- the reason AR-05 exists
- the main innovation of the repo

The repo survives if IR-06 is cut.  
That is mandatory.

---

## IR-06 Sizing Logic

The first-pass recovery relation is:

**P_electric = η_recovery × Q_intercept**

Where:

- `P_electric` = electric output
- `η_recovery` = assumed recovery efficiency
- `Q_intercept` = controlled intercepted thermal power available to the cassette

This is analytical only.

It is useful because it forces every recovery claim to answer:

- how much thermal power is available?
- from what controlled source?
- at what assumed conversion efficiency?
- with what remaining waste heat burden?

---

## Locked Analytical Recovery Efficiencies for v0.1

For first-pass sizing in v0.1, the following efficiency assumptions are admissible as analytical cases only.

### Conservative system-like case
**20%**

Use:
- bounded, serious, non-hype first-pass estimate

### Strong TPV-target case
**27%**

Use:
- more ambitious but still bounded analytical target for a deliberate TPV-first cassette

### Stretch comparison case
Higher values may be discussed only as **comparison references** if clearly labeled as not assumed system performance for Max-01.

Max-01 must not be presented as already achieving stretch-case conversion.

---

## Example Recovery Cases

These examples are analytical only and assume a controlled intercepted stream already exists for protection reasons.

### Case A
Controlled intercepted thermal power:
**5 kW**

At:
**20%**
Estimated electric output:
**1.0 kWe**

At:
**27%**
Estimated electric output:
**1.35 kWe**

---

### Case B
Controlled intercepted thermal power:
**10 kW**

At:
**20%**
Estimated electric output:
**2.0 kWe**

At:
**27%**
Estimated electric output:
**2.7 kWe**

---

### Case C
Controlled intercepted thermal power:
**20 kW**

At:
**20%**
Estimated electric output:
**4.0 kWe**

At:
**27%**
Estimated electric output:
**5.4 kWe**

These cases are not promises.
They exist to show that a secondary recovery branch can be analytically meaningful if the intercepted stream is real and already justified on protective grounds.

---

## Residual Heat Rule

IR-06 does not eliminate the thermal problem.

If the cassette converts only a fraction of the intercepted stream, the remainder still exists as thermal burden that must be:

- rejected
- moved
- tolerated
- or bounded within the architecture

Therefore:

**Q_residual = Q_intercept − P_electric**

in equivalent power terms.

This means recovery never replaces thermal management.
It only extracts value from part of an already-managed stream.

---

## Example Residual Heat Cases

### Case A
Intercept:
**10 kW**

At:
**20%**
Electric output:
**2.0 kWe**

Residual thermal burden:
**8.0 kW**

### Case B
Intercept:
**10 kW**

At:
**27%**
Electric output:
**2.7 kWe**

Residual thermal burden:
**7.3 kW**

### Case C
Intercept:
**20 kW**

At:
**27%**
Electric output:
**5.4 kWe**

Residual thermal burden:
**14.6 kW**

These examples are the reason IR-06 must remain downstream and bounded.
The unrecovered thermal burden is still large.

---

## IR-06 Integration Rules

### Rule R1 — Downstream-only
IR-06 must sit downstream of the main protective function.

### Rule R2 — No harmful leak-feeding
The stack must not be allowed to leak extra heat inward just to improve recovery output.

### Rule R3 — Protection-first
If a change improves electric output but worsens TPS survivability, the change is rejected.

### Rule R4 — Modularity
IR-06 must remain removable without invalidating the passive or active protective logic.

### Rule R5 — Bounded source stream
The thermal source must be defined in terms of location, area, burden, and routing path.

### Rule R6 — Observability
HB-07 must remain able to tell whether IR-06 integration changed the backface burden in a harmful way.

### Rule R7 — Joint discipline
IR-06 routing must not undermine SJ-08 boundary control.

### Rule R8 — No architecture inversion
AR-05 may feed IR-06, but IR-06 may not drive AR-05 to exist where protection does not require it.

---

## IR-06 Failure Modes

The thermal-recovery branch becomes a liability if it falls into one of these failure modes.

### IF-01 — Leak-seeking design
The cassette is sized or placed in a way that rewards harmful inward heat leakage.

### IF-02 — Protection inversion
Design choices are made to improve recovery rather than survivability.

### IF-03 — Residual heat trap
Recovered power looks impressive on paper, but the unrecovered heat creates a worse downstream burden.

### IF-04 — Structural penalty
The cassette or its routing introduces thermal or mechanical penalties that destabilize the stack.

### IF-05 — Measurement corruption
Instrumentation no longer cleanly reveals whether the stack is improving or simply rerouting damage.

### IF-06 — Oversold electric output
The branch is described with optimistic power numbers disconnected from the actual intercepted thermal source.

### IF-07 — Complexity bloat
The cassette adds major integration burden without producing meaningful secondary value.

---

## Keep / Cut Decision Logic for IR-06

IR-06 stays only if all of the following remain true:

- a controlled intercepted thermal stream already exists
- the branch is clearly downstream
- the branch does not worsen TPS function
- the branch produces analytically meaningful secondary value
- the branch remains removable
- the branch stays compatible with validation and instrumentation

IR-06 gets cut if any of the following become true:

- it requires harmful leak-through
- it becomes the main reason for thermal intercept
- it worsens the structural or thermal stack
- it complicates the architecture more than it helps
- it encourages overclaiming
- it cannot be bounded in thermal accounting terms

---

## IR-06 Interaction with AR-05

AR-05 and IR-06 may coexist only under the following logic:

1. AR-05 exists because localized thermal protection requires it
2. AR-05 creates a bounded intercepted stream
3. that stream is still large enough and well controlled enough to justify a secondary cassette
4. IR-06 accepts only a bounded share of that stream
5. removing IR-06 leaves AR-05 still justified on thermal grounds alone

If those conditions are not met, the branches must remain decoupled or IR-06 must be removed.

---

## What Later Validation Must Prove

Future validation for IR-06 must eventually answer:

- what intercepted thermal power actually reached the cassette
- what fraction was converted to electricity
- what fraction remained residual heat
- whether protection-first logic remained intact
- whether the backface thermal burden worsened
- whether the cassette altered structural or boundary behavior
- whether the electrical output remained bounded and credible
- whether the branch stayed worth carrying

Until then, IR-06 remains an analytical branch only.

---

## What This Module Does Not Claim

This module does **not** claim:

- validated TPV performance in the Max-01 architecture
- validated TEG tail-stage performance
- validated power output under aerospace use conditions
- validated residual heat management
- validated structural integration
- validated mass efficiency
- validated reliability
- validated maintainability
- validated mission usefulness

---

## Relationship to Other Modules

This module depends on:
- `stack-architecture.md`
- `thermo-structural-budget.md`
- `hotspot-active-relief.md`

This module informs:
- `shield-health-monitoring.md`
- `risk-failure-register.md`
- `validation-campaign.md`
- later IR-06-specific test packages

---

## v0.1 Thermal Intercept Recovery Summary

IR-06 is a **secondary downstream thermal-recovery cassette**.

It exists only if:

- thermal interception is already justified for protection reasons
- the intercepted stream is controlled
- recovery remains subordinate to survival
- the cassette can be removed without collapsing the core architecture

The branch is allowed because it may recover useful power from an already-managed thermal stream.

It is forbidden from becoming the reason the thermal architecture exists.

That is the locked IR-06 logic for v0.1.
