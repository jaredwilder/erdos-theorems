# Research mirrors inside `erdos-theorems`

**Author:** Jared Wilder  
**Repository hygiene note:** 2026-09-11

`erdos-theorems` was created as a **Lean theorem bank**. Its canonical formal core is the `theorems/` directory together with `MANIFEST.json`, the `.axioms.txt` files and the stored verification receipts.

During the September 11 release, additional research packets were copied into top-level directories of this repository. Those packets are useful public mathematics, but they are **not part of the 79-declaration kernel-verified count merely because they live in this repository**.

This file records their role so repository location cannot accidentally upgrade proof status or bury a program that deserves its own mathematical home.

## Formal core

The following surface defines the repository's formal theorem-bank claim:

- `theorems/`
- `MANIFEST.json`
- theorem-specific `.lean`, `.axioms.txt`, `.verify.json` and hash files

The README's count of 79 clean declarations refers to that formal core only.

## Program-scale mirrors awaiting dedicated homes

These top-level research subtrees have crossed the threshold where they should be read as mathematical programs rather than miscellaneous theorem-bank attachments:

- `erdos-gyarfas-power-cycle/` — power-of-two-cycle program with theorem banks, ear-extension material, transition structure, computations, negative results and open targets;
- `erdos142-ap-free/` — 124-record / 53-round audited progression-free-set program with exact convex-level construction, carry-free transfer, several architecture-specific barriers, a dyadic reciprocal-sum implication and an exact finite certificate target;
- `erdos271-stanley/` — full 184-entry audited Stanley-sequence ledger;
- `erdos500-theorem-forge/` and `erdos500-turan34/` — 76-record Turán `(3,4)` program plus machine-readable packages;
- `erdos595-coherence/` and `erdos595-fiber-coherence/` — major portions of the 216-record fiber-coherence / cycle-rank / finite-kernel program;
- `erdos738-frontier/` — large #738 frontier/theorem-bank material, recursive data and semantic review;
- `erdos77-ramsey-limit/` — 23-asset diagonal-Ramsey asymptotic/corridor program;
- `erdos1093-divisor-window/` — problem-scale #1093 divisor-window material that belongs with the #890↔#1093 program;
- `p6-erdos-hajnal/` — 30-asset P6 Erdős–Hajnal structural program with bounded finite verification and explicit remaining obligations.

Human entry-point READMEs now exist for #142, #500, #595 coherence/fiber coherence, #738, #77 and P6 so readers do not need to infer the mathematics from historical bank filenames.

These programs should migrate, or be canonically superseded, by focused problem/program repositories. They may remain here as public mirrors/provenance after promotion, but this repository should not be their permanent editorial front door.

## Compact mathematical mirrors

These are currently small enough that a compact theorem bank or focused formal home is more sensible than another standalone repository:

- `erdos243-deviation-series/`;
- `erdos247-sparse-binary/`;
- `erdos289-reciprocal-sums/`;
- `erdos885-factor-differences/`.

Where a human theorem statement is already routed to `jaredwilder/erdos-proved-lemmas`, that bank should be the preferred ordinary-math reading surface while the Lean declarations remain under `theorems/` here.

## Archive mirrors that belong conceptually in provenance repositories

- `long-tail/`;
- `msl-day2-2026-09-02/`.

These preserve useful release material but are archive/provenance objects, not formal-theorem-bank content. `jaredwilder/msl-ore-estate` is the natural estate-level provenance home.

## Authority rule

Repository location never upgrades mathematical authority.

A Markdown theorem ledger under a top-level mirror is not Lean-certified unless a corresponding declaration in `theorems/` has actually been checked and its axiom footprint recorded. Conversely, a genuine ordinary proof does not become less useful because it is not formalized.

The public organization should expose both facts clearly:

> **formal proof status follows the formal artifact; mathematical subject identity follows the problem/program.**

## Promotion rule

When a focused subject repository is initialized:

1. move or reproduce the human-facing research map there;
2. retain exact source/provenance links back to this mirror where useful;
3. keep actual Lean theorem files in the formal theorem bank unless the subject repo intentionally vendors them too;
4. update the release indexes so the subject repository is the preferred citation surface;
5. do not delete history merely to make the tree cosmetically clean.
