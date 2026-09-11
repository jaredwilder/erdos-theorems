# Erdős #477 — square-image tiling obstruction, verified Lean receipt

**Author:** Jared Wilder  
**Public formal-receipt release:** 2026-09-11

Recovered source path:

```text
oracle/evidence/msl-machine/campaigns/erdos477-campaign-001/kernel/Erdos477NoSquareTiling.lean
```

The historical kernel runner reports:

```text
status=VERIFIED
backend=wsl
exitCode=0
seconds=3.7
needsMathlib=true
project=/root/erdosfire-bench/proofs
```

Verified declarations:

```text
erdos477_sq_sub_sq_of_mod_four
erdos477_no_square_tiling
```

Axiom footprints:

```text
erdos477_sq_sub_sq_of_mod_four : [propext, Quot.sound]
erdos477_no_square_tiling      : [propext, Classical.choice, Quot.sound]
```

No `sorryAx` is present in the recorded verification result.

## Mathematical content

For the square image

\[
B=\{k^2:k\in\mathbb Z\},
\]

there is no finite `A⊂Z` giving a unique exact tiling `Z=A⊕B`. The proof uses the exact mod-4 characterization of differences of squares and the direct-sum uniqueness obstruction.

A human proof is public in `jaredwilder/unpublished-math-papers/validated-new-gold-ledger/` and a compact theorem statement in `jaredwilder/erdos-proved-lemmas`.

## Authority / novelty boundary

This is a **verified formalization** of the square/quadratic obstruction. The audit classifies the mathematical result as known externally; publication here establishes the formal artifact's provenance, not historical priority.

The exact original `.lean` bytes are still a source-recovery obligation; this file records the green receipt without reconstructing missing source text from snippets.
