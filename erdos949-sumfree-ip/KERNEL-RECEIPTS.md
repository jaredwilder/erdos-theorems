# Erdős #949 — verified Lean receipt ledger

**Author:** Jared Wilder  
**Recovered kernel audit:** September 2026  
**Public formal-receipt release:** 2026-09-11

This directory records the already-executed Lean verification receipts for the #949 theorem cluster. The natural-language mathematics has a fuller public writeup at `jaredwilder/unpublished-math-papers/erdos949-sumfree-ip/`.

## 1. `Erdos949Core.lean`

Recovered source path:

```text
oracle/evidence/msl-machine/campaigns/erdos949-campaign-001/kernel/Erdos949Core.lean
```

Kernel runner result:

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

The theorem content is the sharp finite statement: for every sum-free `S⊂R`, some integer `q` with `1<=q<=5` has both `q` and `2q` outside `S`, together with the sharpness witness `{1,4,6}` showing 5 cannot be replaced by 4.

## 2. `Erdos949Hindman.lean`

Recovered source path:

```text
oracle/evidence/msl-machine/campaigns/erdos949-campaign-001/kernel/Erdos949Hindman.lean
```

Kernel runner result:

```text
status=VERIFIED
backend=wsl
exitCode=0
seconds=71.8
needsMathlib=true
project=/root/erdosfire-bench/proofs
```

Fourteen declarations were recorded, including:

```text
bsum_zero
bsum_succ
bsum_mem
bsum_add_mem
le_bsum
blk_succ_fst
blk_succ_snd
ypos_mem
blk_fst_strictMono
ypos_strictMono
ypos_add_mem
erdos949_countable_analogue
above
erdos949_countable_analogue_control
```

The main theorem `erdos949_countable_analogue` and the controlled strengthening `erdos949_countable_analogue_control` were both reported clean with footprint

```text
[propext, Classical.choice, Quot.sound]
```

and no `sorryAx`.

## Authority boundary

These are **green historical kernel receipts**, not merely source labels. They establish that the listed files compiled successfully under the recorded Mathlib environment with the listed axiom footprints.

The original `.lean` file bytes have not yet been recovered as standalone Library objects in the current release session. This receipt ledger therefore does not fabricate source files from partial extracts. Recovering and mirroring the exact source bytes remains a separate provenance task.

The continuum-cardinality parent problem is not claimed closed by these results.
