# Oxidation Recession

## Module Purpose

This module defines the **oxidation and recession logic** for IX-HfTaZen-Shield v0.1.

Its job is to answer:

1. why oxidation is treated as a primary design threat
2. how oxidation risk is distributed across the Max-01 stack
3. what recession means in this program context
4. what the architecture is trying to resist, delay, or localize
5. what must be measured later to determine whether the stack is improving or failing

This module does **not** claim measured oxidation or recession performance for the IX-HfTaZen-Shield stack.

It freezes the analytical posture for v0.1.

---

## Governing Rule

For IX-HfTaZen-Shield, the exposed-face problem is **oxidation-limited before it is bragging-rights temperature-limited** in the oxidizing baseline case.

That means the program does **not** treat nominal ultra-high melting-point behavior as sufficient proof of usable extreme-heat TPS performance.

A candidate or stack survives oxidation screening only if it improves the architecture under **real oxidizing exposure logic**, not just inert-condition hero logic.

---

## Why Oxidation Is a Primary Threat

In the Max-01 mission envelope:

- the baseline environment is oxidizing
- the exposed face is expected to encounter severe heat
- the insert is localized and segmented
- seams, joints, and edges exist
- thermal gradients and structural mismatch exist
- repeated exposure is part of the concept ambition

Under those conditions, the system can fail long before “bulk melting” becomes the dominant question.

The likely oxidizing-failure drivers include:

- surface chemistry change
- protective-scale instability
- scale cracking or spallation
- oxygen ingress through defects
- interfacial oxidation beneath the hot face
- edge attack at joints or insert boundaries
- locally accelerated degradation at damage sites
- oxidation-assisted embrittlement
- oxidation plus thermal cycling interaction

This is why oxidation gets its own module rather than being treated as a footnote under materials screening.

---

## What Recession Means in This Repo

For IX-HfTaZen-Shield, **recession** means any net loss of effective thermal-protection geometry or function at the exposed region due to combined thermal and chemical attack.

Recession in this repo includes, but is not limited to:

- direct surface material loss
- edge rounding or material retreat
- local thickness loss
- scale loss exposing fresh material
- spall-driven geometry reduction
- oxidation-assisted pitting or roughening that changes the thermal behavior of the exposed surface
- boundary or seam retreat that undermines insert integrity

This repo does **not** assume recession must be zero to remain useful.

It does assume recession must become:
- bounded
- measurable
- localized
- compatible with the intended localized reusable or limited-reuse mission

If recession becomes uncontrolled, the concept fails its mission posture.

---

## Oxidation and Recession Design Philosophy

The v0.1 oxidation/recession philosophy is:

1. **do not pretend the hot face alone solves oxidation**
2. **separate hot-face thermal ambition from buried oxidation-control function**
3. **treat boundaries and joints as oxidation access paths**
4. **assume defects matter**
5. **assume thermal cycling can destabilize protection that looked fine in a single static condition**
6. **prefer architectures that keep damage local and observable**
7. **avoid design choices that require perfect surfaces, perfect processing, or perfect oxygen exclusion**

---

## Oxidation Threat Map by Layer

The stack does not see oxidation uniformly.

### HTZ-01 Radiative UHTC Face
Primary oxidation threat zone.

Threat classes:
- exposed-surface reaction
- protective-scale instability
- local chemistry shift
- crack-assisted oxygen access
- reradiative surface degradation if the surface state changes too far

Primary design intent:
- delay severe oxidation-driven loss of function
- preserve enough exposed-face integrity to keep the stack working

---

### OX-02 Oxidation-Control Transition
Secondary oxidation-defense layer.

Threat classes:
- interface oxidation if HTZ-01 is compromised
- buried scale instability
- loss of chemistry-control function if the transition layer cracks or debonds

Primary design intent:
- slow or localize deeper oxygen-driven damage
- reduce the chance that the hot-face/support interface becomes the first catastrophic internal failure plane

---

### SD-03 Strain-Decoupling Interlayer
Indirect oxidation concern.

Threat classes:
- oxygen access if upper layers crack or open
- property loss if the interlayer is not chemically suited to oxidizing thermal exposure
- degraded compliance if oxidation changes structure or stiffness

Primary design intent:
- remain compatible with the oxidation-control logic above it
- avoid turning into a chemically weak hidden failure zone

---

