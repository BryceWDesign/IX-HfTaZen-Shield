# Materials Screening

## Module Purpose

This module defines the **v0.1 material screening logic** for IX-HfTaZen-Shield.

Its job is to answer:

1. what material families are being considered for each layer
2. why those families are being considered
3. what screening criteria decide whether a family stays or gets cut
4. which families are primary, secondary, reserve, or excluded
5. what assumptions are still analytical rather than measured

This module does **not** claim that the selected materials are validated in the IX-HfTaZen-Shield stack.

It freezes the **screening direction** for v0.1.

---

## Screening Rule

A material family is only useful to this program if it improves the localized extreme-heat TPS problem **as a system**.

That means a candidate is judged against more than nominal peak temperature.

A family survives screening only if it is at least plausibly useful for the intended role when considering:

- high-temperature survivability
- oxidation behavior
- thermal reradiation potential
- thermal conductivity implications
- interface compatibility
- thermo-structural mismatch risk
- segmentation suitability
- joint/edge survivability
- analytical coherence with the Max-01 stack
- ability to fit a coupon-to-subscale validation path

If a candidate looks impressive only in isolation but becomes a stack liability, it does not survive screening.

---

## Screening Structure

Material screening is organized by layer role:

1. HTZ-01 Radiative UHTC Face
2. OX-02 Oxidation-Control Transition
3. SD-03 Strain-Decoupling Interlayer
4. TC-04 Thermal Choke Carrier
5. AR-05 Active Relief Branch
6. IR-06 Thermal Intercept & Recovery Cassette
7. HB-07 Health-Monitoring Backplane
8. SJ-08 Seal & Joint Management Ring

Each layer has:
- primary candidate family
- secondary candidate families
- reserve candidates
- excluded directions
- screening rationale

---

## Global Screening Criteria

The following criteria apply to all material families.

### G1 — Layer-role fit
A candidate must make sense for the exact layer role it is assigned to.

### G2 — Oxidizing-environment credibility
Because v0.1 assumes an oxidizing baseline environment, candidates that only look strong in inert or vacuum conditions are not enough on their own.

### G3 — Interface realism
A candidate must not require perfect interfaces, perfect monoliths, or zero mismatch to remain plausible.

### G4 — Localized insert compatibility
Candidates must remain coherent in segmented small-area inserts with edges, seams, and attachment realities.

### G5 — Testability
A candidate must support a coupon-to-subscale validation logic.

### G6 — No miracle-material thinking
A candidate that is only attractive because of one extreme property but creates severe weakness elsewhere will be downgraded or excluded.

### G7 — Stack discipline
No candidate may force the architecture away from passive-first localized TPS into uncontrolled whole-system complexity without a strong reason.

---

## HTZ-01 Radiative UHTC Face

## Role Summary

HTZ-01 is the exposed hot face.

Its required traits are:

- very high thermal capability
- strong reradiative potential
- better oxidizing-environment promise than simpler one- or two-component UHTC directions
- compatibility with segmentation
- compatibility with buried oxidation-control and decoupling layers

---

## HTZ-01 Primary Candidate Family

### Primary
**Hf-rich high-entropy carbide / carbonitride**
within the **Hf–Ta–Zr–W–(C,N)** design lane

### Why this family is primary
This family is screened as primary because it best aligns with the v0.1 objective:

- keeps the hot face in the serious UHTC regime
- stays closer to the strongest current oxidation-resistant refractory ceramic direction identified for this repo
- allows tuning across more than a simple binary carbide
- supports the design philosophy of building a stack around real oxidizing limits rather than just nominal peak-temperature bragging

### Primary screening intent
The primary hot-face direction is not a single exact composition claim.

It is a **design lane** anchored by:
- hafnium-rich thermal ceiling logic
- tantalum participation for strong refractory UHTC behavior
- zirconium for broader high-entropy ceramic design space
- tungsten in controlled proportion for refractory stabilization logic
- carbonitride tuning rather than pure carbide-only dogma

---

## HTZ-01 Secondary Candidate Families

### Secondary A
**Hf–Ta–(C,N)** focused carbide / carbonitride lane

Why kept:
- simpler than the primary lane
- useful as a reduced-complexity comparison baseline
- helps determine whether the full high-entropy direction is actually buying enough to justify itself

### Secondary B
**HfC / TaC / Ta-Hf carbide solid-solution family**

Why kept:
- strong reference baseline for comparison
- useful as a control family in screening logic
- historically central to UHTC discussion

