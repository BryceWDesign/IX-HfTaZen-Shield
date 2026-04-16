# Thermo-Structural Budget

## Module Purpose

This module defines the **first-pass thermal and thermo-structural budgeting logic** for IX-HfTaZen-Shield v0.1.

Its job is to answer:

1. what thermal loads the Max-01 configuration is analytically built around
2. how the stack is expected to distribute thermal burden by layer role
3. where the passive stack begins to run out of credible margin
4. why thermo-structural mismatch is a first-order design problem
5. what must later be measured to determine whether the analytical budget was useful or wrong

This module does **not** claim measured thermal or structural performance for Max-01.

It freezes the analytical budget posture for v0.1.

---

## Governing Rule

IX-HfTaZen-Shield is not designed by asking only:

> “What is the hottest material?”

It is designed by asking:

- what heat burden reaches the exposed face
- how much can be reradiated
- how much threatens to move deeper into the stack
- where oxidation and geometry change alter that behavior
- how much mismatch strain the stack generates while trying to survive
- whether the support and joint architecture can remain coherent while the thermal gradient exists

This means the program uses a **thermo-structural budget**, not a material brag sheet.

---

## Budget Philosophy

The Max-01 budget is built around five principles.

### 1. Exposed-face temperature is not the only temperature that matters
A concept can fail at:
- the hot-face/subsurface interface
- the decoupling layer
- the carrier
- the joint ring
- the backface

without ever “melting” at the exposed face.

### 2. Thermal success is layered
A good stack does not ask one layer to do everything.

### 3. Structural success is thermal-path dependent
The thermal gradient and restraint pattern help determine where the structure fails.

### 4. Passive margin must be explicit
If a zone needs active relief, that should be admitted by the budget instead of hidden.

### 5. Every number in v0.1 is conditional
The budget uses analytical bands and first-pass assumptions, not validated operating data.

---

## Baseline Thermal Bands

The budget is frozen around the following local heat-flux bands.

### Band A — Baseline Passive Local Zone
**500–800 W/cm²**

Budget meaning:
- preferred passive-only localized design band
- expected to be the most credible passive target region for Max-01

### Band B — Stretched Passive Local Zone
**800–1000 W/cm²**

Budget meaning:
- aggressive passive region
- strong sensitivity to emissivity, oxidation state, interface behavior, and mismatch stress

### Band C — Assisted Local Hotspot Zone
**1000–1500 W/cm²**

Budget meaning:
- local-only severe hotspot region
- passive wall margin becomes thin enough that local active relief may be necessary
- this band is not treated as a broad-area operating condition

---

## First-Pass Radiative Balance Logic

The primary first-pass exposed-face estimate in v0.1 uses a simplified reradiative balance form:

q = εσT^4

Where:

- q = local incident heat flux at the exposed face
- ε = effective emissivity assumption for the exposed hot face
- σ = Stefan-Boltzmann constant
- T = absolute exposed-face temperature

This relation is used only as a **first-pass bounding tool**.

It does **not** capture all of the following:
- catalytic surface effects
- local flow complexity
- changing emissivity with damage
- conduction into deeper layers
- oxidation-induced surface evolution
- geometric concentration effects
- seam or edge behavior
- transient complexity
- active-relief interaction

It is still useful because it shows where a purely reradiative passive wall begins to crowd the credible oxidizing survivability region.

---

## Locked First-Pass Emissivity Assumption

For v0.1, the first-pass exposed-face analytical calculations use:

**ε = 0.85**

This is not a claim that the real exposed surface will permanently hold that value.

It is a bounded analytical assumption used to establish a credible reradiative target posture.

Any future measured or literature-supported revision must explicitly replace it.

---

## First-Pass Exposed-Face Temperature Estimates

Using the simplified reradiative balance and the locked emissivity assumption, the following first-pass estimates are frozen for v0.1.

### At 500 W/cm²
Estimated exposed-face temperature:
**~2918°C**

### At 800 W/cm²
Estimated exposed-face temperature:
**~3337°C**

### At 1000 W/cm²
Estimated exposed-face temperature:
**~3522°C**

### At 1200 W/cm²
Estimated exposed-face temperature:
**~3699°C**

### At 1500 W/cm²
Estimated exposed-face temperature:
**~3927°C**

These are **analytical exposed-face estimates only**.

They are not validated operating points.

They exist to show the shape of the thermal problem:
- Band A stays inside a more comfortable analytical passive region
- Band B pushes toward the edge of credible passive oxidizing-UHTC ambition
- Band C pushes into the zone where passive-only behavior becomes increasingly strained

---

## What These Estimates Mean

The first-pass numbers do **not** mean the stack can “handle” those heat fluxes just because the equation yields a temperature.

They mean:

- a reradiative exposed face in these bands must live in a very severe thermal regime
- oxidation and interface survivability likely dominate before simplistic peak-temperature rhetoric becomes useful
- as the local band approaches and exceeds the top of Band B, active local burden reduction becomes easier to justify
- the exposed-face temperature estimate is only one entry in the total budget

---

