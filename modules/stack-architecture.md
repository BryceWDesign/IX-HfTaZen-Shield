# Stack Architecture

## Module Purpose

This module defines the **canonical IX-HfTaZen-Shield stack architecture** for v0.1.

The purpose of this module is to freeze the layer order, the role of each layer, the interface logic between layers, and the conditions under which optional branches are allowed.

This module does **not** claim that the architecture is validated.  
It defines the baseline system structure that later screening, thermal reasoning, and validation planning will use.

---

## Architecture Rule

IX-HfTaZen-Shield is not a single-material concept.

It is a **layered localized TPS insert architecture** built around the following ideas:

1. the exposed face must survive the worst local thermal environment
2. oxidation must be managed as a separate problem from nominal peak temperature
3. thermo-structural mismatch must be treated as a layer-stack problem, not just a material property problem
4. heat transmission into deeper structure must be throttled
5. active relief is permitted only where passive margin becomes too thin
6. thermal energy recovery is optional and must sit downstream of the protective function
7. observability is part of the architecture, not an afterthought

---

## Canonical Layer Order

The v0.1 canonical layer order is locked as follows:

1. **HTZ-01 Radiative UHTC Face**
2. **OX-02 Oxidation-Control Transition**
3. **SD-03 Strain-Decoupling Interlayer**
4. **TC-04 Thermal Choke Carrier**
5. **AR-05 Active Relief Branch** *(optional, local only)*
6. **IR-06 Thermal Intercept & Recovery Cassette** *(optional, downstream only)*
7. **HB-07 Health-Monitoring Backplane**
8. **SJ-08 Seal & Joint Management Ring**

This order is the baseline reference architecture for `Max-01`.

---

## Layer-by-Layer Definition

## 1. HTZ-01 Radiative UHTC Face

### Role
HTZ-01 is the primary exposed surface of the localized insert.

### Core purpose
- take the direct thermal assault
- reradiate as aggressively as practical
- resist oxidation better than simpler UHTC directions
- provide the first thermal and chemical defense boundary

### Design posture
HTZ-01 is treated as:
- high-temperature capable
- oxidation-limited rather than melting-point-limited in real oxidizing use
- segmented rather than assumed monolithic over large areas

### Locked behavior rule
HTZ-01 must not be treated as a miracle layer that solves:
- oxidation
- stress mismatch
- backface heating
- attachment survivability
- joint durability
on its own.

---

## 2. OX-02 Oxidation-Control Transition

### Role
OX-02 sits directly beneath HTZ-01 as the oxidation-control and chemistry-transition layer.

### Core purpose
- reduce oxygen ingress toward deeper interfaces
- manage the chemistry transition between the exposed face and deeper structure
- support more stable interfacial behavior under oxidizing heat exposure
- reduce the chance that the hot-face/substructure interface becomes the first failure site

### Design posture
OX-02 is not the primary exposed truth layer for the most severe hot-face condition.

It exists because:
- peak hot-face chemistry and oxidation-control chemistry do not have to be the same thing
- a buried transition can help the stack more than forcing one layer to do everything badly

### Locked behavior rule
OX-02 must improve survivability without becoming the dominant thermal bottleneck or a weak brittle interface.

---

## 3. SD-03 Strain-Decoupling Interlayer

### Role
SD-03 is the first dedicated thermo-structural protection layer inside the stack.

### Core purpose
- reduce stress transfer caused by differential thermal expansion
- lower crack-driving mismatch stress
- reduce interface restraint severity
- improve survivability of segmented inserts under thermal cycling and handling

### Design posture
SD-03 is a functional requirement, not a decorative one.

The stack assumes that:
- the hot face expands differently than deeper structure
- the layer stack must tolerate restraint and gradient-driven stress
- decoupling is a system requirement for credibility

### Locked behavior rule
If the architecture only works when the hot face is rigidly hard-bonded to the deeper carrier, the architecture is considered immature and structurally suspect.

---

## 4. TC-04 Thermal Choke Carrier

### Role
TC-04 provides structural support and thermal-flow moderation beneath the decoupling layer.

### Core purpose
- carry insert-level structural loads
- support the segmented hot-face architecture
- reduce heat transfer into deeper protected structure
- provide a stable geometry for local integration

### Design posture
TC-04 must balance:
- thermal conservatism
- structural support
- compatibility with SD-03
- compatibility with local instrumentation

### Locked behavior rule
TC-04 is not allowed to become a hidden thermal short that defeats the purpose of the upper layers.

---

## 5. AR-05 Active Relief Branch *(optional, local only)*

### Role
AR-05 is the optional local-only branch used when the passive stack does not retain credible margin in the highest local hotspot band.

### Core purpose
- reduce peak local thermal burden
- intercept or redistribute heat only in the most severe zones
- prevent passive hot-face loading from crossing the credible oxidizing survivability cliff

