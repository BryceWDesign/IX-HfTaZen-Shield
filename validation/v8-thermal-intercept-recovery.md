# V8 Thermal Intercept & Recovery Demonstrator

## Stage Identity

**Stage:** V8  
**Name:** Thermal Intercept & Recovery Demonstrator  
**Program:** IX-HfTaZen-Shield  
**Reference configuration:** Max-01  
**Primary architecture branch under test:** IR-06 Thermal Intercept & Recovery Cassette  
**Evidence tier target if later executed:** bounded E3-to-E4 bridge evidence depending on demonstrator fidelity  
**Execution status:** planned / frozen for v0.1  
**Purpose:** determine whether a downstream thermal intercept and recovery cassette can extract bounded secondary value from a controlled intercepted heat stream without harming the thermal-protection mission

---

## Stage Purpose

V8 exists because the repo made a very specific promise:

- energy recovery is secondary
- energy recovery is downstream
- energy recovery must not justify harmful leak-through
- energy recovery must be removable
- energy recovery must never become the reason the architecture exists

That means IR-06 does not get to survive on interesting math alone.

V8 is the stage where IX-HfTaZen-Shield forces IR-06 to answer the hard question:

> Can a downstream recovery cassette extract bounded useful power from a controlled intercepted heat stream without worsening the thermal-protection architecture?

If the answer is no, IR-06 gets cut.

---

## What V8 Is Testing

V8 is testing whether a **controlled intercepted thermal stream** can support bounded secondary energy conversion honestly.

The stage focuses on:

- a controlled intercepted heat source justified by thermal-protection logic
- a downstream IR-06-style cassette
- recovery efficiency and residual-heat accounting
- the thermal and architectural consequences of integrating the cassette

V8 is not testing:

- ambient scavenger fantasies
- broad-area leak-fed harvesting
- energy-first thermal architecture
- primary survival by power generation

It is a downstream sidecar truth stage.

---

## Why V8 Matters

A recovery branch is easy to oversell.

Numbers can look attractive if the repo stops asking:

- where did the heat come from?
- why was that heat there?
- how much was intercepted for protection reasons first?
- how much residual heat remains after recovery?
- did the backface burden get worse?
- did the cassette make the stack more complex than it was worth?

V8 exists to force those questions into one bounded stage.

---

## V8 Test Objective

The objective of V8 is to determine whether IR-06 can:

1. operate only on a controlled intercepted heat stream
2. produce nontrivial bounded electric output
3. preserve protection-first architecture logic
4. account honestly for residual heat
5. remain removable and secondary
6. justify continuation into integrated insert logic

---

## Primary Question

The primary V8 question is:

> Can IR-06 extract bounded secondary electrical value from a controlled intercepted stream without creating a worse thermal or integration penalty than the value it provides?

---

## Secondary Questions

V8 also asks:

1. Does TPV-first recovery remain the most credible recovery concept for this architecture?
2. Does the cassette worsen backface or downstream burden even if electric output looks useful?
3. Does the residual heat remain manageable after conversion?
4. Does the recovery branch stay downstream and modular in practice, not just on paper?
5. Would the architecture still make sense if IR-06 were removed?
6. Is the recovery branch worth carrying relative to its added complexity?

---

## Candidate Set for V8

### Required demonstrator families

#### V8-B0
**Controlled intercepted thermal stream with no recovery cassette**

Intent:
- preserve a thermal-only baseline for comparison

#### V8-I1
**TPV-first recovery cassette demonstrator**

Intent:
- primary IR-06 concept class
- measure bounded electric recovery from a controlled intercepted stream

#### V8-I2
**TPV-first cassette with alternate configuration or operating point**

Intent:
- avoid overcommitting to one arbitrary cassette implementation

---

### Optional demonstrator families

#### V8-R1
**TEG tail-stage or lower-temperature recovery comparison**

Intent:
- determine whether a secondary lower-grade tail stage adds enough value to matter