## Thermal Burden Distribution by Layer

The Max-01 thermal budget assumes the layers divide the thermal problem by function.

### HTZ-01 Radiative UHTC Face
Primary budget role:
- accept direct local heat load
- reradiate as much of that burden as possible
- resist severe exposed-face degradation long enough to preserve function

Thermal budget rule:
- HTZ-01 must carry the largest share of direct thermal burden

---

### OX-02 Oxidation-Control Transition
Primary budget role:
- protect the deeper interface region
- reduce interfacial chemical damage under severe hot-face operation

Thermal budget rule:
- OX-02 is not primarily a bulk heat sink
- it must support survivability without becoming a thermal sabotage layer

---

### SD-03 Strain-Decoupling Interlayer
Primary budget role:
- reduce the structural penalty created by thermal gradients
- limit mismatch-driven damage

Thermal budget rule:
- SD-03 may tolerate elevated temperature, but its main job is thermo-structural moderation rather than brute-force heat absorption

---

### TC-04 Thermal Choke Carrier
Primary budget role:
- slow deeper heat penetration
- support geometry and attachment
- prevent the lower stack from becoming a direct thermal dump path

Thermal budget rule:
- TC-04 must reduce deeper thermal transmission relative to a more conductive structural path

---

### AR-05 Active Relief Branch
Primary budget role:
- intercept or redistribute a bounded local thermal burden when passive margin becomes too thin

Thermal budget rule:
- AR-05 exists to shave peak local burden, not to become the normal state of the whole system

---

### IR-06 Thermal Intercept & Recovery Cassette
Primary budget role:
- accept a controlled intercepted thermal stream only after the protective stack has already done its main job

Thermal budget rule:
- IR-06 cannot be allowed to worsen upstream protection just to improve recovery output

---

### HB-07 Health-Monitoring Backplane
Primary budget role:
- measure surviving heat leakage and interface behavior

Thermal budget rule:
- HB-07 is where the stack admits what got through

---

### SJ-08 Seal & Joint Management Ring
Primary budget role:
- prevent edges and seams from becoming thermal and oxidation shortcuts

Thermal budget rule:
- boundary paths must not bypass the logic of the central stack

---

## Passive Margin Interpretation

The passive budget posture for Max-01 is:

### Comfortable passive region
**500–800 W/cm²**

Interpretation:
- this is where Max-01 should most credibly live as a passive-first localized insert

### Thin-margin passive region
**800–1000 W/cm²**

Interpretation:
- the stack may still remain analytically coherent here
- but oxidation, emissivity drift, interface damage, and structural mismatch become increasingly punishing
- this is the zone where optimism must be restrained

### Passive cliff approach region
**1000 W/cm² and above**

Interpretation:
- this is where local-only active relief becomes increasingly justified
- not because the stack is automatically impossible here
- but because the analytical passive margin begins to crowd the severe oxidizing survivability ceiling too aggressively

---

## Local Active-Relief Sizing Logic

The v0.1 budget uses a simple burden-reduction framing for AR-05.

If a local hotspot receives heat flux:

q_hotspot

and the stack is intended to behave more like a safer effective local band:

q_target

then the active branch must help manage approximately:

Δq = q_hotspot - q_target

For a local area A, the thermal intercept burden becomes:

Q_intercept = Δq × A

This gives a first-pass sizing logic for local active relief.

---

## Example Local Active-Relief Estimates

These examples are analytical only.

### Example 1
Local hotspot:
**1200 W/cm²**

Desired effective local target:
**1000 W/cm²**

Required intercept:
**200 W/cm²**

For area:
**25 cm²**
Intercept burden:
**5 kW**

For area:
**50 cm²**
Intercept burden:
**10 kW**

For area:
**100 cm²**
Intercept burden:
**20 kW**

---

### Example 2
Local hotspot:
**1500 W/cm²**

Desired effective local target:
**1000 W/cm²**

Required intercept:
**500 W/cm²**

For area:
**10 cm²**
Intercept burden:
**5 kW**

For area:
**25 cm²**
Intercept burden:
**12.5 kW**

For area:
**50 cm²**
Intercept burden:
**25 kW**

These examples show why AR-05 cannot be treated casually.
Severe local hotspot relief quickly becomes a multi-kilowatt thermal-management problem.

---

## Thermal Intercept and Recovery Budget Logic

IR-06 is only permitted to operate on a controlled intercepted heat stream.

The analytical recovery estimate is:

P_electric = η_recovery × Q_intercept

Where:

- P_electric = electric output
- η_recovery = conversion efficiency assumption
- Q_intercept = controlled intercepted thermal power

For v0.1, IR-06 is treated as:

- **TPV-first**
- **TEG-tail optional**
- **secondary to TPS survival**

---

## Example Recovery Estimates

These examples are analytical only.

### Recovery Case A
Intercepted thermal stream:
**5 kW**

At recovery efficiency:
**20%**
Estimated electric output:
**1.0 kWe**

At recovery efficiency:
**27%**
Estimated electric output:
**1.35 kWe**

---

