# V3 Thermal Shock / Cycle Coupons

## Stage Identity

**Stage:** V3  
**Name:** Thermal Shock / Cycle Coupons  
**Program:** IX-HfTaZen-Shield  
**Reference configuration:** Max-01  
**Primary architecture layers under test:** HTZ-01 + OX-02, with early SD-03 logic included where justified  
**Evidence tier target if later executed:** E3-class coupon evidence  
**Execution status:** planned / frozen for v0.1  
**Purpose:** determine whether the candidate layered direction remains credible under repeated thermal swings rather than only a single exposure

---

## Stage Purpose

V3 exists because a layered extreme-heat TPS concept can look strong in a single exposure and still be weak in the way that matters most for reuse or limited reuse:

- repeated thermal loading
- repeated cooldown
- repeated gradient-driven strain
- repeated surface / subsurface evolution
- repeated edge and interface punishment

V3 is the stage where IX-HfTaZen-Shield forces the early stack direction to answer a harder question:

> Does the architecture remain coherent when heat happens more than once?

---

## What V3 Is Testing

V3 is testing the **cycling honesty** of the early layered direction.

The stage focuses on:

- selected HTZ-01 survivor(s) from V1
- selected OX-02 survivor(s) from V2
- early SD-03 comparison where it is appropriate to include a decoupling concept at coupon scale

V3 is **not yet** the full integrated insert stage.

It is still a coupon-level truth stage.

---

## Why V3 Matters

The entire repo is built around the idea that:

- oxidation matters
- mismatch stress matters
- interfaces matter
- boundaries matter
- localized reuse or limited reuse is desirable

All of those truths become harder under cycling.

A stack that survives one exposure but loses coherence after a few thermal swings is not a strong foundation for Max-01.

That is why V3 exists before heavier integration.

---

## V3 Test Objective

The objective of V3 is to determine whether the selected layered direction can survive repeated thermal cycling with enough structural and functional coherence to justify:

- continued confidence in HTZ-01
- continued confidence in OX-02
- continued inclusion of SD-03 logic
- progression to V4 attachment / mismatch testing
- progression to V5 high-heat coupon exposure

V3 is also meant to expose whether the layered architecture is:

- too brittle
- too interface-sensitive
- too dependent on one-time exposure assumptions
- too optimistic about limited reuse

---

## Primary Question

The primary V3 question is:

> Does the selected layered direction remain more coherent than rigid or oversimplified comparisons when subjected to repeated thermal shock / cycle conditions?

---

## Secondary Questions

V3 also asks:

1. Does the selected HTZ-01 + OX-02 pairing degrade gracefully or abruptly under repeated exposure?
2. Does early SD-03 inclusion improve cycling survivability or merely complicate the coupon?
3. Does the no-decoupling comparison become visibly worse across cycles?
4. Does damage accumulate in a way that stays bounded and interpretable?
5. Are edges and corners more sensitive than coupon centers under cycling?
6. Does thermal trend drift suggest hidden internal degradation before visible collapse?

---

## Candidate Set for V3

V3 is built from survivors of earlier stages.

### Required coupon families

#### V3-B1
**HTZ-01-only cycling baseline**

Intent:
- determine how the exposed-face family behaves under repeated thermal cycling without layered support

#### V3-B2
**HTZ-01 + selected OX-02 baseline**

Intent:
- determine how the chosen transition-supported pair behaves under repeated cycling

#### V3-C1
**HTZ-01 + selected OX-02 + SD-03 candidate A**

Intent:
- first decoupled layered comparison under cycling

#### V3-C2
**HTZ-01 + selected OX-02 + SD-03 candidate B or alternate decoupling implementation**

Intent:
- avoid overcommitting to one arbitrary decoupling implementation

---

### Optional comparison families

#### V3-R1
**HTZ-01 + simplified transition or simplified decoupling comparison**

Intent:
- determine whether the primary layered logic is overly complex relative to simpler cycling behavior

#### V3-R2
**Rigid-stack comparison coupon**

Intent:
- provide a deliberately less forgiving comparison to expose the value of decoupling logic more clearly

