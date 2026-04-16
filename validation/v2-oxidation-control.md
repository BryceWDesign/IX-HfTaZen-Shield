# V2 Oxidation-Control Coupons

## Stage Identity

**Stage:** V2  
**Name:** Oxidation-Control Coupons  
**Program:** IX-HfTaZen-Shield  
**Reference configuration:** Max-01  
**Primary architecture layers under test:** HTZ-01 + OX-02  
**Evidence tier target if later executed:** E3-class coupon evidence  
**Execution status:** planned / frozen for v0.1  
**Purpose:** determine whether the buried oxidation-control transition improves stack credibility relative to no-transition baselines

---

## Stage Purpose

V2 exists because IX-HfTaZen-Shield does **not** assume the exposed-face material alone solves the oxidizing-use problem.

The stack thesis says:

- HTZ-01 carries the direct exposed thermal burden
- OX-02 exists to improve the buried oxidation and interface logic
- that improvement must be earned, not assumed

V2 is the stage where OX-02 must prove it is doing useful work rather than acting as:

- a brittle penalty layer
- a cosmetic chemistry flourish
- an unnecessary complication
- a hidden failure plane beneath a strong-looking surface

---

## What V2 Is Testing

V2 is testing the value of **OX-02 as a buried oxidation-control transition** beneath the selected V1-surviving HTZ-01 direction.

It is not yet testing:

- full SD-03 performance
- full TC-04 performance
- AR-05
- IR-06
- HB-07 as an integrated backplane
- full seam / boundary architecture

V2 is still a coupon-level logic stage.

---

## V2 Test Objective

The objective of V2 is to determine whether the addition of OX-02:

1. improves the buried oxidation-control logic of the stack
2. reduces interfacial damage risk relative to HTZ-01-only baselines
3. stays mechanically coherent enough to justify deeper layered testing
4. preserves or improves overall survivability logic under oxidizing exposure
5. avoids becoming a brittle interfacial trap

---

## Primary Question

The primary V2 question is:

> Does HTZ-01 + OX-02 behave more credibly than HTZ-01 alone under oxidizing coupon exposure logic?

---

## Secondary Questions

V2 also asks:

1. Is the chosen OX-02 family actually helping, or just adding fragility?
2. Does OX-02 improve buried-interface logic enough to justify carrying it into V3 and V4?
3. Does OX-02 remain compatible with the selected HTZ-01 direction?
4. Do alternative OX-02 implementations matter enough to compare now?
5. Is the transition layer making the stack more oxidation-aware **and** more mechanically fragile at the same time?

---

## Candidate Set for V2

V2 uses the top surviving HTZ-01 direction from V1 and compares OX-02 variants against no-transition controls.

### Required baseline set

#### V2-B0
**HTZ-01 only baseline**

Intent:
- establish what the selected hot-face family does without a buried oxidation-control transition

---

### Primary OX-02 candidates

#### V2-O1
**HTZ-01 + OX-02 primary transition variant A**

Intent:
- first primary HfSiCN-class buried oxidation-control implementation

#### V2-O2
**HTZ-01 + OX-02 primary transition variant B**

Intent:
- altered OX-02 implementation for comparison within the same family direction

---

### Secondary OX-02 candidates

#### V2-O3
**HTZ-01 + secondary silicon-bearing transition variant**

Intent:
- determine whether the HfSiCN-class direction is meaningfully stronger than a broader silicon-bearing refractory transition concept

---

### Optional reserve comparison

#### V2-R1
**HTZ-01 + simplified thin transition concept**

Intent:
- determine whether a lower-complexity transition captures most of the value of the primary OX-02 direction

Reserve candidates are allowed only if they do not weaken the main comparison logic.

---

## Candidate Naming Rule

The repo may refer to V2 candidates using the following identifiers:

- V2-B0
- V2-O1
- V2-O2
- V2-O3
- V2-R1

Exact thickness, formulation, and process details may live in supporting artifacts later, but the stage logic should remain readable through stable IDs.

---

## Coupon Philosophy

The V2 coupon philosophy is:

