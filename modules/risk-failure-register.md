# Risk Failure Register

## Module Purpose

This module defines the **v0.1 risk and failure register** for IX-HfTaZen-Shield.

Its job is to answer:

1. what can realistically go wrong in the Max-01 architecture
2. how those risks are categorized
3. which risks are expected, tolerated, elevated, or unacceptable
4. what signals would indicate each risk is emerging
5. what architectural response is expected if a risk begins to dominate

This module does **not** claim that the listed risks are fully solved.

It freezes the failure-aware posture for v0.1.

---

## Governing Rule

IX-HfTaZen-Shield is not allowed to behave like a concept that only describes how it succeeds.

A credible localized extreme-heat TPS insert architecture must also state:

- how it is most likely to fail
- where it is most likely to fail first
- what conditions accelerate failure
- what signs of failure should appear
- when a feature should be cut rather than defended

This register exists to keep the repo honest.

---

## Risk Posture

The v0.1 program uses the following posture:

- **identify early**
- **bound clearly**
- **instrument where possible**
- **do not hide architectural contradictions**
- **cut complexity that does not earn its place**
- **prefer smaller truthful scope over larger fictional scope**

This means the register is a design tool, not a disclaimer.

---

## Risk Categories

The Max-01 risk register is organized into the following categories:

1. thermal risks
2. oxidation and recession risks
3. thermo-structural and interface risks
4. joint and boundary risks
5. active-relief risks
6. thermal-recovery risks
7. instrumentation risks
8. scope and evidence risks
9. integration risks

Each risk entry includes:

- risk ID
- name
- category
- description
- likely trigger
- likely indicator
- likely consequence
- risk class
- preferred mitigation posture

---

## Risk Class Definitions

### Class R1 — Managed
Known and expected.  
May remain in the architecture if bounded and observed.

### Class R2 — Elevated
Materially important.  
Requires explicit design attention and later validation focus.

### Class R3 — Critical
Can dominate the architecture or invalidate the concept if not handled correctly.

### Class R4 — Disqualifying
If this risk becomes real in the current configuration, the affected branch or architecture posture must be cut, narrowed, or restructured.

---

## Thermal Risks

### RF-THERM-01
**Name:** Passive margin collapse at local hotspot  
**Category:** Thermal  
**Description:**  
A local region enters a thermal burden state where the passive stack no longer has credible margin.  
**Likely trigger:**  
Local loading in upper Band B or Band C, geometric concentration, edge intensification, or degraded emissive surface state.  
**Likely indicator:**  
Rising backface trend, rising interface burden, or exposed-face damage progression inconsistent with the passive model.  
**Likely consequence:**  
Rapid degradation of HTZ-01, interface overburden, or need for AR-05 where none was planned.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Do not hide it. Narrow the local use case, add bounded AR-05, or reduce the claimed passive target.

---

### RF-THERM-02
**Name:** Thermal choke underperformance  
**Category:** Thermal  
**Description:**  
TC-04 fails to sufficiently limit deeper thermal transfer.  
**Likely trigger:**  
Overly conductive carrier logic, poor layer integration, or local bypass paths.  
**Likely indicator:**  
Backface thermal burden rises faster than expected for a given surface condition.  
**Likely consequence:**  
Protected-side overheating, reduced insert usefulness, or false confidence in exposed-face survival.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Rework TC-04 family choice, geometry, or integration before adding downstream complexity.

---

### RF-THERM-03
**Name:** Boundary thermal bypass  
**Category:** Thermal  
**Description:**  
Heat bypasses the intended central stack logic through seams, edges, or joint paths.  
**Likely trigger:**  
Poor SJ-08 design, mismatch-driven gaps, or localized boundary damage.  
**Likely indicator:**  
Perimeter or seam-adjacent backface burden exceeds center-region expectation.  
**Likely consequence:**  
Boundary-led failure even when the central stack looks acceptable.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Treat boundaries as first-class thermal paths in design and validation.

---

## Oxidation and Recession Risks

### RF-OX-01
**Name:** Exposed-face oxidation acceleration  
**Category:** Oxidation / recession  
**Description:**  
HTZ-01 degrades faster than expected in oxidizing heat.  
**Likely trigger:**  
Surface-state instability, insufficient oxidation tolerance, or hotter-than-expected local loading.  
**Likely indicator:**  
Visible surface change, geometry retreat, emissive behavior shift, or increased downstream burden over time.  
**Likely consequence:**  
Rapid loss of useful hot-face behavior and narrowed reuse potential.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Downgrade claims, revise hot-face candidate family, or admit a narrower thermal band.