### Allowed forms
AR-05 may be treated as one of the following concept classes:
- porous-UHTC transpiration-like relief
- refractory heat-pipe local intercept
- tightly bounded local heat-spreading branch
- other strictly local thermal-intercept concepts that do not transform the whole architecture into broad active cooling

### Locked behavior rule
AR-05 is permitted only when all of the following are true:
- the location is a localized hotspot
- passive margin is analytically too thin
- the active branch improves survivability without creating broader system instability
- the branch remains removable without invalidating the core passive stack concept

### Disallowed behavior
AR-05 must not become:
- broad-area cooling
- the default answer everywhere
- proof that the passive stack is good enough when it is not
- a substitute for proper hot-face and interface design

---

## 6. IR-06 Thermal Intercept & Recovery Cassette *(optional, downstream only)*

### Role
IR-06 is an optional downstream subsystem that accepts a **controlled intercepted heat stream** and attempts secondary energy conversion.

### Core purpose
- recover a bounded share of thermal energy that has already been intentionally intercepted
- support self-power for sensing, logging, or bounded subsystem loads
- explore multifunctional value without compromising the primary TPS role

### Design posture
IR-06 is always subordinate to the protective function of the stack.

This means:
- the stack is not allowed to leak extra heat on purpose just to feed IR-06
- IR-06 must operate on controlled thermal routing, not uncontrolled interior heating
- removing IR-06 must not collapse the core TPS concept

### Locked behavior rule
IR-06 must never be described as the main heat-relief mechanism.

---

## 7. HB-07 Health-Monitoring Backplane

### Role
HB-07 is the instrumentation and awareness layer behind the thermal architecture.

### Core purpose
- track backface temperature
- support interface thermal awareness
- support strain or displacement observability
- log anomalies, excursions, and degradation indicators
- support comparison between expected and observed behavior

### Design posture
HB-07 exists because:
- a modern high-risk TPS concept should not be blind
- measurement helps separate real progress from self-deception
- localized inserts are especially vulnerable at boundaries and interfaces

### Locked behavior rule
HB-07 must not require the thermal stack to be weakened just to become observable.

---

## 8. SJ-08 Seal & Joint Management Ring

### Role
SJ-08 is the architecture around the insert boundary.

### Core purpose
- manage seams, edges, and local interface discontinuities
- reduce the chance that joints fail before the hot face does
- bound heat, stress, and damage behavior at insert edges

### Design posture
The architecture assumes that insert boundaries are high-risk zones.

That means the design must explicitly consider:
- seam geometry
- edge chipping
- local restraint
- differential movement
- oxidation access paths
- damage-growth pathways from the boundary inward

### Locked behavior rule
If joints are left undefined until late in development, the architecture is considered incomplete.

---

## Baseline Thermal Path Logic

The canonical thermal logic of the stack is:

1. HTZ-01 accepts and reradiates the direct heat load
2. OX-02 helps preserve interface chemistry and oxidation resistance
3. SD-03 reduces structural penalty from thermal mismatch
4. TC-04 slows and manages deeper heat penetration while carrying support duties
5. AR-05 optionally intercepts peak local heat only where necessary
6. IR-06 optionally accepts part of a controlled intercepted heat stream for secondary conversion
7. HB-07 observes what survives the upper stack
8. SJ-08 protects the boundary from becoming the dominant failure path

This logic must remain intact across all `Max-01` analyses.

---

## Interface Rules

The stack is only credible if the interfaces are credible.

The following interface rules are locked for v0.1.

### Rule I1 — HTZ-01 to OX-02
The hot face and oxidation-control transition must be chemically and mechanically compatible enough that the interface does not become an obvious sacrificial crack plane.

### Rule I2 — OX-02 to SD-03
The oxidation-control layer must not defeat the purpose of the strain-decoupling layer by transmitting excessive brittle constraint.

### Rule I3 — SD-03 to TC-04
The decoupling layer must reduce thermal-mismatch stress without allowing uncontrolled instability, collapse, or loss of support.

### Rule I4 — AR-05 integration
If AR-05 exists, it must integrate in a way that does not create a worse structural weakness than the hotspot it is trying to save.

### Rule I5 — IR-06 integration
IR-06 must sit downstream of protective function and must not pull the thermal architecture toward harmful heat leakage.

### Rule I6 — HB-07 integration
Instrumentation routing and sensing placement must avoid creating obvious thermal shorts or crack initiators.

### Rule I7 — SJ-08 continuity
The joint and seal ring must be treated as part of the stack, not as cosmetic trim around it.

---

## Canonical Zone Logic

The stack supports three severity zones.

## Zone A — Baseline Passive Local Zone
Target band:
**500–800 W/cm²**