### TC-04 Thermal Choke Carrier
Protected but not immune.

Threat classes:
- damage if upper-layer oxidation breaches deepen
- local oxidation at attachment paths or exposed interface regions
- thermal-conduction changes if surface breach exposes the carrier region to heat and chemistry it was not meant to see

Primary design intent:
- survive long enough beneath upper-layer degradation to preserve insert function and test observability

---

### AR-05 Active Relief Branch
Oxidation implications depend on architecture.

Threat classes:
- local flow-path exposure
- channel or porous-path degradation
- active branch unintentionally increasing oxidation sensitivity if poorly integrated

Primary design intent:
- reduce hotspot burden without opening worse oxidation pathways than the passive stack would have had

---

### IR-06 Thermal Intercept & Recovery Cassette
Not a primary oxidation layer.

Threat classes:
- indirect thermal penalty if upstream oxidation damage increases heat leakage
- interface penalty if thermal-routing hardware becomes exposed to conditions it was not designed to see

Primary design intent:
- remain safely downstream of oxidation-critical layers

---

### HB-07 Health-Monitoring Backplane
Indirect oxidation concern.

Threat classes:
- exposure after upper-stack breach
- measurement loss due to thermal or chemical overrun

Primary design intent:
- preserve enough function to capture failure progression

---

### SJ-08 Seal & Joint Management Ring
High-risk oxidation-access region.

Threat classes:
- seam oxygen ingress
- edge-scale breakdown
- local movement opening oxidation paths
- insert-boundary degradation that outruns central-face degradation

Primary design intent:
- prevent the perimeter from becoming an oxidation shortcut into the stack

---

## Oxidation Control Strategy in Max-01

Max-01 does **not** rely on one oxidation trick.

It uses a layered strategy:

### Strategy 1 — Delay direct exposed-face degradation
HTZ-01 is chosen to keep the exposed surface in a serious refractory ceramic lane rather than a low-ceiling surface chemistry.

### Strategy 2 — Add a buried oxidation-control transition
OX-02 exists because the exposed hot-face chemistry and the deeper oxidation-control job do not have to be the same material problem.

### Strategy 3 — Reduce crack-driving mismatch
SD-03 exists partly because cracking is not only a structural problem — it is also an oxidation-access problem.

### Strategy 4 — Keep the stack segmented and boundary-aware
A realistic insert architecture must assume oxygen can exploit edges, seams, and local flaws if they are ignored.

### Strategy 5 — Use active relief sparingly
Where local hotspot severity threatens to push the exposed face too close to its credible limit, AR-05 is allowed because lower thermal burden can also reduce oxidation acceleration.

### Strategy 6 — Keep damage measurable
HB-07 is included so oxidation-driven degradation does not remain invisible until the insert is already functionally lost.

---

## Recession-Control Strategy in Max-01

The Max-01 recession-control posture is:

1. keep exposed-face chemistry in the strongest credible lane available to the repo
2. reduce oxidation-driven interface collapse beneath the surface
3. keep structural mismatch from turning microdamage into material-loss acceleration
4. protect edges and seams from becoming first-loss zones
5. allow local-only active relief where it materially reduces geometric-loss risk
6. require later inspection logic capable of detecting geometry and surface-state change

The architecture does **not** assume zero recession.
It assumes recession must be pushed toward:
- smaller
- slower
- more local
- more observable
- less architecture-dominant

---

## Primary Oxidation Failure Modes

These are the major oxidation-linked failure modes the repo is explicitly shaped around.

### OF-01 — Exposed-face scale instability
The hot face reacts and forms a surface state that loses integrity, reducing protection.

### OF-02 — Crack-assisted oxygen ingress
Thermal or mechanical cracking opens access paths for deeper oxidation.

### OF-03 — Interface oxidation beneath the hot face
The region beneath the exposed face becomes the first real damage plane.

### OF-04 — Edge/seam oxidation shortcut
The insert perimeter degrades faster than the center and defeats the stack from the boundary inward.

### OF-05 — Oxidation-assisted embrittlement
Thermal and chemical attack reduce toughness enough that later mechanical or thermal loading drives faster cracking.

### OF-06 — Oxidation plus thermal cycling interaction
A stack that appears acceptable in one exposure becomes unstable across repeated cycles.

### OF-07 — Active-branch oxidation penalty
AR-05 introduces or worsens oxidation sensitivity instead of reducing total risk.