---

### RF-OX-02
**Name:** Hidden interface oxidation  
**Category:** Oxidation / recession  
**Description:**  
OX-02 or the region beneath HTZ-01 degrades before surface failure becomes obvious.  
**Likely trigger:**  
Crack-assisted ingress, interface brittleness, or local chemistry incompatibility.  
**Likely indicator:**  
Unexpected thermal drift, local delamination signs, or post-test hidden damage.  
**Likely consequence:**  
Sudden structural loss beneath a seemingly acceptable surface.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Prioritize interface-focused coupon and sectioned post-test inspection.

---

### RF-OX-03
**Name:** Edge-first oxidation defeat  
**Category:** Oxidation / recession  
**Description:**  
The insert perimeter or seam becomes a faster oxidation path than the exposed center.  
**Likely trigger:**  
Poor joint-ring chemistry, local movement, exposed boundary paths, or edge damage.  
**Likely indicator:**  
Perimeter recession, seam roughening, or edge-driven heat leakage.  
**Likely consequence:**  
Boundary-led insert defeat.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Increase SJ-08 priority and validate damaged-edge conditions early.

---

### RF-OX-04
**Name:** Recession-driven geometry destabilization  
**Category:** Oxidation / recession  
**Description:**  
Material loss changes geometry enough to alter local heating or stress concentration.  
**Likely trigger:**  
Local retreat, spall, pitting, or uneven edge loss.  
**Likely indicator:**  
Surface profile change, hotspot migration, or accelerating local degradation.  
**Likely consequence:**  
Self-amplifying local failure.  
**Risk class:** R2  
**Preferred mitigation posture:**  
Track geometry change explicitly in later test planning.

---

## Thermo-Structural and Interface Risks

### RF-STRUCT-01
**Name:** Hot-face / support mismatch cracking  
**Category:** Thermo-structural  
**Description:**  
Thermal expansion mismatch drives cracking between upper and lower stack regions.  
**Likely trigger:**  
High gradients, rigid restraint, poor SD-03 function, or incompatible layer choices.  
**Likely indicator:**  
Crack initiation, displacement change, abnormal thermal shift, or edge chipping.  
**Likely consequence:**  
Loss of exposed-face integrity or creation of new oxidation paths.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Protect SD-03’s role and validate against hard-bond controls.

---

### RF-STRUCT-02
**Name:** Decoupling layer underperformance  
**Category:** Thermo-structural  
**Description:**  
SD-03 fails to reduce mismatch stress enough or becomes mechanically incoherent.  
**Likely trigger:**  
Interlayer too stiff, too weak, too thermally aggressive, or poorly integrated.  
**Likely indicator:**  
No meaningful improvement versus rigid-stack comparison, or new instability appears.  
**Likely consequence:**  
The central structural thesis of Max-01 weakens.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Do not protect SD-03 out of pride; replace or narrow it if it does not earn its role.

---

### RF-STRUCT-03
**Name:** Transition-layer brittleness trap  
**Category:** Thermo-structural / interface  
**Description:**  
OX-02 helps oxidation logic but becomes a brittle crack plane under thermal loading.  
**Likely trigger:**  
Poor chemistry-mechanics balance or incompatible adjacency with HTZ-01 / SD-03.  
**Likely indicator:**  
Interfacial cracking, layer separation, or unexpected sensitivity to cycling.  
**Likely consequence:**  
The oxidation-control layer becomes the failure accelerator.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Assess OX-02 as both chemistry and mechanics, never chemistry alone.

---

### RF-STRUCT-04
**Name:** Carrier becomes thermal-stress amplifier  
**Category:** Thermo-structural  
**Description:**  
TC-04 acts as both a heat path and a mechanical restraint trap.  
**Likely trigger:**  
Carrier over-prioritized for stiffness or support while ignoring thermal penalty.  
**Likely indicator:**  
Higher-than-expected backface burden and poor mismatch response together.  
**Likely consequence:**  
Lower-stack damage and architecture contradiction.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Rebalance carrier logic before adding optional branches.

