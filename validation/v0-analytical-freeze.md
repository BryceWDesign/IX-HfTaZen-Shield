# V0 Analytical Freeze

## Stage Identity

**Stage:** V0  
**Name:** Analytical Freeze  
**Program:** IX-HfTaZen-Shield  
**Reference configuration:** Max-01  
**Evidence tier supported:** E0 + E1 + E2 only  
**Execution status:** planned / frozen for v0.1  
**Purpose:** lock the analytical baseline before any physical validation claims are attempted

---

## Stage Purpose

V0 exists to make sure the repo is coherent **before** chemistry screening, coupon design, or subsystem ambition starts spreading in different directions.

V0 is the stage where the program must prove that it has:

- a stable mission envelope
- a stable claim ceiling
- a stable layer stack
- a stable materials-screening direction
- a stable thermal and thermo-structural budget
- a stable risk posture
- a stable validation order

If those are not frozen first, later validation work becomes noisy, contradictory, and much easier to oversell.

---

## What V0 Must Freeze

The following items are mandatory freeze targets.

### F1 — Mission identity
The program must remain:

- localized
- reusable or limited-reuse in concept
- extreme-heat focused
- oxidizing-baseline
- passive-first
- test-first
- no-flight-worthiness-claim

### F2 — Claim ceiling
The repo must remain at:

- E0 for concept framing
- E1 for analytical reasoning
- E2 for literature-grounded screening

No higher evidence may be implied.

### F3 — Reference configuration
`Max-01` must remain the canonical reference configuration for v0.1.

### F4 — Canonical layer stack
The following layer order must remain frozen:

1. HTZ-01 Radiative UHTC Face  
2. OX-02 Oxidation-Control Transition  
3. SD-03 Strain-Decoupling Interlayer  
4. TC-04 Thermal Choke Carrier  
5. AR-05 Active Relief Branch *(optional)*  
6. IR-06 Thermal Intercept & Recovery Cassette *(optional)*  
7. HB-07 Health-Monitoring Backplane  
8. SJ-08 Seal & Joint Management Ring  

### F5 — Severity bands
The thermal bands must remain frozen as:

- **Band A:** 500–800 W/cm²
- **Band B:** 800–1000 W/cm²
- **Band C:** 1000–1500 W/cm² local only

### F6 — Primary materials direction
The following candidate-family directions must remain frozen:

- **HTZ-01:** Hf-rich Hf–Ta–Zr–W–(C,N) high-entropy carbide / carbonitride lane
- **OX-02:** HfSiCN-class oxidation-control transition
- **SD-03:** refractory compliant interlayer architecture
- **TC-04:** refractory or ceramic-compatible segmented carrier
- **AR-05:** porous-UHTC local transpiration-style relief
- **IR-06:** TPV-first recovery cassette
- **HB-07:** high-temperature-compatible sensing backplane
- **SJ-08:** refractory-compatible joint and edge-management architecture

### F7 — First-pass thermal posture
The v0.1 budget must remain frozen around:

- emissivity assumption: **0.85**
- analytical radiative-balance logic
- passive comfort band in Band A
- thin passive margin in Band B
- local-only active-relief justification in Band C

### F8 — Risk posture
The repo must remain failure-aware and explicitly centered on:

- passive margin collapse
- hidden interface oxidation
- hot-face / support mismatch cracking
- seam-first failure
- active-branch self-harm
- recovery-branch leak-seeking behavior
- claim inflation beyond evidence

### F9 — Validation order
The validation sequence must remain:

- V0 Analytical Freeze
- V1 Chemistry Screening
- V2 Oxidation-Control Coupons
- V3 Thermal Shock / Cycle Coupons
- V4 Attachment / Mismatch Stack Coupons
- V5 High-Heat Coupon Exposure
- V6 Deliberate Damage Coupons
- V7 Local Active-Relief Demonstrator
- V8 Thermal Intercept & Recovery Demonstrator
- V9 Integrated Subscale Insert

