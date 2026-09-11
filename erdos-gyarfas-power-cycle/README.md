# Erdős–Gyárfás power-of-two cycle theorem forge

Public release of the 2026-08-04 `power-cycle-terminal-encirclement` theorem bank.

## Claim boundary

The flagship conjecture is **not claimed solved**. The source bank contains 102 exact theorem cards: 59 `PROVED_IN_PACKET`, 3 `PROVED_NEGATIVE_THEOREM`, 2 `PROVED_USING_STANDARD_THEOREM`, 1 `PROVED_FROM_SOURCE_PREMISE`, 2 `SOURCE_DERIVED`, 2 `CONDITIONAL_DEDUCTION`, 25 `UNPROVED_CHECKABLE_TARGET`, 6 `REFUTED_ROUTE`, and 2 `WITHDRAWN_UNSUPPORTED`. It also contains 24 finite/computational targets, 14 complete proof programs, 67 Lean missions, and 102 novelty missions.

**Novelty was UNRUN in the source packet. Lean names are formalization missions, not receipts.** This release therefore publishes the mathematics and its original authority labels without promoting any card to a historical-novelty or kernel-verified claim.

## Files

- `minimal-counterexample.md` — MC cards: minimality, sparsity, degree census.
- `dyadic-avoidance.md` — CY cards: C4/C8 and dyadic-cycle exclusions.
- `degree-defect-quotient.md` — DS cards: cubic/high-degree partition, exact surplus, bounded defect kernel, quotient/lifting.
- `transition-matching.md` — TR cards: matching contraction, switching cycles, exchange congruences.
- `boundary-routing.md` — BR cards: boundary pairing and residue leakage.
- `open-targets.md` — TG cards: explicit unproved closure targets.
- `negative-bank.md` — NG cards: refuted/withdrawn route mathematics retained permanently.
- `programs-and-computation.md` — 14 proof programs and 24 finite/computational targets.

The point of this package is not to inflate a theorem count. It is to expose the exact local theory, its dependencies, and its remaining wall so every statement can be independently attacked.