### Secondary C
**Hf–Zr–Ta carbide family without W**

Why kept:
- useful to isolate whether tungsten participation is helping or complicating the design lane
- lower-complexity comparison against the primary family

---

## HTZ-01 Reserve Candidate Families

### Reserve A
**Hf–Zr carbonitride lane**

Why reserved:
- may be useful if Ta/W participation causes interface or processing concerns
- remains in the serious refractory ceramic space

### Reserve B
**Ta-rich UHTC lane**

Why reserved:
- useful as a comparison branch
- not preferred as the primary direction because the repo is biased toward the strongest Hf-led ceiling logic

---

## HTZ-01 Excluded or Downgraded Directions

### Excluded X1
**Pure tungsten exposed hot face**

Reason:
- not rejected as a refractory material in general
- rejected as the primary exposed-face answer because the repo is not building a simple refractory metal wall and does not want the hot face defined by metal-led oxidation and thermal behavior

### Excluded X2
**Diamond / graphite / exposed carbon-rich front face**

Reason:
- incompatible with the oxidizing baseline logic for this repo
- wrong design direction for a reusable exposed front face in this concept

### Excluded X3
**Low-temperature ceramics framed as oxidation coatings for the main face**

Reason:
- insufficient hot-face ambition
- may still matter elsewhere in the stack, but not here

### Downgraded X4
**Single-number “highest melting material wins” logic**

Reason:
- the hot-face problem is not solved by a single peak-temperature talking point

---

## HTZ-01 Screening Questions

A hot-face candidate survives only if it can answer yes to most of these:

- does it remain plausible in an oxidizing high-heat environment?
- does it fit a segmented insert architecture?
- does it pair coherently with a buried oxidation-control layer?
- does it avoid creating impossible mismatch demands on the support stack?
- does it remain worthy of coupon comparison against simpler controls?
- does it preserve the passive-first logic before active relief is considered?

---

## OX-02 Oxidation-Control Transition

## Role Summary

OX-02 is the buried oxidation-control and chemistry-transition layer.

Its required traits are:

- help reduce oxygen-driven interfacial damage
- support the hot-face chemistry rather than fight it
- remain more than a cosmetic coating concept
- avoid becoming a brittle penalty layer

---

## OX-02 Primary Candidate Family

### Primary
**HfSiCN-class oxidation-control transition**

### Why this family is primary
This family best fits the intended role because:
- it supports a buried oxidation-management function
- it offers a chemistry bridge between ultra-hot face logic and deeper stack survivability
- it aligns with the design decision not to force the outer face and oxidation-control strategy to be the same exact material problem

---

## OX-02 Secondary Candidate Families

### Secondary A
**Hf-based silicon-bearing transition ceramics**

Why kept:
- useful if the HfSiCN framing needs a broader family treatment

### Secondary B
**Si-bearing refractory oxidation-control interlayers**

Why kept:
- comparison lane to check whether the Hf-specific direction is truly necessary at this layer

---

## OX-02 Excluded or Downgraded Directions

### Excluded X1
**Treating OX-02 as the main exposed hot face**

Reason:
- violates the stack logic
- collapses the separation between radiative hot-face role and buried oxidation-control role

### Downgraded X2
**Glass-like or soft oxidation-control logic without mechanical realism**

Reason:
- the transition layer cannot survive as an idea only
- it must remain coherent under thermal gradients and structural constraint

---

## OX-02 Screening Questions

- does the layer improve buried-interface oxidation logic?
- does it remain coherent beneath the hot face?
- does it avoid becoming a brittle crack-initiation penalty?
- does it fit a coupon comparison against no-transition baselines?

---

## SD-03 Strain-Decoupling Interlayer

## Role Summary

SD-03 is the thermo-structural damage-mitigation layer.

Its required traits are:

- reduce transmitted mismatch stress
- allow segmented inserts to move without instantly punishing the hot face
- avoid becoming a weak collapse layer
- avoid becoming a hidden thermal short

---

## SD-03 Primary Candidate Family

### Primary
**Refractory compliant interlayer architecture**
using one or more of the following concept classes:
- refractory mesh
- refractory felt
- compliant porous refractory layer
- refractory foil-based decoupling concept
- other high-temperature compliant structures

### Why this family is primary
The layer is defined by **function first**, not by one exact chemistry at v0.1.

This layer survives screening if it can plausibly:
- broaden stress transfer
- reduce hard restraint
- survive the local thermal gradient environment
- integrate with the carrier without becoming a slippage or collapse disaster

