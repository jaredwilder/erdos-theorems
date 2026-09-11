# erdos-theorems

Kernel-verified Lean 4 theorems produced while attacking open Erdős problems. **79 declarations across 20 files and 15 problems. Every declaration has a clean axiom footprint.**

Author: Jared Wilder. First public timestamp: 2026-09-10.

Companion repos:
- https://github.com/jaredwilder/erdos152 (formalized statements, mostly unproved, with defect audit)
- https://github.com/jaredwilder/lean-semantic-blades (the auditor)

## What "clean axiom footprint" means

Every declaration here was checked with `#print axioms` and depends on nothing outside

    {propext, Classical.choice, Quot.sound}

which is Lean's standard classical foundation. No `sorry`, no `native_decide`, no hand-declared axiom, no unverified import. Each file ships with its `.axioms.txt` naming the footprint of every declaration, its `.sha256`, and the kernel `.verify.json`.

**One exception, found by re-counting the repository on 2026-09-11 rather than trusting this paragraph:** `theorems/erdos289-campaign-001/Erdos289Head.lean` ships its `.axioms.txt` (five declarations, every one `[propext, Classical.choice, Quot.sound]`) but **no `.verify.json`**. It is the only file of the twenty missing one. The axiom footprint is present and clean; the kernel run receipt is not, so that file's footprint has not been re-confirmed here from a shipped kernel log.

The same re-count confirmed the rest: **20 files, 79 declarations, 79 clean footprints, 0 carrying any other axiom**, and the per-file table below matches the shipped axiom receipts file by file with no mismatches.

**Count of declarations here carrying any other axiom: 0.**

## Mathematical scope and standout result

These are proved theorems at the scopes of their statements: structural lemmas, bounds, finite exhaustions, special cases, and standalone consequences extracted from larger Erdős campaigns. Their status is determined by the theorem statement itself rather than inherited from the larger problem under which the theorem was discovered.

The result worth singling out is `Erdos949Hindman.lean`: a countable analogue of Erdős problem 949, proved via Mathlib's Hindman theorem in 13 declarations with a clean footprint and a non-vacuity control. `Erdos949HindmanFS.lean` extends this to full finite sums in 16 declarations. Together they isolate the countable theorem cleanly and identify the jump to the continuum formulation as the remaining larger-problem frontier.

As far as the author can determine, this countable formulation is not recorded on the problem's page. That records the result of the author's search; historical novelty remains a separate literature question.

## Verifying this yourself

Each `.lean` file is self contained against Mathlib. Compile it and run `#print axioms` on any declaration; the result should match the shipped `.axioms.txt`. If it does not, the file is wrong and an issue is welcome.

## Contents

| problem | file | declarations | all clean axioms |
|---|---|---:|---|
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