Allowed architecture:
- HTZ-01
- OX-02
- SD-03
- TC-04
- HB-07
- SJ-08

Active relief:
- not required by default

Energy recovery:
- optional only if downstream thermal routing remains controlled

---

## Zone B — Stretched Passive Local Zone
Target band:
**800–1000 W/cm²**

Allowed architecture:
- same as Zone A
- stronger emphasis on interface survivability and thermal choke behavior

Active relief:
- still optional
- may be deferred if analytical margin remains credible

Energy recovery:
- still secondary and optional

---

## Zone C — Assisted Local Hotspot Zone
Target band:
**1000–1500 W/cm²**

Allowed architecture:
- HTZ-01
- OX-02
- SD-03
- TC-04
- AR-05
- optional IR-06
- HB-07
- SJ-08

Active relief:
- allowed and likely necessary in this band

Energy recovery:
- permitted only from a controlled intercepted stream
- cannot justify weaker thermal protection upstream

---

## Architecture Dependencies

The stack has the following dependency logic.

### Dependency D1
HTZ-01 depends on OX-02 and SD-03 to remain part of a credible reusable insert architecture.

### Dependency D2
OX-02 depends on both chemical logic and interface logic.  
It cannot be chosen solely for oxidation behavior while ignoring brittleness or mismatch penalties.

### Dependency D3
SD-03 depends on TC-04 geometry and stiffness behavior.  
A decoupling layer is meaningless without a compatible deeper support architecture.

### Dependency D4
AR-05 depends on a defined hotspot criterion.  
If no hotspot criterion exists, AR-05 should not be added.

### Dependency D5
IR-06 depends on a bounded thermal intercept path.  
If no bounded intercept path exists, IR-06 should not exist in the configuration.

### Dependency D6
HB-07 depends on instrumentation survivability logic.  
Measurement intent alone is not enough.

### Dependency D7
SJ-08 depends on segmentation geometry, local movement expectations, and edge damage logic.

---

## Architectural Failure Modes This Stack Is Meant to Resist

The stack exists to reduce risk from the following major failure classes:

- hot-face oxidation-driven degradation
- hot-face cracking or spall initiation
- brittle interface failure beneath the hot face
- thermal expansion mismatch
- support-layer thermal shorting
- attachment or boundary failure
- excessive backface heat leakage
- uncontrolled hotspot escalation
- blind degradation with no measurement trail
- overcomplication through unnecessary active features

This does not mean the stack has solved these problems.  
It means the architecture was deliberately shaped around them.

---

## Excluded Architecture Patterns

The following architecture patterns are excluded from v0.1.

### Exclusion X1 — Monolithic miracle slab
A single slab that is expected to solve all thermal, chemical, structural, and interface problems by material choice alone.

### Exclusion X2 — Broad active cooling shell
A design that requires wide-area active cooling to remain credible.

### Exclusion X3 — Energy-first thermal stack
A design that lets energy recovery dictate the thermal stack instead of keeping recovery downstream and secondary.

### Exclusion X4 — Blind TPS
A design with no measurement or health-awareness path.

### Exclusion X5 — Undefined joints
A design that describes the insert face in detail but treats seams and boundaries as someone else’s problem.

### Exclusion X6 — Radiation-muddied baseline
A design that mixes radiation shielding into the baseline stack before the core localized TPS problem is coherent.

---

## `Max-01` Baseline Stack Summary

### Required layers
- HTZ-01 Radiative UHTC Face
- OX-02 Oxidation-Control Transition
- SD-03 Strain-Decoupling Interlayer
- TC-04 Thermal Choke Carrier
- HB-07 Health-Monitoring Backplane
- SJ-08 Seal & Joint Management Ring

### Optional layers
- AR-05 Active Relief Branch
- IR-06 Thermal Intercept & Recovery Cassette

### Baseline philosophy
- passive-first
- active local only
- energy recovery secondary only
- instrumented by design
- segmented and interface-aware
- localized insert, not full-body TPS

---

## Success Condition for This Module

This module is successful if it forces all later work to answer:

- What exact layer is responsible for this function?
- Is the function passive, optional active, or optional downstream?
- Does the layer order still make sense thermally and structurally?
- Does the design still behave like a localized insert architecture?
- Are joints and interfaces treated as part of the system?
- Has any optional feature started to dominate the design improperly?

If those questions cannot be answered, the architecture is not locked tightly enough.

---

## v0.1 Stack Architecture Summary

IX-HfTaZen-Shield v0.1 is locked as a **segmented localized TPS insert architecture** with:

- a radiative UHTC hot face
- an oxidation-control transition
- a strain-decoupling interlayer
- a thermal choke carrier
- optional local-only active hotspot relief
- optional downstream thermal intercept and recovery
- a health-monitoring backplane
- a seal and joint management ring

This is the canonical stack for `Max-01`.