- keep the comparison focused on the value of the transition layer
- do not hide OX-02 inside too many additional layers yet
- compare against a no-transition baseline every time
- judge OX-02 as both a chemistry helper and a mechanics liability candidate
- treat visible surface condition and buried interface condition as separate truths

The exposed face can look acceptable while the buried transition is already losing.

V2 exists to catch that possibility.

---

## What V2 Is Trying to Prove

V2 is trying to prove only the following:

1. A buried oxidation-control transition can improve stack logic relative to no-transition HTZ-01 controls.
2. OX-02 adds value in an oxidizing coupon regime that matters more than its penalties.
3. The selected OX-02 family is worth carrying into V3 and V4.
4. The stack’s oxidation-control thesis remains credible beyond rhetoric.

---

## What V2 Is Trying to Disprove

V2 is trying to disprove any of the following bad outcomes:

1. OX-02 is unnecessary.
2. OX-02 helps chemistry but creates unacceptable mechanical brittleness.
3. OX-02 becomes the first real failure plane.
4. The selected OX-02 family is not better than simpler transition logic.
5. The buried transition strategy is overcomplicated relative to the gain it provides.
6. The repo’s separate oxidation-control thesis is weaker than a simpler exposed-face-only path.

---

## Required Comparisons

The following comparisons are mandatory.

### Comparison C1
V2-B0 versus V2-O1

Reason:
- first proof test of whether the primary buried transition adds value at all

### Comparison C2
V2-O1 versus V2-O2

Reason:
- avoid treating one arbitrary OX-02 implementation as sufficient proof

### Comparison C3
V2-O1 / V2-O2 versus V2-O3

Reason:
- determine whether the preferred HfSiCN-class direction is actually earning its primary status

### Comparison C4
Any OX-02 variant versus HTZ-01-only post-test interface condition

Reason:
- the whole point is whether buried behavior improved

---

## Planned Exposure Logic

The exact test hardware is not frozen in v0.1, but the V2 planning logic requires an oxidizing coupon regime severe enough to reveal:

- whether OX-02 is doing anything meaningful
- whether OX-02 remains adherent and coherent
- whether the buried interface looks better or worse than the no-transition baseline
- whether visible surface stability hides buried weakness
- whether candidate OX-02 implementations separate clearly enough to guide later stages

V2 is not yet the full severe-heat coupon stage.
It is a transition-layer truth stage.

---

## Planned Observation Set

At minimum, V2 should eventually capture the following.

### O1 — Pre-test coupon identity
- HTZ-01 candidate identity
- OX-02 candidate identity if present
- coupon geometry ID
- batch/process notes

### O2 — Pre-test condition
- surface appearance
- baseline mass
- baseline geometry
- visible interface preparation notes

### O3 — Post-exposure visible condition
- exposed-face cracking
- surface-state change
- edge condition
- obvious delamination indicators

### O4 — Post-exposure buried/interface condition
- interface cracking
- layer separation
- scale behavior near or through the transition
- sectioned or inspected subsurface condition if feasible

### O5 — Post-exposure mass trend
- before/after mass comparison

### O6 — Post-exposure geometry trend
- thickness loss
- local retreat
- edge degradation

### O7 — Comparative ranking notes
- better / similar / worse than no-transition baseline
- better / similar / worse than alternate transition variants

The key distinction in V2 is that **surface appearance alone is not enough**.

---

## Minimum Evaluation Questions per Candidate

Each OX-02 candidate should be judged against the following questions.

### Q1
Did the layered coupon remain grossly intact?

### Q2
Did the exposed-face / transition system avoid obvious catastrophic separation?

### Q3
Did the buried interface look better, similar, or worse than HTZ-01 alone?

### Q4
Did the transition layer appear to reduce deeper oxidation-related damage logic?

### Q5
Did the transition layer avoid becoming an obvious brittle trap?

### Q6
Is this variant worth carrying into V3 and V4?

If the answer set is mostly no, that candidate should be downgraded or cut.

---

## Stage-Level Pass Conditions

V2 passes only if all of the following are true:

