# V9 Integrated Subscale Insert

## Stage Identity

**Stage:** V9  
**Name:** Integrated Subscale Insert  
**Program:** IX-HfTaZen-Shield  
**Reference configuration:** Max-01  
**Primary architecture under test:** integrated localized insert using the surviving passive stack and only the optional branches that earned continuation in V7 and V8  
**Evidence tier target if later executed:** E4-class integrated subscale evidence  
**Execution status:** planned / frozen for v0.1  
**Purpose:** determine whether the surviving architecture behaves like one coherent localized TPS insert rather than a collection of individually attractive subsystems

---

## Stage Purpose

V9 exists because every earlier stage is still only part of the truth.

The program may already have tested, screened, or bounded:

- HTZ-01 hot-face direction
- OX-02 oxidation-control logic
- SD-03 decoupling logic
- TC-04 carrier logic
- damaged passive behavior
- AR-05 active-relief value if it survived
- IR-06 recovery-cassette value if it survived

But none of that yet proves the actual thing the repo wants to be:

> a coherent localized extreme-heat TPS insert architecture

V9 is the first stage where the architecture must survive as an **integrated system**.

If the parts only make sense separately, Max-01 is not a real insert architecture yet.

---

## What V9 Is Testing

V9 is testing the integrated behavior of a subscale localized insert that includes:

### Required stack layers
- HTZ-01 Radiative UHTC Face
- OX-02 Oxidation-Control Transition
- SD-03 Strain-Decoupling Interlayer
- TC-04 Thermal Choke Carrier
- HB-07 Health-Monitoring Backplane
- SJ-08 Seal & Joint Management Ring

### Optional branches only if they earned continuation
- AR-05 Active Relief Branch
- IR-06 Thermal Intercept & Recovery Cassette

V9 is not a full-vehicle TPS stage.  
It is not flight hardware.  
It is not mission certification.

It is the first integrated localized insert truth stage.

---

## Why V9 Matters

The architecture has been deliberately built around the belief that the hard problem is not one layer.

The hard problem is the interaction between:

- heat
- oxidation
- mismatch
- support
- boundaries
- damage
- optional hotspot relief
- optional downstream recovery
- observability

V9 exists because an architecture can be locally clever and still globally incoherent.

This stage answers whether Max-01 survives that integration test.

---

## V9 Test Objective

The objective of V9 is to determine whether the surviving Max-01 architecture:

1. behaves as one coherent localized insert
2. remains bounded under integrated thermal and structural loading
3. preserves observability rather than becoming opaque when assembled
4. keeps seams and boundaries from dominating unexpectedly
5. integrates optional branches without allowing them to corrupt the core passive logic
6. justifies continued existence as a reference architecture rather than forcing a Max-02 redesign

---

## Primary Question

The primary V9 question is:

> When the surviving elements of Max-01 are assembled into a subscale localized insert, does the system still behave like a disciplined TPS architecture rather than a pile of separate good ideas?

---

## Secondary Questions

V9 also asks:

1. Does the integrated insert preserve the thermal logic established earlier?
2. Does the integrated insert preserve the structural logic established earlier?
3. Does SJ-08 keep the boundary from defeating the insert prematurely?
4. Does HB-07 remain useful and nonintrusive once the architecture is assembled?
5. If AR-05 survived, does it stay local and bounded in the integrated article?
6. If IR-06 survived, does it remain clearly downstream and secondary in the integrated article?
7. Does the insert fail in a way that remains interpretable?
8. Does the integrated result support keeping Max-01 as the canonical reference configuration?

---

## V9 Entry Rule

A V9 article is valid only if every included subsystem has already earned its place.

That means:

### Required
- passive stack survivor from V6

### Optional only if explicitly earned
- AR-05 survivor from V7
- IR-06 survivor from V8

If AR-05 or IR-06 did not survive their keep / cut stages, they do not enter V9.

V9 is not allowed to resurrect failed optional branches for the sake of completeness.

---

## Integrated Insert Philosophy

The V9 philosophy is:

- assemble only what has earned integration
- preserve the localized nature of the insert
- include boundaries honestly
- include monitoring honestly
- keep optional branches subordinate
- compare integrated behavior against the architecture’s promises
- accept that integration may reveal contradictions earlier stages could not expose

V9 is not about building the most complex article possible.

It is about building the **minimum honest integrated insert**.

---

## Required Integrated Article Classes

### V9-I1
**Integrated passive insert baseline**

Includes:
- HTZ-01
- OX-02
- SD-03
- TC-04
- HB-07
- SJ-08

Intent:
- first integrated truth article for the baseline Max-01 stack

---

### V9-I2
**Integrated passive insert with earned AR-05 branch**
only if V7 succeeded

