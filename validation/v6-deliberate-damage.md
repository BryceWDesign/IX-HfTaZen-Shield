# V6 Deliberate Damage Coupons

## Stage Identity

**Stage:** V6  
**Name:** Deliberate Damage Coupons  
**Program:** IX-HfTaZen-Shield  
**Reference configuration:** Max-01  
**Primary architecture layers under test:** surviving V5 passive stack family, with damage introduced before or between severe exposures  
**Evidence tier target if later executed:** E3-class coupon evidence  
**Execution status:** planned / frozen for v0.1  
**Purpose:** determine whether the surviving passive stack fails in a bounded, interpretable way when realistic local damage is introduced

---

## Stage Purpose

V6 exists because the earlier stages can only tell part of the truth.

A stack can:

- survive chemistry screening
- survive transition-layer screening
- survive cycling
- survive mismatch-driven loading
- survive severe high-heat exposure

and still fail too easily once it is no longer perfect.

V6 is the stage where IX-HfTaZen-Shield deliberately stops pretending the hardware is pristine.

It asks the next hard question:

> Does the surviving passive stack degrade in a bounded, observable, architecture-consistent way once realistic local damage is introduced?

This stage is required because the repo is not allowed to depend on perfect geometry, perfect edges, perfect seams, or perfect handling.

---

## What V6 Is Testing

V6 is testing the **damaged-state honesty** of the best surviving passive stack from V5.

The stage focuses on damage introduced into:

- exposed-face regions
- edges and corners
- boundary-adjacent features
- seam/gap analog features where feasible

V6 is not yet:

- the AR-05 proof stage
- the IR-06 proof stage
- the full integrated insert stage

It is the damaged-state truth stage for the passive stack.

---

## Why V6 Matters

The Max-01 concept already assumes that failure may begin at:

- the exposed face
- the buried interface
- the support path
- the edge
- the seam
- the boundary ring

V6 exists to expose whether small but realistic damage:

- stays bounded
- grows predictably
- changes thermal behavior gradually
- or instead causes sudden architecture defeat

If minor damage collapses the passive stack too easily, then:

- reuse claims must narrow
- seam logic must rise in priority
- damage tolerance must be reframed honestly
- AR-05 cannot be used as an excuse to hide the weakness

---

## V6 Test Objective

The objective of V6 is to determine whether the best surviving passive stack:

1. remains interpretable under damaged conditions
2. avoids immediate catastrophic collapse from modest realistic flaws
3. reveals where damage sensitivity is most dangerous
4. preserves enough bounded behavior to justify progression toward later optional-branch testing or integrated insert planning
5. exposes whether edges, seams, or face flaws dominate the damage-response story

---

## Primary Question

The primary V6 question is:

> When realistic local damage is introduced, does the surviving passive stack degrade in a bounded, understandable way rather than losing architectural credibility immediately?

---

## Secondary Questions

V6 also asks:

1. Is face damage less dangerous than edge or boundary damage?
2. Does a chipped edge create a worse thermal / structural escalation path than a central surface flaw?
3. Does local damage remain local, or does it rapidly become system-dominant?
4. Does the damaged article still behave better than simpler passive comparisons?
5. Does the damaged-state response reveal where SJ-08 and later integrated boundary logic must focus?
6. Does damage shift the thermal trend enough to expose hidden vulnerability that pristine testing did not show?

---

## Damage Classes Required in V6

The following damage classes are mandatory planning targets.

### D1 — Surface flaw
A controlled surface imperfection introduced on the exposed face.

Intent:
- reveal whether modest face damage causes disproportionate thermal or structural penalty

---

### D2 — Chipped edge
A controlled chip or local loss at the coupon edge.

Intent:
- reveal whether edge distress outruns center damage

---

### D3 — Corner loss
A controlled corner imperfection or missing local corner feature.

Intent:
- reveal whether corner geometry is more failure-sensitive than flat regions

---

### D4 — Boundary / seam analog imperfection
A controlled boundary-like disturbance where feasible.

Intent:
- reveal whether seam-adjacent logic is likely to dominate later integrated behavior

---

### D5 — Post-cycle or post-exposure damage progression
Damage introduced before exposure or tracked across repeated exposure progression.

Intent:
- reveal whether damage remains bounded or accelerates disproportionately

---

## Candidate Set for V6

V6 uses the strongest surviving passive article from V5 and compares pristine versus damaged states.

### Required article families

#### V6-B0
**Pristine surviving passive baseline**

Intent:
- preserve a direct comparison against the undamaged passive article

#### V6-D1
**Surface-flaw damaged article**

Intent:
- isolate exposed-face imperfection sensitivity

