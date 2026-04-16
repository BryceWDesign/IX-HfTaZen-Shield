# V4 Attachment / Mismatch Stack Coupons

## Stage Identity

**Stage:** V4  
**Name:** Attachment / Mismatch Stack Coupons  
**Program:** IX-HfTaZen-Shield  
**Reference configuration:** Max-01  
**Primary architecture layers under test:** HTZ-01 + OX-02 + SD-03 + TC-04, with boundary-aware restraint logic  
**Evidence tier target if later executed:** E3-class coupon evidence  
**Execution status:** planned / frozen for v0.1  
**Purpose:** determine whether the decoupled stack actually reduces thermo-structural mismatch damage relative to more rigid comparison architectures

---

## Stage Purpose

V4 exists because Max-01 makes a strong structural claim:

> The stack is more credible when thermal mismatch is treated as a first-class architecture problem instead of being left to the hot face and support structure to “work out” on their own.

That claim must earn its place.

V4 is the stage where the program forces the stack to answer a harder question than V3:

> Does the decoupled layered stack behave better than more rigid or under-decoupled comparisons when real restraint and thermal mismatch are part of the test logic?

V4 is the first stage centered explicitly on the **thermo-structural thesis** of Max-01.

---

## What V4 Is Testing

V4 is testing the interaction of:

- the surviving HTZ-01 hot-face direction
- the surviving OX-02 transition direction
- one or more SD-03 decoupling candidates
- one or more TC-04 carrier/support concepts or stiffness/thermal-choke analogs
- restrained or gradient-driven mismatch conditions that force the stack to reveal whether its decoupling logic is real

V4 is not yet the full integrated insert stage.

It is still a coupon / stack-article truth stage.

---

## Why V4 Matters

A severe localized TPS insert can fail even if:

- the hot-face family looks good in V1
- the buried transition looks helpful in V2
- the early layered direction survives cycling in V3

because those stages do not yet force the stack to fully reveal whether:

- the upper and lower layers want to move incompatibly
- the decoupling logic is actually strong enough to matter
- the carrier choice is helping or silently punishing the stack
- the interface stack is robust under restraint rather than only under freer coupon conditions

V4 exists to expose that.

---

## V4 Test Objective

The objective of V4 is to determine whether the Max-01 stack’s decoupling and carrier logic:

1. reduces thermo-structural mismatch distress relative to rigid-stack comparisons
2. preserves layered coherence under restrained thermal loading
3. avoids turning OX-02 into an interface crack trap
4. avoids turning TC-04 into a thermal and structural punishment path
5. preserves enough integrity to justify V5 high-heat coupon exposure and later integrated insert planning

---

## Primary Question

The primary V4 question is:

> Does the HTZ-01 + OX-02 + SD-03 + TC-04 direction materially improve mismatch survivability relative to more rigid or under-decoupled comparisons?

---

## Secondary Questions

V4 also asks:

1. Is SD-03 doing meaningful structural work or just adding stack complexity?
2. Is TC-04 helping as a support and thermal choke, or acting like a hidden rigid penalty?
3. Does OX-02 remain acceptable once restraint and mismatch loading are included?
4. Are boundaries, edges, or restraint points now more failure-prone than the coupon center?
5. Does the layered stack fail more gracefully than rigid comparisons?
6. Does the thermal trend suggest that mismatch damage is undermining the thermal thesis?

---

## Candidate Set for V4

V4 is built from survivors of V1–V3.

### Required comparison families

#### V4-B1
**HTZ-01 + OX-02 baseline without explicit decoupling**

Intent:
- provide a direct “less decoupled” baseline for comparison

#### V4-C1
**HTZ-01 + OX-02 + SD-03 candidate A + TC-04 candidate A**

Intent:
- first full mismatch-aware stack comparison

#### V4-C2
**HTZ-01 + OX-02 + SD-03 candidate B + TC-04 candidate A**

Intent:
- isolate SD-03 implementation effect while holding carrier logic steady

#### V4-C3
**HTZ-01 + OX-02 + SD-03 candidate A + TC-04 candidate B or alternate carrier logic**

Intent:
- isolate carrier/support effect while holding decoupling logic steady

---

### Optional comparison families

#### V4-R1
**Rigid-stack comparison with hard-bond or highly restrained architecture**