Includes:
- V9-I1 baseline
- AR-05

Intent:
- determine whether the kept active-relief branch remains coherent in integrated form

---

### V9-I3
**Integrated passive insert with earned IR-06 branch**
only if V8 succeeded

Includes:
- V9-I1 baseline
- IR-06

Intent:
- determine whether the kept recovery cassette remains coherent in integrated form

---

### V9-I4
**Integrated insert with both earned AR-05 and IR-06 branches**
only if both survived and only if IR-06 depends on a controlled intercepted stream that remains justified

Includes:
- V9-I1 baseline
- AR-05
- IR-06

Intent:
- test whether the fully kept architecture still behaves coherently when all earned branches are present

This article is optional and should not be built unless both optional branches truly earned continuation.

---

## Optional comparison classes

### V9-B1
**Simplified integrated insert baseline**
if a simpler passive route remained competitive through V6

Intent:
- determine whether full Max-01 complexity is still earning itself at integrated scale

### V9-R1
**Boundary-stressed integrated article**
if capacity allows

Intent:
- expose whether the boundary ring remains the dominant integrated weakness

### V9-R2
**Damaged integrated insert**
if capacity allows and if staged progression supports it

Intent:
- connect V6 damaged-state logic to the integrated architecture

Reserve integrated articles are allowed only if they sharpen the truth instead of turning V9 into a feature parade.

---

## Article Naming Rule

The repo may refer to V9 integrated articles using the following identifiers:

- V9-I1
- V9-I2
- V9-I3
- V9-I4
- V9-B1
- V9-R1
- V9-R2

Detailed geometry, instrumentation layout, branch routing, and fixture specifics may live in later support artifacts, but the stage must remain readable through stable IDs.

---

## Integrated Geometry Rule

The V9 article must include a real localized insert logic, not just a stacked slab.

That means the integrated article should preserve as many of the following truths as possible:

- localized insert boundaries
- edge and seam behavior
- support-path definition
- boundary ring function
- monitoring-path reality
- optional-branch locality if present

If the article has no meaningful insert boundary behavior, it is not a valid V9 representation of Max-01.

---

## What V9 Is Trying to Prove

V9 is trying to prove only the following:

1. The surviving Max-01 architecture remains coherent when integrated.
2. The required layers still earn their places when assembled together.
3. Boundaries and seams do not immediately erase the value of the central stack.
4. HB-07 remains useful without becoming intrusive.
5. Optional branches, if kept, remain clearly subordinate to the passive-first architecture.
6. The integrated insert behaves in a way that is bounded and interpretable enough to justify keeping Max-01 alive.

---

## What V9 Is Trying to Disprove

V9 is trying to disprove any of the following bad outcomes:

1. The architecture only works as isolated subsystems.
2. Integration reveals contradictions between thermal, structural, and boundary logic.
3. HB-07 becomes intrusive or meaningless in the integrated article.
4. SJ-08 or the boundary geometry dominates so strongly that the center-stack story becomes misleading.
5. AR-05 or IR-06 corrupts the integrated insert even though it looked acceptable alone.
6. Max-01 complexity no longer earns itself once the parts are assembled.

---

## Planned Observation Set

At minimum, V9 should eventually capture the following.

### O1 — Integrated article identity
- article ID
- included layer set
- optional-branch inclusion state
- geometry ID
- boundary configuration ID
- instrumentation configuration ID

### O2 — Baseline condition
- pre-test imagery
- mass
- geometry / profile notes
- boundary condition
- sensor / monitoring readiness
- optional-branch readiness if present

### O3 — During-test thermal observations where feasible
- surface thermal trend
- backface thermal trend
- boundary thermal trend
- interface-adjacent thermal trend if instrumented
- optional-branch thermal behavior if present

### O4 — During-test structural / integrity observations where feasible
- crack initiation
- boundary motion or distress
- local delamination cues
- support-path distress
- branch-adjacent instability if present

### O5 — Monitoring observations
- whether HB-07 remained useful
- whether measurements revealed integrated behavior cleanly
- whether monitoring introduced penalty or confusion

### O6 — Post-test integrated condition
- overall article integrity
- center versus boundary damage pattern
- layer interaction evidence
- branch interaction evidence
- profile or geometry change
- whether failure was bounded and interpretable

### O7 — Comparative ranking notes
- integrated baseline versus simplified baseline if present
- integrated passive-only versus branch-enabled variants if present
- bounded / unstable / contradictory integrated behavior classification

The goal is to reveal whether the integrated insert is still the same architecture the repo thinks it is.

---

## Minimum Evaluation Questions per Integrated Article

Each integrated article should be judged against the following questions.

### Q1
Did the article remain grossly coherent as an integrated insert?