#### V8-R2
**Alternate recovery geometry or modularity comparison**

Intent:
- determine whether the recovery cassette can remain more removable and less invasive

Reserve demonstrators are allowed only if they sharpen the keep / cut decision.

---

## Candidate Naming Rule

The repo may refer to V8 demonstrators using the following identifiers:

- V8-B0
- V8-I1
- V8-I2
- V8-R1
- V8-R2

Detailed emitter, cassette, and routing specifics may live in later support artifacts, but the stage must remain readable through stable IDs.

---

## Demonstrator Philosophy

The V8 philosophy is:

- define the intercepted thermal source clearly
- compare recovery against a no-recovery thermal baseline
- count residual heat honestly
- treat protection-first logic as nonnegotiable
- ask whether the cassette earns its place or is just clever excess

V8 is not a power-generation celebration stage.

It is a protection-discipline stage with energy accounting attached.

---

## Controlled Thermal Source Rule

A V8 demonstrator is valid only if the intercepted heat source is:

1. defined
2. bounded
3. already justified for protection reasons
4. upstream-independent of IR-06
5. compatible with the architecture even if IR-06 is removed

If the source does not satisfy those rules, the V8 result is invalid for Max-01.

---

## Recovery Accounting Rule

Every V8 demonstrator must define:

- intercepted thermal input `Q_intercept`
- assumed or measured electric output `P_electric`
- residual heat `Q_residual`
- cassette location
- whether the cassette altered the downstream thermal burden

Without that accounting, the stage is not engineering.

---

## What V8 Is Trying to Prove

V8 is trying to prove only the following:

1. A downstream recovery cassette can extract bounded useful power from a controlled intercepted stream.
2. The cassette remains clearly secondary to the thermal-protection mission.
3. The cassette does not reward harmful leak-through.
4. Residual heat accounting remains honest and manageable.
5. The repo can explain whether IR-06 deserves continuation or removal.

---

## What V8 Is Trying to Disprove

V8 is trying to disprove any of the following bad outcomes:

1. IR-06 only looks good because the source-stream accounting is loose.
2. Recovery output is not meaningful enough to justify the integration burden.
3. The cassette worsens the thermal-protection function.
4. The cassette becomes the reason intercepted heat is routed inward at all.
5. The recovery branch survives only by becoming too central or too invasive.
6. The branch is more conceptually attractive than architecturally useful.

---

## Planned Observation Set

At minimum, V8 should eventually capture the following.

### O1 — Demonstrator identity
- demonstrator ID
- cassette concept ID
- intercepted-stream definition ID
- no-recovery baseline ID

### O2 — Thermal-source definition
- source location
- intercepted thermal burden
- operating condition
- routing logic
- downstream baseline state

### O3 — Recovery observations
- electrical output
- output stability or trend
- thermal input to cassette
- thermal-to-electric conversion interpretation

### O4 — Residual-heat observations
- downstream heat that remained after conversion
- whether the backface burden changed
- whether the cassette introduced new thermal concentration

### O5 — Integration observations
- structural or routing penalties
- modularity / removability cues
- whether the cassette appeared overly invasive

### O6 — Comparative ranking notes
- better / similar / worse than no-recovery baseline from a total-architecture perspective
- bounded / marginal / unjustified recovery value classification

The purpose is to reveal total-system honesty, not only electrical output.

---

## Minimum Evaluation Questions per Demonstrator

Each V8 demonstrator should be judged against the following questions.

### Q1
Was the thermal source clearly controlled and already justified for protection reasons?

### Q2
Did the cassette produce bounded useful electrical output?

### Q3
Was residual heat accounted for honestly?

### Q4
Did the cassette avoid worsening the protected-side thermal burden?

### Q5
Did the cassette remain clearly removable and secondary?

### Q6
Did the total architecture look better with the cassette than without it?

### Q7
Is this recovery concept worth carrying forward?

If the answer set is mostly no, that concept should be cut.

---