Intent:
- deliberately expose the penalty of over-rigid integration

#### V4-R2
**Simplified decoupling comparison**

Intent:
- determine whether the full SD-03 concept is earning its complexity

Reserve comparisons are allowed only if they sharpen the structural truth instead of blurring it.

---

## Candidate Naming Rule

The repo may refer to V4 stack articles using the following identifiers:

- V4-B1
- V4-C1
- V4-C2
- V4-C3
- V4-R1
- V4-R2

Detailed process, geometry, and restraint details may be tracked in later support artifacts, but the stage must remain readable through stable IDs.

---

## Stack-Article Philosophy

The V4 philosophy is:

- compare decoupled against less decoupled
- compare alternate decoupling and carrier choices
- include restraint or gradient logic that forces mismatch to matter
- avoid hiding structural problems behind thermal storytelling
- observe where the stack fails first under mismatch burden

V4 is not merely about “did it crack.”

It is about **how** it cracked, **where**, and **relative to what comparison**.

---

## What V4 Is Trying to Prove

V4 is trying to prove only the following:

1. The SD-03 + TC-04 thesis is real enough to remain in Max-01.
2. The decoupled stack behaves better under mismatch than less decoupled comparisons.
3. The layered architecture can preserve coherence under restrained thermal loading.
4. The hot-face and transition logic are still compatible once structural reality is introduced.
5. The stack deserves to advance to V5 severe high-heat exposure.

---

## What V4 Is Trying to Disprove

V4 is trying to disprove any of the following bad outcomes:

1. SD-03 is decorative rather than functional.
2. TC-04 silently amplifies both heat leakage and structural restraint.
3. OX-02 becomes the interface failure plane under mismatch.
4. The decoupled stack performs no better than rigid or simplified comparisons.
5. The carrier/support concept undermines the thermal architecture.
6. The current Max-01 stack is structurally less coherent than it appears.

---

## Planned Mismatch / Restraint Logic

The exact fixture and restraint design are not frozen in v0.1, but V4 requires a test logic severe enough to reveal:

- thermal-expansion mismatch behavior
- restraint sensitivity
- interface distress
- crack initiation location
- whether the decoupling layer reduces or merely relocates the damage
- whether carrier logic helps or hurts the stack

V4 must not be a free-expansion stage that politely avoids the real problem.

---

## Planned Observation Set

At minimum, V4 should eventually capture the following.

### O1 — Pre-test article identity
- stack article ID
- HTZ-01 / OX-02 / SD-03 / TC-04 identities
- geometry ID
- restraint / support condition ID

### O2 — Baseline condition
- initial visual condition
- initial mass
- initial geometry / thickness
- interface documentation where feasible
- edge / corner / support-point condition

### O3 — During-test observations if instrumented
- displacement or strain trend where feasible
- thermal trend at protected side where feasible
- signs of local instability near restraint regions

### O4 — Post-test visible condition
- crack initiation location
- crack growth path
- interface separation
- edge distress
- support-point distress
- warping or loss of layered coherence

### O5 — Post-test thermal observations
- backface trend shift relative to expectation
- evidence that structural damage altered the thermal path

### O6 — Post-test comparative ranking notes
- better / similar / worse than the less-decoupled baseline
- better / similar / worse than rigid comparison
- whether the decoupler and carrier earned their places

The purpose is to identify the **dominant structural truth** of the stack.

---

## Minimum Evaluation Questions per Stack Family

Each V4 stack family should be judged against the following questions.

### Q1
Did the stack remain grossly intact under the planned mismatch / restraint condition?

### Q2
Did SD-03 reduce apparent mismatch distress relative to less-decoupled comparisons?

### Q3
Did TC-04 help preserve stack coherence or behave like a hidden penalty?

### Q4
Did OX-02 remain acceptable once structural mismatch was added to the problem?

### Q5
Did the failure location stay understandable and bounded?

### Q6
Did the decoupled stack outperform rigid or simplified comparisons in a meaningful way?

### Q7
Is this stack family worth carrying into V5 and later integrated logic?

If the answer set is mostly no, that family should be downgraded or cut.

---

## Stage-Level Pass Conditions

V4 passes only if all of the following are true:

1. At least one SD-03 + TC-04 stack family remains more coherent under mismatch than less-decoupled comparisons.
2. The decoupling logic appears to reduce real structural penalty rather than merely move it invisibly.
3. OX-02 does not become an immediate disqualifying brittle plane under mismatch conditions.
4. The selected stack remains plausible enough to justify V5 severe high-heat exposure.
5. The repo can clearly explain why the surviving stack family continues.

---

## Stage-Level Fail Conditions

V4 fails if any of the following occur:

1. Decoupled comparisons do not outperform simpler or rigid baselines meaningfully.
2. SD-03 repeatedly fails to earn its place.
3. TC-04 repeatedly acts like a thermal-stress amplifier.
4. The stack loses structural coherence under restraint too early for the intended mission posture.
5. The stage cannot distinguish whether the problem lies in the decoupler, the transition, or the carrier.
6. The repo tries to carry forward a weak mismatch thesis anyway.

If V4 fails, Max-01 must be simplified, narrowed, or restructured before V5.

---

## V4 Keep / Cut Logic

### Keep SD-03 / TC-04 logic if:
- at least one decoupled stack family clearly outperforms less-decoupled comparisons
- the improvement is architectural, not cosmetic
- the stack remains interpretable and bounded

### Downgrade SD-03 / TC-04 logic if:
- some value appears real, but the implementation is weak or too narrow
- a simpler decoupling or carrier route now looks more credible

### Cut or restructure the current mismatch thesis if:
- rigid or simplified comparisons perform equally well or better
- SD-03 and TC-04 fail to justify their complexity
- the stack’s structural logic collapses under restraint

---

## Controls and Baselines

V4 must not run without the following control philosophy:

- at least one no-decoupling or less-decoupled baseline
- at least one SD-03 comparison
- at least one TC-04 comparison
- at least one rigid or highly restrained comparison if feasible
- thermal and structural observations tied together where possible

Without these controls, V4 cannot honestly evaluate whether the stack’s structural thesis is real.

---

## V4 Risk Focus

The main risks V4 is trying to expose are:

- hot-face / support mismatch cracking
- decoupling layer underperformance
- carrier thermal-stress amplification
- transition-layer brittleness under restraint
- boundary / support-point distress
- false confidence from freer earlier coupon stages
- structural contradictions hidden inside the layered stack

If V4 does not expose those risks, it is not doing its job.

---

## What V4 Does Not Prove

Even if V4 succeeds, it does **not** prove:

- final seam-system validity
- AR-05 value
- IR-06 value
- integrated insert maturity
- full severe-environment survivability
- flight relevance
- operational reuse capability

V4 is the mismatch-thesis truth stage only.

---

## Data Package Required from V4

When V4 is eventually executed, the stage should produce a data package that includes:

- stack article roster
- restraint / support condition definition
- pre/post imagery
- geometry and mass notes
- thermal and structural observation notes
- failure-location summary
- comparative ranking summary
- justification for stack family(ies) advanced to V5

If that package does not exist, V4 has not really been completed.

---

## V4 Exit Decisions

At the end of V4, only the following decisions are valid.

### D1 — Advance surviving mismatch-aware stack family(ies) to V5
Use when one or more decoupled stack families remain structurally credible.

### D2 — Narrow the decoupling or carrier logic before V5
Use when the thesis remains useful but the implementation is weak.

### D3 — Simplify the stack architecture before V5
Use when the current SD-03 / TC-04 logic is not earning its place honestly.

### D4 — Repeat V4 with corrected mismatch / restraint logic
Use when the stage setup failed to expose the real structural question.

### D5 — Branch to revised reference configuration
Use when mismatch behavior reveals a deeper contradiction in Max-01.

---

## Relationship to Other Modules

This stage depends on:
- `reference-configs/max-01.md`
- `modules/thermo-structural-budget.md`
- `modules/risk-failure-register.md`
- V1 / V2 / V3 survivor logic

This stage informs:
- V5 high-heat coupon exposure planning
- future SD-03 and TC-04 narrowing decisions
- later integrated insert logic
- potential Max-02 branching if needed

---

## V4 Summary

V4 is the stage where IX-HfTaZen-Shield forces its structural thesis to prove itself under restraint and thermal mismatch.

If the decoupled stack cannot outperform more rigid comparisons here, it does not deserve to carry its current complexity into later stages.