---

## V0 Questions That Must Be Answered

Before the stage is considered complete, the repo must be able to answer the following without contradiction.

### Q1
What exact problem is IX-HfTaZen-Shield trying to solve?

### Q2
What exact use case is inside scope, and what is outside scope?

### Q3
What exact layer stack is the program evaluating?

### Q4
What exact claims are allowed now?

### Q5
What exact claims are forbidden now?

### Q6
What exact heat-flux bands define the concept’s intended analytical operating envelope?

### Q7
What exact optional branches exist, and under what gating rules?

### Q8
What exact failure modes are expected to dominate first?

### Q9
What exact validation sequence will decide whether the architecture deserves stronger claims later?

If the repo cannot answer all nine questions clearly, V0 is incomplete.

---

## V0 Inputs

V0 depends on the following frozen modules and files.

### Required source files
- `PROJECT_CHARTER.md`
- `modules/mission-envelope.md`
- `modules/claims-evidence-ladder.md`
- `modules/stack-architecture.md`
- `reference-configs/max-01.md`
- `modules/materials-screening.md`
- `modules/oxidation-recession.md`
- `modules/thermo-structural-budget.md`
- `modules/hotspot-active-relief.md`
- `modules/thermal-intercept-recovery.md`
- `modules/shield-health-monitoring.md`
- `modules/risk-failure-register.md`
- `modules/validation-campaign.md`

### Required interpretation posture
These files must agree in meaning, not merely exist.

---

## V0 Outputs

When V0 is complete, it should yield the following outputs.

### O1 — Frozen analytical baseline
A stable point of reference for all later work.

### O2 — Unknowns list
An explicit list of what the repo still does not know.

### O3 — Contradiction check
A record showing whether the modules agree or whether a reference-configuration correction is needed.

### O4 — Gate to V1
A clear decision on whether the program is coherent enough to proceed to chemistry screening.

### O5 — Claims lock
A clean statement of the maximum public-facing claim allowed at this stage.

---

## Public Claim Allowed at V0

The maximum allowed summary claim at V0 is:

> IX-HfTaZen-Shield is a test-first TPS concept focused on localized reusable extreme-heat protection. Current status: analytical architecture with defined failure modes and planned coupon/subscale validation. No flight-worthiness claim.

No statement stronger than this is allowed at V0.

---

## Public Claims Forbidden at V0

The following remain prohibited:

- proven
- validated
- flight-ready
- mission-ready
- better than NASA
- better than SpaceX
- best heat shield
- self-powering shield
- integrated radiation shielding by default
- operational reuse claim
- real-world service-temperature claim
- full-vehicle TPS implication

---

## V0 Acceptance Checklist

A V0 freeze is accepted only if every item below is true.

### Identity and scope
- [ ] The repo is clearly localized, not full-vehicle TPS.
- [ ] Oxidizing environment is clearly baseline.
- [ ] Radiation shielding is not part of baseline v0.1.
- [ ] Passive-first posture is explicit.
- [ ] Optional branches are clearly secondary.

### Claims discipline
- [ ] Allowed claims are explicitly listed.
- [ ] Forbidden claims are explicitly listed.
- [ ] No module overstates maturity.
- [ ] The repo remains within E0 + E1 + E2 only.

### Architecture freeze
- [ ] Max-01 is explicitly frozen.
- [ ] The layer order is stable across files.
- [ ] AR-05 is optional and local-only everywhere it appears.
- [ ] IR-06 is downstream and secondary everywhere it appears.
- [ ] HB-07 is treated as nonintrusive observability support.
- [ ] SJ-08 is treated as part of the architecture, not trim.

### Materials freeze
- [ ] HTZ-01 is locked to the Hf-rich Hf–Ta–Zr–W–(C,N) lane.
- [ ] OX-02 is locked to the HfSiCN-class lane.
- [ ] Comparison families are preserved but do not displace the primary direction without evidence.

