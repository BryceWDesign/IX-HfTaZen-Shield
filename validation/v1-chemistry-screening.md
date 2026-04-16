# V1 Chemistry Screening

## Stage Identity

**Stage:** V1  
**Name:** Chemistry-Screening Coupons  
**Program:** IX-HfTaZen-Shield  
**Reference configuration:** Max-01  
**Primary architecture layer under test:** HTZ-01 Radiative UHTC Face  
**Evidence tier target if later executed:** E3-class coupon evidence  
**Execution status:** planned / frozen for v0.1  
**Purpose:** identify whether the primary hot-face material lane is strong enough to justify deeper stack integration

---

## Stage Purpose

V1 is the first physical screening gate planned for IX-HfTaZen-Shield.

This stage exists to answer a narrow but critical question:

> Is the chosen HTZ-01 hot-face direction actually worth building the rest of the architecture around?

The program does not get to hide weak hot-face logic behind:
- a clever transition layer
- a clever decoupling layer
- a clever active branch
- a clever monitoring story

If the exposed-face lane is not credible relative to simpler comparison families, the stack must be simplified or redirected before deeper integration begins.

---

## What V1 Is Testing

V1 is testing **candidate hot-face chemistry families only**.

It is not yet testing:
- full Max-01 integration
- AR-05
- IR-06
- HB-07
- full SJ-08 behavior
- final carrier architecture

The point of V1 is disciplined separation.

---

## V1 Test Objective

The objective of V1 is to rank the credibility of HTZ-01 candidate families under an initial coupon-level screening program that emphasizes:

- exposed-face survivability
- visible integrity
- comparative degradation resistance
- early oxidation-screening coherence
- compatibility with later layered evolution

V1 is a **comparison stage**, not a hero-shot stage.

---

## Primary Question

The primary question for V1 is:

> Does the Hf-rich Hf–Ta–Zr–W–(C,N) primary lane earn the right to remain the leading HTZ-01 direction for Max-01?

---

## Secondary Questions

V1 also asks:

1. Is the reduced-complexity Hf–Ta–(C,N) lane nearly as good or better?
2. Do simpler HfC / TaC / Ta-Hf comparison families perform well enough to justify a simpler path?
3. Is tungsten participation helping enough to justify remaining in the primary lane?
4. Does carbonitride tuning appear worthwhile relative to simpler carbide-only comparisons?
5. Are any candidate families obviously too fragile, too unstable, or too contradictory to continue?

---

## Candidate Set for V1

The planned V1 candidate set is frozen as follows.

### Primary lane candidates
These represent the preferred HTZ-01 direction.

#### V1-P1
**Hf-rich Hf–Ta–Zr–W–(C,N) candidate A**

Intent:
- balanced primary-lane reference
- baseline primary comparison point

#### V1-P2
**Hf-rich Hf–Ta–Zr–W–(C,N) candidate B**

Intent:
- shifted ratio inside the same primary lane
- tests whether a different internal weighting improves early behavior

#### V1-P3
**Hf-rich Hf–Ta–Zr–W–(C,N) candidate C**

Intent:
- alternate primary-lane composition variant
- helps avoid overcommitting to one exact internal proportion too early

---

### Secondary lane candidates

#### V1-S1
**Hf–Ta–(C,N) reduced-complexity lane**

Intent:
- test whether a simpler lane preserves most of the value of the primary family

#### V1-S2
**Hf–Zr–Ta carbide / carbonitride lane without W**

Intent:
- isolate whether W participation is helping enough to justify it

#### V1-S3
**HfC / TaC / Ta-Hf comparison lane**

Intent:
- provide a serious simpler baseline grounded in classic UHTC logic

---

### Reserve candidates
Reserve candidates may be included only if test capacity supports them without diluting the main question.

#### V1-R1
**Hf–Zr carbonitride reserve lane**

#### V1-R2
**Ta-rich reserve UHTC lane**

Reserve candidates are allowed only if the main primary-versus-secondary comparison remains clean.