Reserve comparisons are allowed only if they sharpen the answer instead of diluting it.

---

## Candidate Naming Rule

The repo may refer to V3 coupons using the following identifiers:

- V3-B1
- V3-B2
- V3-C1
- V3-C2
- V3-R1
- V3-R2

Exact process and geometry details may live in later support artifacts, but the stage must remain readable through stable IDs.

---

## Coupon Philosophy

The V3 coupon philosophy is:

- compare repeated-cycle behavior, not one-time hero behavior
- track deterioration trend rather than only final state
- include at least one rigid or reduced-decoupling comparison
- preserve visibility into edge, corner, and interface effects
- judge the layered concept by whether it remains coherent after thermal repetition

V3 is not only about surviving the first cycle.  
It is about how the stack changes from cycle to cycle.

---

## What V3 Is Trying to Prove

V3 is trying to prove only the following:

1. The selected layered direction remains coherent under repeated thermal cycling.
2. The combination of HTZ-01 + OX-02 does not collapse under early reuse-like thermal repetition.
3. Early SD-03 logic improves cycling survivability relative to more rigid comparisons.
4. The architecture’s thermo-structural thesis remains alive after repeated heat events.
5. The repo can justify moving into more aggressive mismatch and high-heat stages.

---

## What V3 Is Trying to Disprove

V3 is trying to disprove any of the following bad outcomes:

1. The selected layered direction only looks good in single-event logic.
2. OX-02 becomes a cycling-driven brittle plane.
3. SD-03 adds complexity without reducing real cycling damage.
4. Cracking or edge failure accelerates too quickly for the intended mission posture.
5. Limited-reuse language is already too optimistic.
6. The stack becomes less interpretable with each cycle instead of more informative.

---

## Planned Cycling Logic

The exact thermal-cycle hardware and profile are not frozen in v0.1, but V3 requires a repeated heating and cooldown sequence severe enough to reveal:

- crack initiation
- crack growth
- interfacial damage progression
- edge and corner sensitivity
- damage accumulation rate
- drift in thermal behavior between cycles

V3 is not trying to reproduce the entire final mission environment.

It is trying to reveal whether the layered architecture is fundamentally honest under repetition.

---

## Planned Observation Set

At minimum, V3 should eventually capture the following.

### O1 — Pre-test coupon identity
- coupon ID
- layer stack ID
- candidate-family traceability
- geometry notes

### O2 — Baseline condition
- initial visual condition
- initial mass
- initial thickness / representative geometry
- initial edge and corner condition
- initial interface documentation where feasible

### O3 — Per-cycle visible condition
- crack appearance
- crack growth
- edge or corner chipping
- surface-state evolution
- visible warping or delamination cues

### O4 — Per-cycle thermal trend if instrumented
- trend in thermal response between cycles
- signs of increasing heat leakage
- signs of deteriorating thermal performance

### O5 — Post-test condition
- cumulative cracking
- layer separation
- geometry change
- mass change
- final visible integrity state

### O6 — Comparative ranking notes
- better / similar / worse than baseline
- better / similar / worse than rigid comparison
- bounded / unstable / unacceptable degradation behavior

The point is to reveal progression, not just the final wreckage.

---

## Minimum Evaluation Questions per Coupon Family

Each V3 coupon family should be judged against the following questions.

### Q1
Did the coupon remain grossly intact across the planned cycle set?

### Q2
Did cracking remain bounded or did it accelerate rapidly?

### Q3
Did the edge and corner behavior remain credible relative to the center?

### Q4
Did the transition layer remain coherent under cycling?

### Q5
Did the decoupling layer improve cycling behavior relative to a more rigid comparison?

### Q6
Did thermal behavior drift in a way that suggests growing hidden damage?

### Q7
Is this coupon family still worth carrying into V4 and V5?

If the answer set is mostly no, that family should be downgraded or cut.

---

## Stage-Level Pass Conditions

V3 passes only if all of the following are true:

1. At least one layered coupon family remains coherent across repeated thermal cycles.
2. The selected HTZ-01 + OX-02 direction does not reveal obvious early cycle-instability that invalidates continued use.
3. SD-03 logic, if included, shows a credible cycling-survivability benefit or at minimum does not clearly worsen the architecture.
4. The results support continued progression to V4 and V5.
5. The repo can explain how the cycle results changed or refined the stack assumptions.

---

## Stage-Level Fail Conditions

V3 fails if any of the following occur:

1. The layered direction degrades too rapidly to support the intended mission posture.
2. OX-02 or SD-03 repeatedly becomes a cycling-driven weak plane.
3. Rigid or simpler comparisons perform as well or better in a way that undermines the current layered thesis.
4. Edge/corner failure dominates so strongly that the architecture must be rethought before proceeding.
5. The stage cannot distinguish better from worse candidates honestly.

If V3 fails, the stack must be simplified, narrowed, or revised before V4 or V5.

---

## V3 Keep / Cut Logic

### Keep the layered direction if:
- at least one layered family remains coherent across the cycle set
- damage stays more bounded than in rigid comparisons
- the results strengthen the case for continued decoupling and transition logic

### Downgrade the layered direction if:
- some value remains, but the reuse/limited-reuse posture now looks too optimistic
- decoupling or transition logic helps only marginally
- a simpler stack is beginning to look more credible

### Cut or restructure the layered direction if:
- repeated cycling reveals fundamental instability
- rigid or reduced-complexity comparisons undermine the current thesis
- the stack loses coherence faster than it earns its complexity

---

## Controls and Baselines

V3 must not run without the following comparison posture:

- HTZ-01-only cycling baseline
- HTZ-01 + OX-02 layered baseline
- at least one SD-03-inclusive comparison
- at least one more rigid or simplified comparison if feasible

Without those controls, V3 cannot honestly answer whether decoupling and layering are improving cyclic survivability.

---

## V3 Risk Focus

The main risks V3 is trying to expose are:

- cycling-induced brittle failure
- repeated thermal mismatch damage
- early edge or corner fragility
- transition-layer degradation under repetition
- decoupling logic that does not survive repeated use
- false confidence from single-event success
- drift in thermal behavior that reveals hidden internal damage

If V3 does not expose those risks, it is not doing its job.

---

## What V3 Does Not Prove

Even if V3 succeeds, it does **not** prove:

- full attachment survivability
- final carrier adequacy
- integrated insert behavior
- AR-05 value
- IR-06 value
- full seam-system validity
- high-heat severe-environment maturity
- flight relevance

V3 is a cycling-honesty stage only.

---

## Data Package Required from V3

When V3 is eventually executed, the stage should produce a data package that includes:

- coupon roster
- cycle profile definition
- per-cycle or staged observation record
- pre/post imagery
- mass and geometry notes
- damage trend summary
- comparative ranking summary
- justification for candidates advanced to V4 / V5

If that package does not exist, V3 has not really been completed.

---

## V3 Exit Decisions

At the end of V3, only the following decisions are valid.

### D1 — Advance layered survivors to V4 and V5
Use when one or more coupon families remain credible under cycling.

### D2 — Narrow the reuse / limited-reuse posture
Use when the layered direction remains interesting but cycling damage is more severe than hoped.

### D3 — Simplify the stack before V4 / V5
Use when rigid or simpler comparisons begin to look more credible.

### D4 — Repeat V3 with corrected coupon logic
Use when the comparison setup failed to isolate the real question.

### D5 — Branch to revised reference configuration
Use when cycling behavior reveals a deeper contradiction in Max-01.

---

## Relationship to Other Modules

This stage depends on:
- `reference-configs/max-01.md`
- `modules/thermo-structural-budget.md`
- `modules/risk-failure-register.md`
- the V1 and V2 survivor logic

This stage informs:
- V4 attachment / mismatch stack planning
- V5 high-heat coupon exposure planning
- future reuse-boundary decisions
- future SD-03 narrowing decisions

---

## V3 Summary

V3 is the stage where IX-HfTaZen-Shield asks whether its layered architecture is real under repetition or only attractive in a single event.

If the selected layered direction cannot remain coherent across thermal cycling, it does not deserve to carry reuse or limited-reuse ambition forward.