---

## Joint and Boundary Risks

### RF-JOINT-01
**Name:** Seam-first failure  
**Category:** Joint / boundary  
**Description:**  
The insert fails first at a seam, gap, or interface ring rather than the central hot face.  
**Likely trigger:**  
Poor SJ-08 definition, local motion, poor edge protection, or thermal bypass.  
**Likely indicator:**  
Perimeter-localized damage, crack growth from an edge, or seam heat signature rise.  
**Likely consequence:**  
Localized defeat of the insert and invalidation of central-stack optimism.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Make seams and damaged-edge states part of early validation, not late cleanup.

---

### RF-JOINT-02
**Name:** Boundary movement incompatibility  
**Category:** Joint / boundary  
**Description:**  
Center and perimeter regions do not move compatibly under heating.  
**Likely trigger:**  
Segmentation mismatch, restraint mismatch, or underdesigned joint geometry.  
**Likely indicator:**  
Edge lift, displacement divergence, or repeated edge cracking.  
**Likely consequence:**  
Insert life becomes boundary-limited.  
**Risk class:** R2  
**Preferred mitigation posture:**  
Treat movement compatibility as a design function, not a fabrication detail.

---

## Active-Relief Risks

### RF-AR-01
**Name:** Active branch added without real need  
**Category:** Active relief  
**Description:**  
AR-05 is included because it sounds advanced rather than because the thermal budget demanded it.  
**Likely trigger:**  
Unbounded ambition or fear of admitting the passive envelope.  
**Likely indicator:**  
No clear hotspot criterion, no clear intercept burden, vague justification language.  
**Likely consequence:**  
Complexity without real gain.  
**Risk class:** R2  
**Preferred mitigation posture:**  
Cut AR-05 unless the hotspot case is explicitly defined.

---

### RF-AR-02
**Name:** Active branch creates worse oxidation path  
**Category:** Active relief  
**Description:**  
AR-05 integration opens chemistry or flow paths that worsen total risk.  
**Likely trigger:**  
Poorly integrated porous or routed relief concept.  
**Likely indicator:**  
New local degradation concentrated around the relief region or its interfaces.  
**Likely consequence:**  
AR-05 becomes worse than the hotspot.  
**Risk class:** R4  
**Preferred mitigation posture:**  
If this appears, cut or redesign AR-05 before defending it.

---

### RF-AR-03
**Name:** Local relief moves failure instead of reducing it  
**Category:** Active relief  
**Description:**  
AR-05 shaves the hotspot but creates unacceptable burden elsewhere.  
**Likely trigger:**  
Poorly bounded heat routing or redistribution.  
**Likely indicator:**  
Improved local peak with worse downstream or perimeter response.  
**Likely consequence:**  
False success narrative with hidden system penalty.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Require before/after burden accounting in any AR-05 evaluation.

---

### RF-AR-04
**Name:** Active branch becomes architecture dependency  
**Category:** Active relief  
**Description:**  
The stack stops being a coherent passive-first concept without AR-05.  
**Likely trigger:**  
Progressive overreliance on active relief to rescue poor passive choices.  
**Likely indicator:**  
Passive envelope keeps shrinking while AR-05 keeps growing in importance.  
**Likely consequence:**  
Mission drift outside v0.1 scope.  
**Risk class:** R4  
**Preferred mitigation posture:**  
Narrow the mission or redesign the passive stack; do not hide behind AR-05.

---

## Thermal-Recovery Risks

### RF-IR-01
**Name:** Recovery branch incentivizes harmful heat leakage  
**Category:** Thermal recovery  
**Description:**  
IR-06 is positioned or justified in a way that rewards extra inward heat.  
**Likely trigger:**  
Energy-first thinking or poorly bounded thermal source logic.  
**Likely indicator:**  
Recovery claims rise while thermal choke discipline weakens.  
**Likely consequence:**  
The TPS starts sacrificing protection for power.  
**Risk class:** R4  
**Preferred mitigation posture:**  
Immediate architectural correction or cut IR-06.

---

### RF-IR-02
**Name:** Recovery output is oversold relative to source stream  
**Category:** Thermal recovery  
**Description:**  
Electric output claims become disconnected from the actual intercepted thermal stream.  
**Likely trigger:**  
Hype, loose accounting, or failure to track residual heat.  
**Likely indicator:**  
Power numbers appear without bounded Q_intercept logic.  
**Likely consequence:**  
Repo credibility loss and corrupted design priorities.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Enforce source-stream accounting and conservative analytic cases.