### Recovery Case B
Intercepted thermal stream:
**10 kW**

At recovery efficiency:
**20%**
Estimated electric output:
**2.0 kWe**

At recovery efficiency:
**27%**
Estimated electric output:
**2.7 kWe**

---

### Recovery Case C
Intercepted thermal stream:
**20 kW**

At recovery efficiency:
**20%**
Estimated electric output:
**4.0 kWe**

At recovery efficiency:
**27%**
Estimated electric output:
**5.4 kWe**

These numbers do **not** justify weakening the upstream thermal stack.
They exist only to show that a bounded recovery sidecar could be analytically meaningful if the intercept stream already exists for protection reasons.

---

## Thermo-Structural Budget Logic

The stack is expected to see strong thermal gradients.

Thermo-structural budget logic in v0.1 focuses on the following truths:

1. the exposed face wants to run much hotter than the deeper structure
2. different layers likely want to expand differently
3. rigid restraint can convert thermal success into structural failure
4. segmentation reduces some scaling penalties but introduces joint and edge penalties
5. local damage can shift both stress and thermal flow
6. oxidation and cracking can reinforce each other

This is why the structural budget is tied to the thermal budget instead of being handled later.

---

## Primary Thermo-Structural Mismatch Risks

### TM-01 — Hot-face expansion against colder support
If HTZ-01 is strongly restrained while running far hotter than the carrier region, crack-driving stress rises.

### TM-02 — Brittle transition/interface failure
If OX-02 or adjacent interfaces are too brittle under gradient loading, the chemistry layer becomes the failure plane.

### TM-03 — Decoupler underperformance
If SD-03 is too stiff, mismatch stress is not sufficiently reduced.  
If it is too soft or weak, support coherence is lost.

### TM-04 — Carrier thermal short plus restraint
If TC-04 is too thermally aggressive and too structurally rigid, it becomes both a heat path and a crack amplifier.

### TM-05 — Joint-ring movement mismatch
If the insert center and perimeter do not move compatibly, SJ-08 becomes a likely failure initiator.

### TM-06 — Damage-induced local stress concentration
A chip, flaw, seam defect, or oxidation pit can raise local stress and also alter the thermal field.

---

## Structural Budget Priorities by Layer

### HTZ-01
Priority:
- survive exposed thermal burden without becoming a crack source too quickly

### OX-02
Priority:
- remain chemically useful without turning into a brittle interfacial trap

### SD-03
Priority:
- provide enough compliance to reduce mismatch damage while preserving support coherence

### TC-04
Priority:
- support the insert without acting like a rigid thermal and structural punishment path

### SJ-08
Priority:
- keep boundary movement and boundary thermal access from defeating the stack

---

## Budget Acceptance Logic for Max-01

A Max-01 architecture remains analytically acceptable only if all of the following stay true:

1. Band A remains passive-first without obvious contradiction
2. Band B remains aggressive but still coherent without hidden fantasy assumptions
3. Band C is treated honestly as a local-only severe hotspot band
4. the stack does not depend on broad active cooling
5. the energy-recovery branch remains secondary
6. structural mismatch is explicitly accounted for
7. seams and joints remain inside the budget, not outside it
8. observability remains compatible with the stack

If any of these fail, Max-01 must be narrowed or revised.

---

## What Later Validation Must Compare Against This Budget

Later validation work should compare measured behavior against these analytical budget questions:

- was the exposed-face temperature trend in family with the first-pass logic?
- did degradation shift the apparent thermal behavior significantly?
- did the deeper stack see more heat than expected?
- did mismatch-driven damage begin earlier than expected?
- did seams and edges behave worse than the center?
- did AR-05 reduce local burden measurably where used?
- did IR-06 recover bounded power without worsening protection?
- did the stack fail thermally, structurally, chemically, or through boundary behavior first?

---

## What This Module Does Not Claim

This module does **not** claim:

- validated exposed-face temperatures
- validated backface temperatures
- validated heat interception values
- validated recovery efficiency
- validated stress values
- validated cycle life
- validated structural survivability
- validated seam survivability
- validated active-relief performance
- validated integrated thermal model accuracy

This is an analytical budget only.

---

## Relationship to Other Modules

This module depends on:
- `mission-envelope.md`
- `stack-architecture.md`
- `materials-screening.md`
- `oxidation-recession.md`

This module informs:
- `hotspot-active-relief.md`
- `thermal-intercept-recovery.md`
- `risk-failure-register.md`
- `validation-campaign.md`

---

## v0.1 Thermo-Structural Budget Summary

The v0.1 thermo-structural budget says:

- Band A is the most credible passive target
- Band B is possible only with tighter realism and less wishful thinking
- Band C is local-only and likely assistance-worthy
- reradiative exposed-face logic is necessary but not sufficient
- oxidation and structural mismatch are major budget drivers
- active relief is sized in kilowatts, not vague optimism
- energy recovery can matter only downstream of controlled interception
- the insert can fail at the face, interface, carrier, or joint ring
- the budget is only useful if later testing proves or corrects it

That is the locked thermo-structural budget posture for v0.1.