#### V6-D2
**Chipped-edge damaged article**

Intent:
- isolate edge damage sensitivity

#### V6-D3
**Corner-loss damaged article**

Intent:
- isolate corner geometry sensitivity

#### V6-D4
**Boundary / seam analog damaged article**
if feasible

Intent:
- reveal whether local boundary imperfection is more dangerous than central damage

---

### Optional comparison families

#### V6-R1
**Damaged simplified passive comparison**
if a simpler passive article remained competitive in V5

Intent:
- determine whether the full passive stack remains worth its complexity even after damage

#### V6-R2
**Multiple severity levels of one damage class**
if test capacity allows

Intent:
- reveal whether damage response is gradual or threshold-like

Reserve comparisons are allowed only if they sharpen the damaged-state truth.

---

## Candidate Naming Rule

The repo may refer to V6 articles using the following identifiers:

- V6-B0
- V6-D1
- V6-D2
- V6-D3
- V6-D4
- V6-R1
- V6-R2

Detailed flaw geometry and process notes may live in later support artifacts, but the stage must remain readable through stable IDs.

---

## Damage Philosophy

The V6 damage philosophy is:

- introduce controlled damage intentionally
- avoid fake perfection
- compare against pristine baseline every time
- prefer bounded, interpretable flaw classes over random breakage
- force the architecture to reveal what kinds of damage matter most

V6 is not about breaking samples for drama.

It is about turning damage into a disciplined truth test.

---

## What V6 Is Trying to Prove

V6 is trying to prove only the following:

1. The passive stack does not depend entirely on pristine geometry to remain meaningful.
2. Some realistic damage classes remain bounded enough that the architecture still behaves coherently.
3. The repo can identify which damage classes are most dangerous.
4. The damaged-state thermal and structural response remains interpretable enough to guide later design priorities.
5. The passive stack still earns itself relative to simpler comparisons after damage is introduced.

---

## What V6 Is Trying to Disprove

V6 is trying to disprove any of the following bad outcomes:

1. Minor damage causes immediate architecture defeat.
2. Edge or corner flaws dominate so completely that prior pristine truth becomes misleading.
3. Damage causes uncontrolled thermal escalation that the analytical posture never anticipated.
4. The full passive stack loses its advantage over simpler comparisons once flaws exist.
5. Damage tolerance is too weak for the intended localized reusable or limited-reuse mission posture.
6. The stack’s most dangerous damage sensitivity was hidden until this stage.

---

## Planned Damage / Exposure Logic

The exact damage tooling and exposure hardware are not frozen in v0.1, but V6 requires a logic severe enough to reveal:

- whether damage stays local or propagates
- whether thermal response changes measurably
- whether edge and boundary flaws are disproportionately severe
- whether structural and oxidation consequences accelerate after damage
- whether the passive stack still behaves better than simpler alternatives once damaged

V6 must not be a cosmetic damage stage.

The flaw must be meaningful enough to challenge the stack honestly.

---

## Planned Observation Set

At minimum, V6 should eventually capture the following.

### O1 — Pre-damage article identity
- article ID
- stack family ID
- comparison class ID
- exposure condition ID

### O2 — Damage definition
- damage class
- damage location
- intended flaw geometry or severity descriptor
- whether damage was pre-exposure or introduced between exposures

### O3 — Post-damage pre-exposure condition
- visual condition after damage introduction
- mass or geometry update if relevant
- edge / corner / flaw documentation
- baseline thermal or structural notes if instrumented

### O4 — During-test observations where feasible
- thermal trend change relative to pristine baseline
- local crack growth
- spall onset
- visible damage propagation
- edge / corner / boundary escalation cues

### O5 — Post-test condition
- final damage extent
- crack pattern
- geometry loss
- local retreat
- interface distress signs
- whether damage remained localized or became system-dominant

### O6 — Comparative ranking notes
- better / similar / worse than pristine baseline
- better / similar / worse than simplified damaged comparison
- bounded / thin-margin / unacceptable damaged-state behavior

The purpose is to reveal **damage response logic**, not only final survival.

---

## Minimum Evaluation Questions per Article Family

Each V6 article family should be judged against the following questions.

### Q1
Did the damaged article remain grossly coherent after exposure?

### Q2
Did the flaw remain bounded or did it trigger rapid architecture-wide distress?

### Q3
Did the thermal trend shift in a way that was measurable and interpretable?

### Q4
Were edge, corner, or boundary flaws more dangerous than face-only flaws?

### Q5
Did the damaged article still remain more credible than simpler damaged comparisons?

### Q6
Does the result support continued passive-first logic with narrowed realism, or force a major scope correction?