### Thermal and structural freeze
- [ ] The three severity bands are stable across the repo.
- [ ] The emissivity assumption is stable across the repo.
- [ ] The passive comfort / thin-margin / assisted-band logic is stable across the repo.
- [ ] The thermo-structural mismatch thesis is explicit.
- [ ] The joint / seam risk is explicit.

### Validation freeze
- [ ] The V0–V9 order is stable.
- [ ] Controls and damage states are part of the validation logic.
- [ ] Optional branches do not outrun the core passive stack.
- [ ] Keep / cut logic for AR-05 and IR-06 exists.

### Risk freeze
- [ ] The highest-priority risks are explicitly named.
- [ ] Claim inflation is treated as a critical failure mode.
- [ ] Boundary-led failure is treated as plausible.
- [ ] Interface-led failure is treated as plausible.
- [ ] Complexity bloat is treated as a real risk.

If any unchecked item remains, V0 stays open.

---

## V0 Failure Conditions

V0 fails if any of the following are found.

### Fail A — Scope contradiction
One module implies localized inserts while another implies full-vehicle coverage.

### Fail B — Claim contradiction
One module respects the evidence ceiling while another implies validation or superiority.

### Fail C — Architecture contradiction
The layer order, layer role, or optional-branch logic disagrees across modules.

### Fail D — Thermal contradiction
The thermal bands or passive/active logic shift without explicit versioning.

### Fail E — Branch inversion
AR-05 or IR-06 starts behaving like a primary architecture requirement.

### Fail F — Risk denial
A major failure mode is erased, downplayed, or treated as someone else’s problem.

### Fail G — Validation incoherence
The program cannot cleanly explain what V1 is supposed to test first.

Any one of these is enough to block progress to V1.

---

## Unknowns List Locked at V0

These unknowns remain open after the analytical freeze and must not be disguised as solved.

### U1 — Exact composition
The exact best-performing HTZ-01 composition inside the primary lane is not yet known.

### U2 — Exact interlayer implementation
The exact SD-03 implementation is not yet known.

### U3 — Exact carrier realization
The best TC-04 structure and material implementation are not yet known.

### U4 — Exact oxidation-control implementation
The best OX-02 formulation and thickness logic are not yet known.

### U5 — Real thermal margin
The actual margin in Bands A, B, and C is not yet measured.

### U6 — Real damage tolerance
The real damaged-state behavior is not yet known.

### U7 — Real AR-05 value
The active-relief branch has not earned retention yet.

### U8 — Real IR-06 value
The recovery branch has not earned retention yet.

### U9 — Real instrumentation survivability
HB-07 remains an architecture requirement, not a proven sensing package.

### U10 — Real seam durability
SJ-08 remains a critical architecture focus, not a solved boundary system.

---

## V0 Decision Logic

After V0, only three decisions are allowed.

### Decision D1 — Proceed to V1
Use when the repo is internally coherent and the first chemistry-screening comparison can be justified.

### Decision D2 — Revise and repeat V0
Use when contradictions exist but the architecture still appears salvageable.

### Decision D3 — Narrow scope before V1
Use when the concept is too ambitious to test honestly in its current frozen form.

There is no valid “pretend it is good enough” option.

---

## V0 Success Criteria

V0 is successful only if it produces:

- one frozen reference configuration
- one frozen scope statement
- one frozen claim ceiling
- one frozen materials-screening direction
- one frozen thermal posture
- one frozen risk posture
- one frozen validation order
- one honest unknowns list

That is enough.  
Anything more belongs to later stages.

---

## V0 Summary

V0 is the stage where IX-HfTaZen-Shield proves that it is at least a **coherent analytical program** rather than a pile of aggressive ideas.

If V0 is done correctly, the repo can move to V1 with discipline.

If V0 is done badly, every later result becomes easier to misread, oversell, or waste.

That is why V0 exists.
