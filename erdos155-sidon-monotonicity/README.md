# Erdős #155 — Sidon one-step monotonicity, Lean rescue source

**Author:** Jared Wilder  
**Public recovery:** 2026-09-11

The mathematical theorem is

\[
\boxed{F(N+1)\le F(N)+1},
\]

where `F(N)` is the maximum size of a Sidon subset of `{1,...,N}` under the source file's diagonal-inclusive unordered-pair definition.

The proof is the deletion argument: from a Sidon subset of `{1,...,N+1}`, delete `N+1` if present. The remainder is a Sidon subset of `{1,...,N}` and at most one element was removed.

## Why this file is here

The archived formalization was recorded `KERNEL_FAILED`, but its cable receipt reports a syntactic source-layout failure: a duplicate/misplaced `import Mathlib` appeared after a `set_option` command. The recovered rescue source removes only that duplicate import and preserves the proof body.

`ERDOS155_R005_L1_RESCUE_UNCOMPILED.lean` is published verbatim from that repair.

## Authority boundary

**The repaired source has not been recompiled in the recovery runtime.** It must therefore be cited as a recovered Lean proof source awaiting kernel rerun, not as a new kernel-certified theorem.

The ordinary mathematical proof is independent of that status and is already public in the compact theorem bank.
