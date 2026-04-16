# V7 Local Active-Relief Demonstrator

## Stage Identity

**Stage:** V7  
**Name:** Local Active-Relief Demonstrator  
**Program:** IX-HfTaZen-Shield  
**Reference configuration:** Max-01  
**Primary architecture branch under test:** AR-05 Active Relief Branch  
**Evidence tier target if later executed:** bounded E3-to-E4 bridge evidence depending on demonstrator fidelity  
**Execution status:** planned / frozen for v0.1  
**Purpose:** determine whether a local-only active-relief branch can reduce severe hotspot burden without creating worse thermal, oxidation, structural, or integration penalties than the hotspot itself

---

## Stage Purpose

V7 exists because the repo has already made a disciplined promise:

- the architecture is passive-first
- AR-05 is optional
- AR-05 is local-only
- AR-05 must earn its place
- AR-05 must never become the reason the architecture works

That means AR-05 does not get to enter the stack just because it sounds advanced.

V7 is the stage where IX-HfTaZen-Shield forces AR-05 to answer the hard question:

> Can a bounded local active-relief concept actually reduce a severe local hotspot burden without destabilizing the rest of the architecture?

If the answer is no, AR-05 gets cut.

---

## What V7 Is Testing

V7 is testing whether a **local severe-hotspot relief branch** can be integrated honestly.

The stage focuses on:

- the best surviving passive stack context from V6
- a localized severe hotspot case that analytically justifies AR-05
- one or more bounded AR-05 implementations
- the thermal, structural, and oxidation consequences of adding local active relief

V7 is not a broad cooling stage.  
It is not a whole-vehicle stage.  
It is not a recovery stage first.

It is a hotspot-relief truth stage.

---

## Why V7 Matters

The repo already froze the thermal posture:

- Band A: 500–800 W/cm²
- Band B: 800–1000 W/cm²
- Band C: 1000–1500 W/cm² local only

V7 exists because Band C was never promised as an easy passive-only region.

Instead, the repo said:

- Band C is local-only
- assistance may be justified there
- assistance must remain bounded
- assistance must not quietly become whole-architecture dependence

V7 is the stage that decides whether that statement was disciplined engineering or wishful thinking.

---

## V7 Test Objective

The objective of V7 is to determine whether one or more AR-05 concept classes can:

1. reduce a clearly defined local hotspot burden
2. keep that relief local
3. avoid introducing worse oxidation, interface, or structural damage
4. avoid corrupting the passive-first architecture
5. justify continuation toward integrated insert logic

---

## Primary Question

The primary V7 question is:

> Does a bounded AR-05 concept reduce the severe local hotspot burden enough to matter, without creating worse total architecture risk?

---

## Secondary Questions

V7 also asks:

1. Is porous-UHTC local transpiration-style relief actually more credible than a heat-pipe local intercept in this architecture?
2. Does local burden reduction stay local, or does it merely move the thermal problem?
3. Does the active branch open a worse oxidation path than the hotspot it is meant to relieve?
4. Does AR-05 create a new structural weak point at the relief site or its interfaces?
5. Does the downstream burden become more manageable or more confusing?
6. Does AR-05 still look worth carrying once the passive stack context is considered honestly?

---

## Candidate Set for V7

### Required demonstrator families

#### V7-B0
**Passive severe-hotspot baseline**

Intent:
- preserve a no-AR-05 comparison against the same local severe hotspot case

#### V7-A1
**Porous-UHTC local transpiration-style relief demonstrator**

Intent:
- primary AR-05 concept class
- direct local severe-hotspot burden reduction test

#### V7-A2
**Refractory heat-pipe local intercept demonstrator**

Intent:
- secondary AR-05 concept class
- local heat removal / redistribution comparison against V7-A1

---

### Optional demonstrator families

#### V7-R1
**Simplified local heat-spreading branch**

Intent:
- reserve concept if a more bounded local heat redistribution comparison is needed

#### V7-R2
**Alternate implementation of V7-A1 or V7-A2**

Intent:
- avoid overcommitting to one arbitrary implementation inside a concept class

