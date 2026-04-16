# V6 Damage Comparison Matrix

## Purpose

This file is the compact comparison matrix for the V6 deliberate-damage stage.

It exists to keep the stage centered on the real question:

> Does the surviving passive stack remain more credible than simpler comparisons once realistic local damage is introduced?

---

## Candidate Set

| Article ID | Damage State | Primary Comparison Purpose |
|---|---|---|
| V6-B0 | Pristine surviving passive baseline | Preserve direct comparison against undamaged behavior |
| V6-D1 | Surface-flaw damaged article | Test exposed-face imperfection sensitivity |
| V6-D2 | Chipped-edge damaged article | Test edge damage sensitivity |
| V6-D3 | Corner-loss damaged article | Test corner geometry sensitivity |
| V6-D4 | Boundary / seam analog damaged article | Test boundary-led damage sensitivity |
| V6-R1 | Simplified damaged passive comparison | Determine whether the full passive stack still earns its complexity after damage |
| V6-R2 | Multiple severity levels of one damage class | Check whether response is gradual or threshold-like |

---

## Ranking Categories

Use the following first-pass ranking categories when V6 is eventually executed.

### Rank A
Strong continuation candidate

### Rank B
Credible continuation candidate with caveats

### Rank C
Useful comparison result but not preferred for continuation

### Rank D
Cut or deprioritize

---

## Minimum Evaluation Questions

Each damaged article family should be judged against these questions.

1. Did it remain grossly coherent after damage and exposure?
2. Did the flaw stay bounded or escalate rapidly?
3. Did the thermal response remain interpretable?
4. Did the full passive stack still outperform simpler damaged comparisons?
5. Is it worth carrying into later architecture decisions?

---

## Planned Advancement Logic

### Advance by default
- Rank A
- Rank B

### Advance only if needed for comparison continuity
- Rank C

### Cut unless a very specific reason exists
- Rank D

---

## Stage Discipline Rule

No damaged article family may advance merely because the pristine stack looked strong.

Advancement must be tied to comparative damaged-state performance.
