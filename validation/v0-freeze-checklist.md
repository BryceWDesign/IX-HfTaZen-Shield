# V0 Freeze Checklist

## Purpose

This checklist is the shortest operational version of the V0 analytical freeze.

Use it to confirm that the repo is ready to leave concept framing and enter V1 chemistry screening.

---

## Pass Gate

All items below must be true.

### Scope
- [ ] Localized insert scope is explicit.
- [ ] Full-vehicle TPS is explicitly out of scope.
- [ ] Oxidizing baseline environment is explicit.
- [ ] Radiation protection is not baseline v0.1.

### Claims
- [ ] Public claim ceiling is locked.
- [ ] No module implies validation beyond E0 + E1 + E2.
- [ ] No superiority claim appears anywhere.

### Architecture
- [ ] Max-01 is frozen.
- [ ] Layer order matches the canonical stack.
- [ ] AR-05 is optional and local-only.
- [ ] IR-06 is downstream and secondary.
- [ ] HB-07 is nonintrusive.
- [ ] SJ-08 is treated as core architecture.

### Materials
- [ ] HTZ-01 primary lane is frozen.
- [ ] OX-02 primary lane is frozen.
- [ ] SD-03, TC-04, AR-05, IR-06, HB-07, and SJ-08 remain at candidate-family level.

### Thermal / structural
- [ ] Band A / B / C are stable across files.
- [ ] Emissivity assumption is stable.
- [ ] Passive margin logic is stable.
- [ ] Mismatch-stress logic is explicit.
- [ ] Boundary-led failure is explicit.

### Validation
- [ ] V0–V9 order is stable.
- [ ] V1 entry condition is clear.
- [ ] Damage-state testing exists in the plan.
- [ ] Optional branches do not outrun the core passive stack.

### Risk
- [ ] Claim inflation is listed as critical.
- [ ] Hidden interface oxidation is listed as critical.
- [ ] Seam-first failure is listed as critical.
- [ ] Complexity bloat is listed as a real threat.

---

## Result

- If every box is checked, V0 may pass and the repo may proceed to V1.
- If any box is unchecked, V0 remains open.