Reserve demonstrators are allowed only if they sharpen the branch decision instead of diluting it.

---

## Candidate Naming Rule

The repo may refer to V7 demonstrators using the following identifiers:

- V7-B0
- V7-A1
- V7-A2
- V7-R1
- V7-R2

Detailed routing, porosity, geometry, and local-zone definitions may live in later support artifacts, but the stage must remain readable through stable IDs.

---

## Demonstrator Philosophy

The V7 philosophy is:

- define the hotspot clearly
- define the local target burden clearly
- define the intercept burden clearly
- compare against a passive severe-hotspot baseline
- force the branch to reveal total cost, not just local peak benefit

V7 is not about whether AR-05 can look impressive at the hotspot center for one photo.

It is about whether AR-05 improves the architecture **overall**.

---

## Hotspot Definition Rule

AR-05 may only be tested in a hotspot case that satisfies all of the following:

1. the hotspot is local rather than broad-area
2. the local burden is severe enough to justify AR-05 analytically
3. the passive baseline shows thin margin or failure tendency
4. the local thermal job of AR-05 can be expressed as a burden reduction target
5. the demonstrator can be compared against a passive baseline honestly

If these conditions are not met, the V7 test case is invalid.

---

## Local Burden-Reduction Rule

The AR-05 demonstrator must define:

- `q_hotspot`
- `q_target`
- `Δq = q_hotspot − q_target`
- local effective area `A`
- expected intercept burden `Q_intercept = Δq × A`

Without those definitions, the stage is not a real engineering comparison.

---

## What V7 Is Trying to Prove

V7 is trying to prove only the following:

1. At least one AR-05 concept class can reduce a severe local hotspot burden measurably.
2. That reduction remains bounded and local.
3. The total architecture penalty is lower than the hotspot penalty it removes.
4. The active branch remains compatible with the passive stack.
5. The repo can explain why one active concept deserves continuation or why both should be cut.

---

## What V7 Is Trying to Disprove

V7 is trying to disprove any of the following bad outcomes:

1. AR-05 is complexity theater.
2. AR-05 reduces the center hotspot but worsens the stack elsewhere.
3. AR-05 opens a worse oxidation path than the baseline.
4. AR-05 introduces a new structural weakness at the relief location.
5. AR-05 makes the architecture more dependent on active systems than the mission envelope allows.
6. AR-05 exists mainly to feed IR-06 rather than to protect the stack.

---

## Planned Observation Set

At minimum, V7 should eventually capture the following.

### O1 — Demonstrator identity
- demonstrator ID
- concept class ID
- hotspot condition ID
- passive baseline reference ID

### O2 — Local thermal definition
- hotspot location
- hotspot burden estimate
- target burden after relief
- estimated intercept burden
- affected area definition

### O3 — During-test thermal observations where feasible
- hotspot temperature trend
- downstream or adjacent thermal trend
- backface trend
- evidence of shifted burden

### O4 — During-test structural / integrity observations where feasible
- local cracking
- local deformation
- interface distress
- support-path change
- edge or boundary penalty if relevant

### O5 — Oxidation / degradation observations where feasible
- local exposed-face degradation
- new local distress introduced by the active branch
- branch-adjacent damage signatures

### O6 — Comparative ranking notes
- better / similar / worse than passive baseline
- bounded / unstable / unacceptable relief behavior
- architecture-helping / architecture-harming classification

The goal is to reveal whether AR-05 is a real solution or a new problem.

---

## Minimum Evaluation Questions per Demonstrator

Each V7 demonstrator should be judged against the following questions.

### Q1
Did the demonstrator reduce the local hotspot burden measurably?

### Q2
Did the reduction remain local and bounded?

### Q3
Did the branch avoid creating a worse oxidation path?

### Q4
Did the branch avoid creating a worse structural weakness?

### Q5
Did the branch avoid simply relocating the failure to another part of the stack?

### Q6
Did the branch preserve the passive-first logic of Max-01?

### Q7
Is this concept class worth carrying forward?

If the answer set is mostly no, that concept class should be cut.