### Q7
Has the stage revealed a clear priority for later SJ-08 and integrated insert boundary design?

If the answer set is mostly no, the passive thesis must narrow or be revised.

---

## Stage-Level Pass Conditions

V6 passes only if all of the following are true:

1. At least one damaged article family remains bounded and interpretable.
2. Damage does not immediately destroy the passive architecture’s credibility for the intended localized mission posture.
3. The stage reveals which damage classes are most dangerous and why.
4. The full passive stack remains more credible than simpler damaged comparisons.
5. The results provide useful direction for later boundary logic and optional-branch decisions.

---

## Stage-Level Fail Conditions

V6 fails if any of the following occur:

1. Modest realistic damage causes immediate architecture defeat across all meaningful comparison articles.
2. Edge or boundary flaws reveal that the passive stack is far more fragile than earlier stages suggested.
3. Simpler damaged comparisons perform as well or better in ways that undermine Max-01.
4. The damaged-state response is too chaotic to interpret.
5. The repo tries to preserve the same mission posture despite clearly weak damage tolerance.

If V6 fails, the passive mission envelope must narrow, the boundary logic must rise sharply in priority, or Max-01 must be revised before later stages.

---

## V6 Keep / Cut Logic

### Keep the passive stack if:
- at least one damaged article family remains bounded and interpretable
- the architecture still earns itself relative to simpler damaged comparisons
- the damage-state results support a narrower but still credible passive-first posture

### Downgrade the passive stack if:
- the stack remains interesting, but damage sensitivity is worse than previously implied
- damage tolerance is acceptable only in a narrower subset of the original mission envelope
- edge / boundary logic must become much more central before further claims

### Cut or restructure the current passive thesis if:
- realistic damage consistently collapses the architecture too easily
- simpler damaged comparisons undermine the full stack
- the damaged-state response contradicts the repo’s core localized reusable posture

---

## Controls and Baselines

V6 must not run without the following comparison posture:

- pristine surviving passive baseline
- at least three distinct damage classes
- edge/corner/boundary damage represented, not just central face damage
- simpler damaged comparison if it remains relevant
- thermal and visible comparisons tied together

Without these controls, V6 becomes a stunt instead of a damaged-state truth stage.

---

## V6 Risk Focus

The main risks V6 is trying to expose are:

- damage-triggered passive margin collapse
- boundary-led failure revealed only after flaw introduction
- damage-driven hidden interface escalation
- geometry-loss concentration effects
- false confidence from pristine-only testing
- overcomplex passive logic that does not survive realistic imperfections

If V6 does not expose those risks, it is not doing its job.

---

## What V6 Does Not Prove

Even if V6 succeeds, it does **not** prove:

- AR-05 value
- IR-06 value
- full integrated insert maturity
- final seam-system validity
- flight relevance
- operational refurbishment strategy
- operational reuse capability

V6 is the damaged-state passive truth stage only.

---

## Data Package Required from V6

When V6 is eventually executed, the stage should produce a data package that includes:

- article roster
- flaw definitions
- pre/post-damage imagery
- pre/post-exposure imagery
- thermal observations where available
- mass and geometry notes
- damage-progression summary
- comparative ranking summary
- interpretation of damaged-state credibility
- justification for progression beyond V6

If that package does not exist, V6 has not really been completed.

---

## V6 Exit Decisions

At the end of V6, only the following decisions are valid.

### D1 — Preserve passive-first posture and continue
Use when at least one damaged article family remains credibly bounded.

### D2 — Narrow the damaged-state mission posture
Use when the stack remains interesting but only under tighter damage-tolerance assumptions.

### D3 — Elevate boundary and joint logic priority before later stages
Use when damage shows edges and seams dominate the next truth problem.

### D4 — Simplify the passive architecture before later optional-branch work
Use when simpler damaged comparisons look more credible.

### D5 — Branch to revised reference configuration
Use when damaged-state behavior reveals a deeper contradiction in Max-01.

---

## Relationship to Other Modules

This stage depends on:
- `reference-configs/max-01.md`
- `modules/risk-failure-register.md`
- `modules/oxidation-recession.md`
- `modules/thermo-structural-budget.md`
- V5 survivor logic

This stage informs:
- later SJ-08 emphasis
- later integrated insert planning
- later optional-branch justification logic
- future scope narrowing if needed

---

## V6 Summary

V6 is the stage where IX-HfTaZen-Shield stops asking how the passive stack behaves when everything is ideal and starts asking how it behaves when reality takes a bite out of it.

If the stack cannot remain bounded and interpretable once realistic damage exists, its reuse posture must narrow before anything else gets more ambitious.