---

## SD-03 Secondary Candidate Families

### Secondary A
**Engineered porosity decoupling layer**

Why kept:
- useful if porosity can provide compliance while preserving thermal and structural logic

### Secondary B
**Thin refractory foil decoupling layer**

Why kept:
- useful if mesh/felt concepts overcomplicate the layer

---

## SD-03 Excluded or Downgraded Directions

### Excluded X1
**Low-temperature polymeric or STF-style decouplers**

Reason:
- incompatible with the thermal envelope

### Excluded X2
**Rigid hard-bond-only architecture with no decoupling logic**

Reason:
- contradicts the structural posture of Max-01

### Downgraded X3
**Overly soft layers with no support credibility**

Reason:
- compliance is not enough by itself
- the layer must still carry its place in a serious stack

---

## SD-03 Screening Questions

- does it reduce mismatch stress in principle?
- does it survive the intended thermal envelope better than low-temp alternatives?
- does it avoid becoming a severe thermal short?
- does it support segmented inserts more credibly than hard-bond baselines?

---

## TC-04 Thermal Choke Carrier

## Role Summary

TC-04 provides structural support and thermal-flow moderation.

Its required traits are:

- support segmented inserts
- avoid acting like a direct heat dump into deeper structure
- remain compatible with SD-03
- allow instrumentation and boundary definition

---

## TC-04 Primary Candidate Family

### Primary
**Refractory or ceramic-compatible segmented carrier architecture**

This is intentionally left at the family level in v0.1.

It may include:
- refractory support concepts
- ceramic-compatible support concepts
- hybrid carrier concepts
- geometry-driven thermal choke architectures

### Why this family is primary
The carrier should not be prematurely over-fixed before the stress, thermal, and instrumentation logic are all frozen.

The key is function:
- carry the insert
- avoid thermal sabotage
- integrate with SD-03 and SJ-08
- remain compatible with validation articles

---

## TC-04 Secondary Candidate Families

### Secondary A
**Ceramic-dominant carrier**

Why kept:
- useful if metal-heavy carrier logic proves too thermally aggressive

### Secondary B
**Refractory-alloy-assisted carrier**

Why kept:
- useful if ceramic-only carrier logic proves too brittle or hard to instrument

---

## TC-04 Excluded or Downgraded Directions

### Excluded X1
**Highly conductive carrier that bypasses the thermal choke purpose**

Reason:
- defeats the architecture

### Downgraded X2
**Carrier chosen only for structural strength with no thermal penalty accounting**

Reason:
- wrong design priority for this stack

---

## AR-05 Active Relief Branch

## Role Summary

AR-05 is the local-only severe-hotspot branch.

Its required traits are:

- only activate where the passive wall approaches its credible limit
- deliver meaningful local thermal relief
- avoid forcing broad-area active cooling dependence
- remain bounded and testable

---

## AR-05 Primary Candidate Family

### Primary
**Porous-UHTC local transpiration-style relief**

### Why this family is primary
This is the cleanest local-only active concept for the current repo because:
- it directly addresses local heat burden
- it stays closest to the severe-hotspot problem
- it fits the logic of an insert-level exceptional branch

---

## AR-05 Secondary Candidate Families

### Secondary A
**Refractory heat-pipe local intercept**

Why kept:
- strong local hotspot management logic
- useful as a comparison against transpiration-style relief

### Secondary B
**Tightly bounded local heat-spreading branch**

Why kept:
- reserve option if other active branches become too complex

---

## AR-05 Excluded or Downgraded Directions

### Excluded X1
**Broad-area active cooling shell**

Reason:
- outside mission envelope

### Excluded X2
**Peltier-style front-line TPS cooling**

Reason:
- wrong scale and wrong physics for the targeted heat burden

### Downgraded X3
**Any active branch with no clear local gating criterion**

Reason:
- active features must stay bounded

---

## IR-06 Thermal Intercept & Recovery Cassette

## Role Summary

IR-06 is the secondary downstream heat-to-power branch.

Its required traits are:

- only consume controlled intercepted heat
- remain downstream of survival-critical thermal protection
- produce bounded useful power if present
- never drive harmful heat leakage

---

## IR-06 Primary Candidate Family

### Primary
**TPV-first recovery architecture**

### Why this family is primary
The repo chooses TPV-first because:
- it is more serious for high-temperature thermal streams than ordinary “ambient harvester” logic
- it better fits a controlled thermal intercept path
- it aligns with the repo’s decision to treat energy recovery as a secondary, engineered function