---

## Stage-Level Pass Conditions

V7 passes only if all of the following are true:

1. At least one AR-05 concept class reduces local severe-hotspot burden meaningfully.
2. That concept class remains bounded and local.
3. The architecture penalty of the branch is smaller than the thermal benefit it provides.
4. The branch remains compatible with the passive-first logic of Max-01.
5. The repo can explain clearly why the surviving branch continues.

---

## Stage-Level Fail Conditions

V7 fails if any of the following occur:

1. No AR-05 concept class provides meaningful local relief.
2. Relief is achieved only by moving the failure somewhere worse.
3. The active branch creates a more dangerous oxidation or structural path than the baseline hotspot.
4. The branch begins to look like a hidden architecture dependency.
5. The stage cannot distinguish true benefit from complexity-driven noise.

If V7 fails, AR-05 must be cut or radically narrowed before integrated-stage use.

---

## V7 Keep / Cut Logic

### Keep AR-05 if:
- at least one concept class reduces local burden meaningfully
- the benefit stays local
- the total architecture remains healthier with the branch than without it
- the branch remains clearly optional and bounded

### Downgrade AR-05 if:
- the branch helps, but only in a narrower hotspot definition than originally assumed
- the branch remains interesting but carries stronger penalties than hoped
- only one concept class survives with heavy caveats

### Cut AR-05 if:
- the branch creates worse total risk than the hotspot it was meant to solve
- no concept class remains bounded and honest
- the branch only survives by becoming broader or more central than Max-01 allows

---

## Controls and Baselines

V7 must not run without the following comparison posture:

- one passive severe-hotspot baseline
- at least one primary AR-05 concept class
- at least one alternate AR-05 concept class
- defined hotspot burden and target burden
- thermal and structural observations tied together
- architecture-wide comparison, not hotspot-center-only comparison

Without those controls, V7 becomes a gadget demo rather than a truth stage.

---

## V7 Risk Focus

The main risks V7 is trying to expose are:

- active-branch self-harm
- oxidation-access penalty
- local structural weakness creation
- heat relocation failure
- hidden dependency creep
- active complexity that outgrows its thermal job

If V7 does not expose those risks, it is not doing its job.

---

## What V7 Does Not Prove

Even if V7 succeeds, it does **not** prove:

- full integrated insert maturity
- IR-06 value
- final seam-system validity
- final reuse capability
- flight relevance
- operational maintainability

V7 is the active-relief truth stage only.

---

## Data Package Required from V7

When V7 is eventually executed, the stage should produce a data package that includes:

- demonstrator roster
- hotspot-definition logic
- intercept-burden logic
- pre/post imagery
- thermal observations
- structural / degradation observations
- comparative ranking summary
- keep / cut recommendation for AR-05

If that package does not exist, V7 has not really been completed.

---

## V7 Exit Decisions

At the end of V7, only the following decisions are valid.

### D1 — Keep AR-05 as an optional bounded branch
Use when at least one concept class survives honestly.

### D2 — Narrow AR-05 to a tighter hotspot-only use case
Use when the branch helps, but only in a smaller operating region than first hoped.

### D3 — Replace the preferred AR-05 concept class
Use when one concept class fails and another proves more credible.

### D4 — Cut AR-05 from Max-01
Use when the branch does not earn its place honestly.

### D5 — Branch to revised reference configuration
Use when V7 reveals that the architecture really wants a different active-relief philosophy than Max-01 permits.

---

## Relationship to Other Modules

This stage depends on:
- `reference-configs/max-01.md`
- `modules/hotspot-active-relief.md`
- `modules/risk-failure-register.md`
- the passive survivor logic from V6

This stage informs:
- V8 recovery-sidecar planning
- V9 integrated insert planning
- future AR-05 keep / cut decisions
- future hotspot-use-case narrowing

---

## V7 Summary

V7 is the stage where IX-HfTaZen-Shield forces its active-relief ambition to justify itself.

If AR-05 cannot reduce a severe local hotspot without creating worse total architecture harm, it does not deserve to remain in Max-01.
