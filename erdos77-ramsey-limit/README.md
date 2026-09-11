# Erdős #77 — diagonal Ramsey exponential-limit program

This directory is a **research-program mirror** for work on the existence and value of the exponential growth rate of diagonal Ramsey numbers.

The main mathematical record is `CHECKABLE-THEOREM-LEDGER.md`, containing **23 theorem / negative-theorem assets**. The parent limit problem remains open; the proved and conditional child results have their own exact scopes.

## Main proved structure

The program includes:

- the thin-corridor inequality
  `r(n-a,n) <= R(n) <= 4^a r(n-a,n)`;
- equivalence of diagonal exponential growth with any sublinear off-diagonal corridor;
- an inverse homogeneous-set formulation through the extremal function `h(N)`;
- clone-saturation structure for extremal Ramsey colourings;
- a weighted wrong-pair inequality;
- summable accumulation of sublinear composition error;
- explicit polarity digraph constructions;
- XOR/direct-sum identities;
- exact pattern-collision and triangular-orthogonality reductions;
- an exact tensor-flag rank formula;
- bilinear mixer algebra and rank-weighted first-moment formulas;
- a perfect-matching construction in the valid-pair incidence graph;
- a matching-restricted polarity digraph eliminating the largest repeated-coordinate fibers.

## Negative structural results

Several routes are eliminated precisely rather than rhetorically:

- raw tuple-counting plus a uniform-rank bound has an explicit exponent barrier;
- two cross matrices have an explicit information-budget ceiling in the investigated architecture;
- the full Cartesian mixed product contains large exact independent coordinate fibers and therefore cannot serve as the desired composition operator without further restriction.

These are architecture-specific impossibility statements, not global claims that Ramsey composition is impossible.

## What remains

The central missing theorem is an approximate-supermultiplicative composition result with sufficiently small parameter loss (or an equivalent container/rank theorem). The ledger proves the implication from such a composition theorem to existence of the exponential limit, but not the needed hypothesis itself.

## Repository status

This program is repository-scale and should ultimately have one dedicated home. A zero-commit public shell named `jaredwilder/diagonal-ramsey-corridor` exists and is a plausible intended destination; until that mapping is confirmed and the shell is initialized, this directory is the clearest human entry point.