---

## Candidate Naming Rule

During V1, exact internal chemistry ratios should be tracked in the test plan, but the repo may still refer to candidates using stable identifiers:

- V1-P1
- V1-P2
- V1-P3
- V1-S1
- V1-S2
- V1-S3
- V1-R1
- V1-R2

This keeps the evidence package readable while preserving technical specificity in supporting artifacts.

---

## Coupon Philosophy

The V1 coupon philosophy is:

- keep the geometry simple enough to isolate chemistry-family behavior
- do not overdesign fixtures until chemistry direction earns it
- compare multiple candidates under matched conditions
- prefer clean ranking logic over dramatic one-off samples
- do not pretend a single coupon result settles the full architecture

V1 must stay honest about what it can and cannot say.

---

## What V1 Is Trying to Prove

V1 is trying to prove only the following:

1. At least one primary-lane candidate is credible enough to continue.
2. The chosen primary lane is not obviously outclassed by simpler comparison families.
3. The exposed-face material discussion can move from pure theory toward disciplined screening evidence.
4. There is a defensible reason to preserve the Hf-rich high-entropy/carbonitride direction into later layered testing.

---

## What V1 Is Trying to Disprove

V1 is trying to disprove any of the following bad outcomes:

1. The primary lane is overcomplicated with no meaningful gain.
2. Simpler families perform equally well or better in ways that matter more.
3. The primary lane shows obvious instability, gross cracking, or unacceptable degradation too early.
4. Carbonitride tuning is adding complexity without apparent benefit.
5. W participation adds more penalty than value.
6. The repo’s chosen hot-face direction is more prestige-driven than evidence-driven.

---

## V1 Required Comparisons

The following comparisons are mandatory.

### Comparison C1
Primary-lane candidates versus each other

Reason:
- avoid anchoring on one arbitrary version of the primary family

### Comparison C2
Primary-lane candidates versus reduced-complexity Hf–Ta–(C,N)

Reason:
- test whether the main lane is actually earning its complexity

### Comparison C3
Primary-lane candidates versus W-free Hf–Zr–Ta lane

Reason:
- isolate W’s role at a screening level

### Comparison C4
Primary-lane candidates versus simpler HfC / TaC / Ta-Hf baseline

Reason:
- force the architecture to justify itself against a simpler serious alternative

---

## Planned Exposure Logic

The exact exposure hardware is not frozen in v0.1, but the stage planning requires that V1 eventually expose coupons to a matched screening regime that is sufficient to reveal:

- gross thermal survivability differences
- obvious cracking differences
- obvious oxidation-screening differences
- gross integrity loss
- visible ranking behavior

V1 is not meant to replace later high-heat or integrated testing.

It is meant to reveal early material-family direction.

---

## Planned Observation Set

At minimum, V1 should eventually capture the following for each coupon:

### O1 — Pre-test coupon identity
- candidate ID
- geometry ID
- batch identity
- preparation notes

### O2 — Pre-test condition
- visual condition
- baseline mass
- baseline dimensions or representative geometry
- surface notes

### O3 — Post-exposure visible condition
- cracking
- surface-state change
- chipping
- spall signs
- warping or gross integrity loss

### O4 — Post-exposure mass trend
- before/after mass comparison

### O5 — Post-exposure geometry trend
- thickness or profile change if measurable
- obvious edge retreat or corner loss

### O6 — Comparative ranking notes
- better / similar / worse relative to matched controls

The purpose is not to collect every possible datum.
The purpose is to collect enough truth to rank the candidates honestly.

---

## Minimum Pass/Fail Logic per Candidate

Each candidate should be judged against the following first-pass questions.

### Q1
Did the coupon remain grossly intact under the planned screening exposure?

### Q2
Did it avoid obviously catastrophic cracking relative to peers?

### Q3
Did it avoid obviously unacceptable visible degradation relative to peers?

### Q4
Did it preserve enough integrity to remain interesting for later stack integration?