### Q2
Did the required layers still appear to earn their places when assembled?

### Q3
Did the boundary and seam behavior remain within the architecture’s expected risk story?

### Q4
Did HB-07 remain useful and nonintrusive?

### Q5
If optional branches were present, did they remain subordinate rather than dominant?

### Q6
Was the integrated behavior still interpretable rather than chaotic?

### Q7
Does this article support keeping Max-01 as the canonical reference configuration?

If the answer set is mostly no, Max-01 should be narrowed or revised.

---

## Stage-Level Pass Conditions

V9 passes only if all of the following are true:

1. At least one integrated article remains grossly coherent.
2. The required stack layers still earn their places in integrated form.
3. Boundary and seam behavior do not immediately invalidate the insert architecture.
4. HB-07 remains helpful rather than harmful.
5. Optional branches, if present, remain clearly subordinate and bounded.
6. The repo can explain the integrated behavior honestly enough to preserve Max-01.

---

## Stage-Level Fail Conditions

V9 fails if any of the following occur:

1. The integrated article reveals fundamental contradiction between subsystems.
2. The boundary ring or seam behavior dominates so completely that the architecture must be reconceived.
3. HB-07 becomes intrusive or unhelpful in integrated form.
4. Optional branches destabilize the insert once integrated.
5. The simplified integrated baseline performs as well or better in a way that undermines full Max-01 complexity.
6. The integrated behavior is too chaotic to support coherent interpretation.

If V9 fails, Max-01 should not be preserved unchanged.

---

## V9 Keep / Cut Logic

### Keep Max-01 as the canonical reference if:
- at least one integrated article remains coherent
- the full required stack still earns itself
- boundaries remain serious but not disqualifying
- optional branches, if kept, remain subordinate and honest

### Downgrade or narrow Max-01 if:
- the integrated insert remains promising, but only under tighter boundaries than originally assumed
- one required subsystem now looks overcomplicated
- the optional branches survive only in narrower forms than expected

### Replace Max-01 with a revised reference configuration if:
- the integrated result reveals a deeper architectural contradiction
- simplified integrated logic consistently looks more credible
- the current version of Max-01 no longer deserves to remain the canonical reference

---

## Controls and Baselines

V9 must not run without the following comparison posture:

- one integrated passive baseline
- one simplified integrated comparison if it remains relevant
- branch-enabled variants only if the branches truly survived earlier keep / cut stages
- measurements that preserve center versus boundary interpretation
- explicit architecture-level interpretation, not just survival language

Without those controls, V9 becomes a complexity showcase instead of an integrated truth stage.

---

## V9 Risk Focus

The main risks V9 is trying to expose are:

- subsystem contradiction
- seam / boundary dominance
- monitoring integration penalty
- optional-branch integration corruption
- full-stack complexity that no longer earns itself
- inability to interpret integrated behavior cleanly

If V9 does not expose those risks, it is not doing its job.

---

## What V9 Does Not Prove

Even if V9 succeeds, it does **not** prove:

- flight readiness
- mission readiness
- production readiness
- operational reuse
- certification readiness
- superiority over existing validated aerospace TPS

V9 is the integrated subscale truth stage only.

---

## Data Package Required from V9

When V9 is eventually executed, the stage should produce a data package that includes:

- integrated article roster
- layer and branch inclusion states
- geometry and boundary definitions
- pre/post imagery
- thermal observations
- structural and boundary observations
- monitoring observations
- comparative ranking summary
- keep / narrow / replace recommendation for Max-01

If that package does not exist, V9 has not really been completed.

---

## V9 Exit Decisions

At the end of V9, only the following decisions are valid.

### D1 — Keep Max-01 as canonical
Use when the integrated article remains coherent and the full architecture still earns itself.

### D2 — Narrow Max-01
Use when the integrated result is promising but only within tighter limits.

### D3 — Remove or narrow optional branches
Use when integration shows AR-05 or IR-06 became too costly or invasive.

### D4 — Simplify required stack logic
Use when one required subsystem no longer earns its place in integrated form.

### D5 — Branch to Max-02
Use when the integrated result reveals a deeper architectural truth that the current Max-01 cannot honestly absorb.

---

## Relationship to Other Modules

This stage depends on:
- `reference-configs/max-01.md`
- all earlier validation-stage survivor logic
- `modules/shield-health-monitoring.md`
- `modules/risk-failure-register.md`

This stage informs:
- future reference-configuration decisions
- future architecture narrowing
- future external presentation discipline

---

## V9 Summary

V9 is the stage where IX-HfTaZen-Shield stops being a set of disciplined modules and attempts to become a real integrated localized insert.

If the integrated article cannot remain coherent, then Max-01 must change rather than be protected by optimism.