## Stage-Level Pass Conditions

V8 passes only if all of the following are true:

1. At least one recovery cassette concept produces bounded useful electrical output.
2. The recovery concept remains downstream and secondary.
3. The total protection architecture is not worsened by the cassette.
4. Residual heat accounting remains explicit and credible.
5. The repo can explain clearly why the surviving recovery concept continues.

---

## Stage-Level Fail Conditions

V8 fails if any of the following occur:

1. No recovery concept produces enough secondary value to justify itself.
2. The cassette worsens the thermal-protection function.
3. The cassette survives only by relying on harmful leak-through or vague source accounting.
4. The branch becomes too central or invasive for Max-01 discipline.
5. The stage cannot distinguish useful recovery from complexity-driven noise.

If V8 fails, IR-06 must be cut or radically narrowed before integrated-stage use.

---

## V8 Keep / Cut Logic

### Keep IR-06 if:
- at least one recovery concept produces bounded useful secondary value
- the concept remains downstream and removable
- the total protection architecture remains healthier with the concept than without it

### Downgrade IR-06 if:
- the concept works only in a narrower intercepted-stream regime than hoped
- the cassette remains interesting but the output-to-complexity ratio is weak
- only a very limited modular use case survives

### Cut IR-06 if:
- the cassette does not justify itself honestly
- the cassette worsens protection
- the cassette rewards harmful thermal leakage
- the cassette only survives by becoming too central to the architecture

---

## Controls and Baselines

V8 must not run without the following comparison posture:

- a no-recovery intercepted-stream baseline
- at least one primary recovery concept
- explicit intercepted-stream accounting
- explicit residual-heat accounting
- comparison of total architecture effect, not just electric output

Without these controls, V8 becomes an energy demo rather than a TPS truth stage.

---

## V8 Risk Focus

The main risks V8 is trying to expose are:

- leak-seeking recovery logic
- residual heat trap
- oversold electric output
- protection inversion
- cassette complexity bloat
- false belief that conversion equals cooling success

If V8 does not expose those risks, it is not doing its job.

---

## What V8 Does Not Prove

Even if V8 succeeds, it does **not** prove:

- full integrated insert maturity
- final mission usefulness
- final operability
- flight relevance
- architecture-wide energy recovery viability

V8 is the downstream recovery truth stage only.

---

## Data Package Required from V8

When V8 is eventually executed, the stage should produce a data package that includes:

- demonstrator roster
- source-stream definition
- recovery and residual-heat accounting
- pre/post imagery where relevant
- thermal observations
- electrical output observations
- comparative ranking summary
- keep / cut recommendation for IR-06

If that package does not exist, V8 has not really been completed.

---

## V8 Exit Decisions

At the end of V8, only the following decisions are valid.

### D1 — Keep IR-06 as an optional bounded downstream cassette
Use when at least one recovery concept survives honestly.

### D2 — Narrow IR-06 to a tighter intercepted-stream use case
Use when the cassette works, but only under a more limited regime than originally hoped.

### D3 — Replace the preferred IR-06 concept class
Use when one recovery concept fails and another proves more credible.

### D4 — Cut IR-06 from Max-01
Use when the cassette does not justify itself honestly.

### D5 — Branch to revised reference configuration
Use when V8 reveals that Max-01 wants a different multifunction architecture than originally allowed.

---

## Relationship to Other Modules

This stage depends on:
- `reference-configs/max-01.md`
- `modules/thermal-intercept-recovery.md`
- `modules/risk-failure-register.md`
- V7 source-stream logic where relevant

This stage informs:
- V9 integrated insert planning
- future IR-06 keep / cut decisions
- future multifunction-architecture narrowing

---

## V8 Summary

V8 is the stage where IX-HfTaZen-Shield forces its energy-recovery ambition to justify itself honestly.

If IR-06 cannot extract bounded useful value from a controlled intercepted stream without harming the thermal-protection architecture, it does not deserve to remain in Max-01.