---

### RF-IR-03
**Name:** Residual heat trap  
**Category:** Thermal recovery  
**Description:**  
IR-06 converts some heat but leaves a worse downstream thermal burden than expected.  
**Likely trigger:**  
Insufficient residual-heat planning or poor cassette placement.  
**Likely indicator:**  
Backface thermal trend worsens despite “successful” recovery math.  
**Likely consequence:**  
Secondary function harms the primary function.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Treat residual heat as a first-class burden in every recovery estimate.

---

### RF-IR-04
**Name:** Recovery branch complexity bloat  
**Category:** Thermal recovery  
**Description:**  
IR-06 adds more architecture burden than secondary value.  
**Likely trigger:**  
Overcomplication or fascination with multifunctionality.  
**Likely indicator:**  
Recovery logic requires major routing, mass, or support concessions.  
**Likely consequence:**  
Reduced coherence of Max-01.  
**Risk class:** R2  
**Preferred mitigation posture:**  
Cut IR-06 unless it remains clearly bounded and removable.

---

## Instrumentation Risks

### RF-HB-01
**Name:** Instrumentation thermal short  
**Category:** Instrumentation  
**Description:**  
HB-07 or its routing creates an unintended heat path.  
**Likely trigger:**  
Poor sensor integration or routing through thermally sensitive layers.  
**Likely indicator:**  
Localized backface hotspot near instrumentation path or unexplained measurement-adjacent heating.  
**Likely consequence:**  
Measurement corrupts the thing being measured.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Simplify or reroute sensing rather than tolerate the penalty.

---

### RF-HB-02
**Name:** Instrumentation survivability mismatch  
**Category:** Instrumentation  
**Description:**  
HB-07 fails too early to provide meaningful trend data.  
**Likely trigger:**  
Sensor placement too aggressive or insufficient thermal tolerance.  
**Likely indicator:**  
Measurement dropout before useful architecture-state information is captured.  
**Likely consequence:**  
Reduced validation value and blind failure progression.  
**Risk class:** R2  
**Preferred mitigation posture:**  
Pull instrumentation farther downstream or simplify the sensing mission.

---

### RF-HB-03
**Name:** False-confidence monitoring  
**Category:** Instrumentation  
**Description:**  
The presence of sensors is mistaken for proof that the architecture is safe.  
**Likely trigger:**  
Cultural or communication failure rather than hardware failure.  
**Likely indicator:**  
Claims become stronger without stronger evidence tiers.  
**Likely consequence:**  
Evidence inflation.  
**Risk class:** R2  
**Preferred mitigation posture:**  
Keep claims tied to evidence, not instrumentation presence.

---

## Scope and Evidence Risks

### RF-SCOPE-01
**Name:** Scope creep into full-vehicle TPS  
**Category:** Scope / evidence  
**Description:**  
The repo starts drifting from localized inserts into general TPS claims.  
**Likely trigger:**  
Enthusiasm, feature creep, or comparison pressure.  
**Likely indicator:**  
Language expands from local severe zones to vehicle-wide use without new evidence.  
**Likely consequence:**  
Loss of technical discipline.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Re-anchor every claim to mission-envelope boundaries.

---

### RF-SCOPE-02
**Name:** Claim inflation beyond evidence tier  
**Category:** Scope / evidence  
**Description:**  
The repo starts claiming validation that it has not earned.  
**Likely trigger:**  
Pressure to sound advanced or impressive.  
**Likely indicator:**  
Words like proven, flight-ready, superior, or breakthrough appear without tier support.  
**Likely consequence:**  
Trust collapse.  
**Risk class:** R4  
**Preferred mitigation posture:**  
Immediate correction using the claims-evidence ladder.

---

### RF-SCOPE-03
**Name:** Radiation-scope contamination  
**Category:** Scope / evidence  
**Description:**  
Radiation protection gets mixed into the baseline stack before the heat-shield concept is coherent.  
**Likely trigger:**  
Trying to do too much in v0.1.  
**Likely indicator:**  
Material choices start serving two missions badly instead of one mission well.  
**Likely consequence:**  
Architecture muddiness and reduced credibility.  
**Risk class:** R2  
**Preferred mitigation posture:**  
Keep radiation as a future branch, not baseline v0.1.