---

## Primary Recession Failure Modes

These are the major recession-linked failure modes for v0.1.

### RF-01 — Surface retreat
Exposed-face material loss reduces thickness or local geometry margin.

### RF-02 — Edge retreat
Insert perimeter loses material first, compromising boundary integrity.

### RF-03 — Spall-driven local loss
Fragments or scales detach, exposing new material and accelerating damage.

### RF-04 — Roughness-driven thermal shift
Surface degradation changes emissive or heat-loading behavior enough to destabilize the expected thermal response.

### RF-05 — Geometry-loss concentration
A local pit, chip, or seam loss creates a hotspot amplifier rather than just a passive loss of thickness.

### RF-06 — Hidden undercutting
The visible surface appears acceptable while deeper regions are being lost or weakened.

---

## Oxidation/Recession Screening Questions

Any candidate stack direction must be checked against the following questions.

### Q1
Does the candidate reduce oxidation risk in the oxidizing baseline case, or does it merely look strong in inert logic?

### Q2
If the exposed face is damaged, does the next layer behave like a meaningful defense or a fast new failure plane?

### Q3
Do seams and boundaries receive explicit oxidation-control logic?

### Q4
Does the architecture remain coherent if small defects exist?

### Q5
Could thermal mismatch damage become an oxidation accelerator?

### Q6
Would the active branch reduce overall damage rate, or accidentally create new vulnerability?

### Q7
Can likely recession signatures be inspected and measured later?

If these questions cannot be answered coherently, the stack remains immature.

---

## What v0.1 Treats as Success

In v0.1, oxidation/recession success is analytical only.

That means success is defined as:

- the stack has explicit oxidation logic
- the stack has explicit recession logic
- the design is not relying on peak-temperature mythology
- the architecture recognizes the difference between exposed-face degradation and deeper interface degradation
- seams and boundaries are recognized as attack paths
- later tests can be designed to reveal whether the logic is real or false

This is enough for v0.1.

---

## What v0.1 Does Not Claim

This module does **not** claim any of the following:

- measured oxidation resistance for Max-01
- measured recession rate for Max-01
- validated cycle life
- validated survivability in a relevant environment
- proven protective-scale chemistry in the integrated stack
- proven edge survivability
- proven seam survivability
- proven active-branch compatibility with oxidation control

Those are later-tier evidence questions.

---

## Required Future Measurements

The validation campaign for oxidation and recession must eventually be able to measure or inspect:

- visible surface-state change
- mass change
- geometry change
- thickness loss or local retreat
- crack and spall appearance
- edge and seam degradation
- interface damage extent
- backface temperature change associated with degradation progression
- pre/post surface and boundary comparison

If the repo cannot define how these will eventually be observed, the oxidation/recession logic is incomplete.

---

## Oxidation-Recession Interaction Rules

The following rules are locked for v0.1.

### Rule OR-1
If a candidate improves nominal peak-temperature prestige but worsens oxidizing survivability, it is downgraded.

### Rule OR-2
If a candidate reduces visible surface loss but increases hidden interface damage risk, it is not automatically acceptable.

### Rule OR-3
If the joint ring is undefined, oxidation control is considered incomplete.

### Rule OR-4
If active relief reduces heat but creates a more dangerous oxygen-access path, it fails the architecture logic.

### Rule OR-5
If a design depends on flawless surfaces and flawless processing to resist oxidation, it is treated as fragile.

### Rule OR-6
If recession cannot be bounded analytically or inspected later, the design remains untrusted.

---

## Relationship to Other Modules

This module depends on:
- `mission-envelope.md`
- `stack-architecture.md`
- `materials-screening.md`

This module informs:
- `thermo-structural-budget.md`
- `hotspot-active-relief.md`
- `risk-failure-register.md`
- `validation-campaign.md`

---

## v0.1 Oxidation-Recession Summary

IX-HfTaZen-Shield treats oxidation and recession as central design problems, not secondary footnotes.

The v0.1 posture is:

- oxidizing environment is the baseline
- exposed-face behavior alone is not enough
- buried oxidation control matters
- cracking and mismatch can become oxidation accelerators
- boundaries are high-risk attack paths
- recession must be bounded and observable
- the stack is trying to delay, localize, and measure damage — not pretend it cannot occur

That is the locked oxidation/recession logic for v0.1.