### Q5
Did it outperform or at least justify itself against simpler comparison families?

If the answer set is mostly no, the candidate should be downgraded or cut.

---

## Stage-Level Pass Conditions

V1 passes only if all of the following are true:

1. At least one primary-lane candidate remains credible.
2. The primary lane is not clearly defeated by simpler comparison families.
3. The results give a rational basis for selecting one or more candidates for V2/V3 continuation.
4. The outcome narrows the HTZ-01 direction rather than making it vaguer.
5. The repo can explain why the surviving lane continues.

---

## Stage-Level Fail Conditions

V1 fails if any of the following occur:

1. All primary-lane candidates show early behavior that makes the lane implausible.
2. Simpler comparison families outperform the primary lane in a way that undermines the current HTZ-01 thesis.
3. The comparison logic is too weak to distinguish candidates honestly.
4. The stage produces noise instead of a ranking.
5. The repo tries to protect the primary lane despite weak evidence.

If V1 fails, the hot-face direction must be simplified or revised before V2.

---

## V1 Keep / Cut Logic

### Keep the primary lane if:
- one or more primary candidates remain credible
- the lane earns at least directional value over simpler controls
- the screening results justify deeper investigation

### Downgrade the primary lane if:
- performance is mixed and not clearly better than simpler families
- some features of the lane appear useful but not enough to stay fully primary

### Cut the primary lane if:
- simpler candidates dominate
- instability is obvious
- the main lane no longer looks like the best exposed-face direction for Max-01

---

## Controls and Baselines

V1 must not run without meaningful baselines.

At minimum, the following control philosophy is required:

- compare complex against simpler
- compare W-containing against W-free
- compare carbonitride direction against simpler carbide logic where feasible
- compare multiple primary-lane variants rather than one arbitrarily chosen example

Without those comparisons, V1 becomes story-building instead of screening.

---

## V1 Risk Focus

The main risks V1 is trying to expose early are:

- overcomplicated hot-face chemistry with no real gain
- early cracking
- early visible degradation
- false optimism about the primary lane
- premature attachment to one composition
- evidence-free continuation of a weak material direction

If V1 cannot expose those risks, it is not doing its job.

---

## What V1 Does Not Prove

Even if V1 succeeds, it does **not** prove:

- full-stack performance
- OX-02 value
- SD-03 value
- seam durability
- integrated insert survivability
- active-relief viability
- recovery-branch viability
- flight relevance
- reuse life

V1 is a material-family screening gate only.

---

## Data Package Required from V1

When V1 is eventually executed, the stage should produce a data package that includes:

- candidate roster
- coupon identities
- exposure conditions
- pre/post imagery
- mass and geometry notes
- comparative ranking summary
- justification for candidates advanced to V2

If that package does not exist, V1 has not really been completed.

---

## V1 Exit Decisions

At the end of V1, only the following decisions are valid.

### D1 — Advance primary-lane survivors to V2
Use when at least one primary-lane candidate remains defensible.

### D2 — Simplify HTZ-01 direction before V2
Use when the primary lane is not clearly winning and a simpler route now looks more credible.

### D3 — Repeat V1 with corrected candidate logic
Use when the candidate set or comparison logic was too weak to support a real decision.

### D4 — Narrow the mission envelope
Use when even the best hot-face candidates do not support the current ambition level honestly.

---

## Relationship to Other Modules

This stage depends on:
- `reference-configs/max-01.md`
- `modules/materials-screening.md`
- `modules/claims-evidence-ladder.md`
- `modules/risk-failure-register.md`

This stage informs:
- V2 oxidation-control planning
- V3 thermal shock / cycle planning
- future HTZ-01 narrowing decisions

---

## V1 Summary

V1 is the stage where IX-HfTaZen-Shield stops assuming its chosen hot-face direction deserves trust.

Instead, it makes the hot-face direction compete against simpler serious alternatives.

That is the only honest way to decide whether the exposed-face thesis of Max-01 should continue.
