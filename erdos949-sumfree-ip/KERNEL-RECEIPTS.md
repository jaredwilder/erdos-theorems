# Erdős #949 — verified Lean source and receipt ledger

**Author:** Jared Wilder  
**Recovered kernel audit:** September 2026  
**Public formal release:** 2026-09-11

The exact historical/reverified Lean source is now public under

`theorems/erdos949-campaign-001/`.

The natural-language mathematics has a fuller public writeup at `jaredwilder/unpublished-math-papers/erdos949-sumfree-ip/`.

## 1. Sharp finite theorem — `Erdos949Core.lean`

Public source:

`theorems/erdos949-campaign-001/Erdos949Core.lean`

Public verification receipt:

`theorems/erdos949-campaign-001/Erdos949Core.verify.json`

Recorded kernel result:

```text
status=VERIFIED
backend=wsl
exitCode=0
seconds=76.5
needsMathlib=true
project=/root/erdosfire-bench/proofs
```

Declarations:

```text
erdos949_finite_core
erdos949_universal
erdos949_five_sharp
erdos949_five_sharp_real
```

Each declaration was reported clean with the ordinary Mathlib footprint

```text
[propext, Classical.choice, Quot.sound]
```

and no `sorryAx`.

The universal theorem is the sharp statement: for every sum-free `S⊂R`, some integer `q` with `1<=q<=5` has both `q` and `2q` outside `S`. The sharpness declarations certify the witness `{1,4,6}` showing that 5 cannot be replaced by 4.

## 2. Pairwise/countable theorem — `Erdos949Hindman.lean`

Public source:

`theorems/erdos949-campaign-001/Erdos949Hindman.lean`

Public verification receipt:

`theorems/erdos949-campaign-001/Erdos949Hindman.verify.json`

Recorded kernel result:

```text
status=VERIFIED
backend=wsl
exitCode=0
seconds=71.8
needsMathlib=true
project=/root/erdosfire-bench/proofs
```

Fourteen declarations were recorded, including

```text
erdos949_countable_analogue
erdos949_countable_analogue_control
```

The main theorem gives an infinite `A⊂N` outside `S` whose pairwise sums, including the diagonal case, stay outside `S`.

## 3. Full finite-sums upgrade — `Erdos949HindmanFS.lean`

This is the strongest formal theorem in the #949 packet.

Public source:

`theorems/erdos949-campaign-001/Erdos949HindmanFS.lean`

Public verification receipt:

`theorems/erdos949-campaign-001/Erdos949HindmanFS.verify.json`

Recorded re-verification result:

```text
status=VERIFIED
backend=scaleway-box
project=/root/mathlib4
exitCode=0
seconds=6.83
sorryFree=true
sha256=f4130c29f345afc9b264aa2331199433f6f0bfdd9dc7e224a49123a60970b9ac
replication runs=2
identicalOutput=true
```

Main declaration:

```text
erdos949_hindman_full_finite_sums
```

It proves: for every sum-free `S⊆R`, there is an infinite set `A` of positive naturals such that for **every nonempty finite subset** `T⊆A`, both

```text
sum T
2 * sum T
```

lie outside `S`.

Equivalently, the full nonempty finite-sums set `FS(A)` is disjoint from `S`, and so is its double. This strictly strengthens the earlier pairwise `A+A` statement.

The file re-derives `erdos949_countable_analogue` as a corollary, includes non-vacuity controls, is sorry-free, and was replayed twice with byte-identical stdout. The main theorem's axiom footprint is the ordinary Mathlib set

```text
[propext, Classical.choice, Quot.sound]
```

with no `sorryAx`.

## Authority boundary

These are **actual public Lean source files plus green verification receipts**, not prose descriptions of missing artifacts.

They establish formal verification in the recorded Mathlib environments. They do **not** establish historical novelty, and they do not solve the continuum-cardinality parent problem.