---

## Integration Risks

### RF-INT-01
**Name:** Too many clever subsystems in the thermal path  
**Category:** Integration  
**Description:**  
Optional features accumulate until the architecture becomes harder to believe than the hotspot problem itself.  
**Likely trigger:**  
Unbounded design ambition.  
**Likely indicator:**  
AR-05, IR-06, HB-07, SJ-08, and core stack all begin to depend on each other too tightly.  
**Likely consequence:**  
The repo reads as complexity theater instead of engineering.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Prefer the minimum coherent stack. Cut optional branches aggressively unless earned.

---

### RF-INT-02
**Name:** Variant drift without control  
**Category:** Integration  
**Description:**  
Changes accumulate without a clean reference configuration boundary.  
**Likely trigger:**  
Silent edits or inconsistent module assumptions.  
**Likely indicator:**  
Modules stop matching Max-01.  
**Likely consequence:**  
Internal contradiction.  
**Risk class:** R2  
**Preferred mitigation posture:**  
Use Max-01 as the hard anchor and version any real change.

---

### RF-INT-03
**Name:** Validation path becomes less coherent than architecture  
**Category:** Integration  
**Description:**  
The concept becomes so layered that it cannot be credibly validated in stages.  
**Likely trigger:**  
Too many branch interactions too early.  
**Likely indicator:**  
Test planning cannot isolate what helped or hurt.  
**Likely consequence:**  
Repo stalls at concept level.  
**Risk class:** R3  
**Preferred mitigation posture:**  
Sequence validation so each layer or branch earns its place progressively.

---

## Highest-Priority Risks for v0.1

The following are the highest-priority risks to watch first:

1. **RF-SCOPE-02 — Claim inflation beyond evidence tier**
2. **RF-THERM-01 — Passive margin collapse at local hotspot**
3. **RF-OX-02 — Hidden interface oxidation**
4. **RF-STRUCT-01 — Hot-face / support mismatch cracking**
5. **RF-JOINT-01 — Seam-first failure**
6. **RF-AR-02 — Active branch creates worse oxidation path**
7. **RF-IR-01 — Recovery branch incentivizes harmful heat leakage**
8. **RF-INT-01 — Too many clever subsystems in the thermal path**

These are the risks most capable of invalidating Max-01’s credibility.

---

## Risk Response Rules

### Rule RR-1
If a feature creates a Class R4 risk, the burden of proof shifts to the feature.  
The feature must be cut, narrowed, or isolated unless it clearly earns retention.

### Rule RR-2
If a risk affects boundaries, it cannot be dismissed as secondary.

### Rule RR-3
If a risk is not measurable later, it must at least remain explicit now.

### Rule RR-4
If a lower-priority feature worsens a higher-priority risk, the feature loses.

### Rule RR-5
If two mitigations conflict, the one that preserves passive-first localized TPS coherence wins.

---

## What This Register Is For

This register is meant to support:

- architecture discipline
- validation prioritization
- test planning
- claims discipline
- later design pruning

It is not meant to create the illusion that every listed risk has already been solved.

---

## What This Register Does Not Claim

This register does **not** claim:

- quantified probability of each risk
- validated mitigation effectiveness
- complete hazard coverage
- operational safety qualification
- full system certification logic

This is a v0.1 architecture risk register only.

---

## Relationship to Other Modules

This module depends on:
- `mission-envelope.md`
- `claims-evidence-ladder.md`
- `stack-architecture.md`
- `oxidation-recession.md`
- `thermo-structural-budget.md`
- `hotspot-active-relief.md`
- `thermal-intercept-recovery.md`
- `shield-health-monitoring.md`

This module informs:
- `validation-campaign.md`
- all later validation packages
- future variant decisions
- future keep / cut decisions for optional branches

---

## v0.1 Risk Failure Register Summary

The v0.1 program is built around the idea that:

- the hottest-looking layer may not fail first
- the seam may beat the center
- the interface may beat the face
- optional complexity can become a bigger threat than the original hotspot
- evidence inflation can kill trust faster than a bad coupon result

This register locks those truths into the repo so they cannot be quietly ignored.

That is the frozen risk and failure posture for v0.1.
