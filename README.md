# erdos-theorems

Kernel-verified Lean 4 theorems produced while attacking open Erdos problems. **79 declarations
across 20 files and 15 problems. Every declaration has a clean axiom footprint.**

Author: Jared Wilder. First public timestamp: 2026-09-10.

Companion repos:
- https://github.com/jaredwilder/erdos152 (formalized statements, mostly unproved, with defect audit)
- https://github.com/jaredwilder/lean-semantic-blades (the auditor)

## What "clean axiom footprint" means

Every declaration here was checked with `#print axioms` and depends on nothing outside

    {propext, Classical.choice, Quot.sound}

which is Lean's standard classical foundation. No `sorry`, no `native_decide`, no hand-declared
axiom, no unverified import. Each file ships with its `.axioms.txt` naming the footprint of every
declaration, its `.sha256`, and the kernel `.verify.json`.

**Count of declarations here carrying any other axiom: 0.**

## What this does and does not claim

These are proved theorems. They are **not** solutions to the Erdos problems they sit under. Most
are lemmas, bounds, finite exhaustions, special cases, or structural results obtained on the way to
a problem that remains open. Read each statement; it says exactly what it proves.

The one result worth singling out: `Erdos949Hindman.lean` proves a countable analogue of Erdos
problem 949, via Mathlib's Hindman theorem, in 13 declarations with a clean footprint, together
with a non-vacuity control. `Erdos949HindmanFS.lean` extends it to full finite sums in 16. This
isolates the jump from countable to continuum as the remaining difficulty in that problem. As far
as the author can determine it is not recorded on the problem's page, which is a statement about
the author's search and not a novelty claim adjudicated by anyone else.

## Verifying this yourself

Each `.lean` file is self contained against Mathlib. Compile it and run `#print axioms` on any
declaration; the result should match the shipped `.axioms.txt`. If it does not, the file is wrong
and an issue is welcome.

## Contents

| problem | file | declarations | all clean axioms |
|---|---|---|---|
| cover-C13-6-3 | `Cover20Degree.lean` | 2 | yes |
| erdos1061-campaign-001 | `Erdos1061Sigma.lean` | 2 | yes |
| erdos1084-harborth-2026-09-02 | `Erdos1084Lower.lean` | 12 | yes |
| erdos276-campaign-001 | `Erdos276Corollary.lean` | 2 | yes |
| erdos289-campaign-001 | `Erdos289Head.lean` | 5 | yes |
| erdos289-campaign-001 | `msl_erdos289_a_m01_c1.lean` | 1 | yes |
| erdos289-campaign-001 | `msl_erdos289_a_m01_c2.lean` | 1 | yes |
| erdos313-campaign-001 | `Erdos313Head.lean` | 2 | yes |
| erdos400-campaign-001 | `Erdos400Witness.lean` | 3 | yes |
| erdos412-campaign-001 | `Erdos412Sigma.lean` | 4 | yes |
| erdos456-campaign-001 | `Erdos456Equality.lean` | 2 | yes |
| erdos477-campaign-001 | `Erdos477NoSquareTiling.lean` | 2 | yes |
| erdos479-campaign-001 | `Erdos479Family.lean` | 1 | yes |
| erdos479-campaign-001 | `Erdos479LTE.lean` | 2 | yes |
| erdos700-campaign-001 | `Erdos700Semiprime.lean` | 2 | yes |
| erdos885-campaign-001 | `Erdos885Duality.lean` | 1 | yes |
| erdos936-campaign-001 | `Erdos936Congruence.lean` | 2 | yes |
| erdos949-campaign-001 | `Erdos949Core.lean` | 4 | yes |
| erdos949-campaign-001 | `Erdos949Hindman.lean` | 13 | yes |
| erdos949-campaign-001 | `Erdos949HindmanFS.lean` | 16 | yes |

## License

Apache-2.0.