---

## IR-06 Secondary Candidate Families

### Secondary A
**TEG tail-stage recovery**

Why kept:
- useful at lower downstream temperatures
- useful as a secondary stage after a hotter primary converter

### Secondary B
**Non-flight bench-only heat-engine comparison lane**

Why kept:
- useful for analytical comparison
- not part of the baseline integrated stack

---

## IR-06 Excluded or Downgraded Directions

### Excluded X1
**Ambient harvester field under the shield as primary relief**

Reason:
- violates the thermal logic of the stack

### Excluded X2
**Energy-first stack design**

Reason:
- TPS survives first, converts second

### Downgraded X3
**Recovery branch that requires intentional extra thermal leakage**

Reason:
- self-defeating for TPS

---

## HB-07 Health-Monitoring Backplane

## Role Summary

HB-07 is the observability layer.

Its required traits are:

- survive enough to measure what matters
- avoid becoming the weak thermal link
- support thermal and mechanical awareness
- preserve post-test interpretability

---

## HB-07 Primary Candidate Family

### Primary
**High-temperature-compatible sensing backplane architecture**

This may include concept classes such as:
- temperature sensing
- strain/displacement awareness
- thermal leakage detection
- anomaly logging paths

### Why this family is primary
The exact instrumentation stack is not frozen in v0.1, but the function is mandatory.

---

## HB-07 Excluded or Downgraded Directions

### Excluded X1
**Blind stack with no observability**

Reason:
- incompatible with the program thesis

### Downgraded X2
**Instrumentation that creates major thermal shorts**

Reason:
- sensing must not destroy the thing being sensed

---

## SJ-08 Seal & Joint Management Ring

## Role Summary

SJ-08 manages seams, insert edges, and local boundary survival.

Its required traits are:

- support segmented insert boundaries
- reduce oxidation ingress at boundaries
- reduce edge-spall risk
- tolerate local movement and mismatch

---

## SJ-08 Primary Candidate Family

### Primary
**Refractory-compatible joint / edge management architecture**

This is treated as a function-first layer family in v0.1.

Possible concept classes include:
- refractory edge shields
- seam-control geometries
- compliant boundary features
- oxidation-aware edge treatments

---

## SJ-08 Excluded or Downgraded Directions

### Excluded X1
**Undefined joints deferred to later**

Reason:
- architecture failure usually starts where design discipline stops

### Excluded X2
**Soft low-temperature seam materials**

Reason:
- incompatible with mission envelope

---

## Cross-Layer Screening Matrix

A candidate direction rises in priority if it helps multiple truths at once:

- supports oxidizing-environment survival
- supports segmented insert geometry
- reduces interface risk
- preserves passive-first logic
- remains instrumentable
- fits coupon and subscale validation

A candidate direction falls in priority if it:

- relies on vacuum-only hero behavior
- requires broad active cooling
- worsens structural mismatch
- increases uncontrolled interior heat leakage
- makes seams/joints less credible
- cannot be tested in a staged way

---

## v0.1 Primary Screening Outcome

The current v0.1 screening outcome is:

### Locked primary directions
- **HTZ-01:** Hf-rich Hf–Ta–Zr–W–(C,N) high-entropy carbide / carbonitride lane
- **OX-02:** HfSiCN-class oxidation-control transition
- **SD-03:** refractory compliant interlayer architecture
- **TC-04:** refractory or ceramic-compatible segmented carrier
- **AR-05:** porous-UHTC local transpiration-style relief
- **IR-06:** TPV-first thermal intercept and recovery
- **HB-07:** high-temperature-compatible sensing backplane
- **SJ-08:** refractory-compatible joint and edge management architecture

### Locked comparison lanes
- reduced-complexity Hf–Ta–(C,N)
- HfC / TaC / Ta-Hf baseline lane
- Hf–Zr–Ta lane without W
- AR-05 heat-pipe comparison lane
- IR-06 TEG tail-stage comparison lane

---

## v0.1 Materials Screening Summary

The repo is not selecting “the hottest thing possible.”

It is selecting material **families by role**.

That is the core correction.

The v0.1 materials-screening posture is:

- hot face chosen for serious refractory thermal ambition
- oxidation control chosen separately
- stress decoupling treated as its own material problem
- carrier chosen for support without hidden thermal sabotage
- active branch tightly bounded
- energy branch strictly downstream and secondary
- sensing and joints treated as material/system problems too

That is the frozen screening logic for v0.1.