1. At least one OX-02 variant improves the buried oxidation-control logic relative to HTZ-01-only baseline.
2. That improvement is not obviously canceled out by brittle interfacial penalty.
3. The results narrow the preferred OX-02 direction instead of making it vaguer.
4. The repo can explain why the surviving transition candidate continues into V3 and V4.

---

## Stage-Level Fail Conditions

V2 fails if any of the following occur:

1. No OX-02 candidate improves on HTZ-01-only behavior in a meaningful way.
2. OX-02 repeatedly becomes the first dominant failure plane.
3. The transition family adds more interfacial penalty than oxidation-control value.
4. The comparison logic is too weak to distinguish the transition candidates honestly.
5. The repo tries to keep OX-02 anyway out of attachment to the original stack thesis.

If V2 fails, OX-02 must be revised, simplified, or removed before moving on.

---

## V2 Keep / Cut Logic

### Keep the OX-02 direction if:
- at least one transition candidate improves buried oxidation-control logic
- the surviving variant remains mechanically credible enough to continue
- the stage supports a narrower, more defensible OX-02 direction

### Downgrade the OX-02 direction if:
- some benefit appears real, but the mechanical or interface penalty is too high
- a simpler transition route now looks more credible than the original primary direction

### Cut the OX-02 direction if:
- no transition candidate beats the HTZ-01-only baseline meaningfully
- the transition layer repeatedly behaves like a brittle trap
- the separate buried oxidation-control thesis is not earning its place

---

## Controls and Baselines

V2 must not run without the following baseline philosophy:

- every OX-02 candidate must be compared against HTZ-01-only
- at least two OX-02 variants should be compared
- simpler transition logic should be compared where feasible
- visible condition must not be allowed to overrule buried/interface evidence by itself

Without these controls, V2 becomes a confirmation exercise instead of a truth test.

---

## V2 Risk Focus

The main risks V2 is trying to expose early are:

- hidden interface oxidation
- transition-layer brittleness
- false optimism from surface-only inspection
- overcomplicated OX-02 logic with no real gain
- chemistry improvement that creates structural penalty
- carrying a weak buried-transition concept forward into the rest of the stack

If V2 cannot expose those risks, it is not doing its job.

---

## What V2 Does Not Prove

Even if V2 succeeds, it does **not** prove:

- full SD-03 effectiveness
- full TC-04 effectiveness
- seam durability
- AR-05 viability
- IR-06 viability
- integrated insert survivability
- flight relevance
- reuse life

V2 is a buried oxidation-control truth stage only.

---

## Data Package Required from V2

When V2 is eventually executed, the stage should produce a data package that includes:

- coupon roster
- HTZ-01 / OX-02 pairing matrix
- exposure conditions
- pre/post imagery
- mass and geometry notes
- sectioned or interface inspection notes where feasible
- comparative ranking summary
- justification for the OX-02 candidate advanced to V3 / V4

If that package does not exist, V2 has not really been completed.

---

## V2 Exit Decisions

At the end of V2, only the following decisions are valid.

### D1 — Advance surviving OX-02 candidate(s) to V3 and V4
Use when at least one transition implementation remains credible.

### D2 — Simplify or revise OX-02 before V3 / V4
Use when the transition thesis remains useful but the current implementation is weak.

### D3 — Remove the buried-transition concept from Max-01
Use when no transition candidate earns continuation honestly.

### D4 — Repeat V2 with corrected comparison logic
Use when the stage setup was too weak to support a real decision.

---

## Relationship to Other Modules

This stage depends on:
- `reference-configs/max-01.md`
- `modules/materials-screening.md`
- `modules/oxidation-recession.md`
- `modules/risk-failure-register.md`

This stage informs:
- V3 thermal shock / cycle planning
- V4 attachment / mismatch stack planning
- future OX-02 narrowing decisions

---

## V2 Summary

V2 is the stage where IX-HfTaZen-Shield forces its buried oxidation-control idea to prove that it is genuinely helping the stack.

If OX-02 cannot improve the buried oxidation and interface logic relative to no-transition controls, it does not deserve to remain in Max-01.
