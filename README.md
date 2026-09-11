# Erdős Lean theorem bank

**79 kernel-verified Lean 4 declarations across 20 files and 15 Erdős problems.** Every declaration in the formal core has a clean axiom footprint.

Author: Jared Wilder. First public timestamp: 2026-09-10.

## Important repository-layout note

The **formal theorem-bank claim applies to `theorems/` and `MANIFEST.json`**, not automatically to every top-level file or directory in this repository.

During the September 11 public-release sweep, several larger Markdown/JSON research programs were also mirrored into top-level directories here: Erdős–Gyárfás power cycles, #271 Stanley sequences, #500 Turán `(3,4)`, #595 fiber coherence, #738 frontier work, #77 Ramsey asymptotics, #1093 divisor-window material, and others.

Those are valuable public mathematics, but repository location does **not** make them kernel-verified. Several have also become too large to remain editorially buried inside a repo whose primary identity is formal proof.

See [`RESEARCH-MIRRORS.md`](RESEARCH-MIRRORS.md) for the routing map. The governing rule is:

> **formal proof status follows the formal artifact; mathematical subject identity follows the problem/program.**

Program-scale mirrors are being promoted toward focused subject repositories. Compact ordinary-math statements may instead route through `jaredwilder/erdos-proved-lemmas`; provenance archives remain provenance archives.

Companion repositories:
- https://github.com/jaredwilder/erdos152 — statement formalizations and semantic audit;
- https://github.com/jaredwilder/lean-semantic-blades — source-fidelity checks for formalizations.

## Axiom footprints of the formal core

Every declaration counted in the formal bank was checked with `#print axioms` and depends only on

```text
{propext, Classical.choice, Quot.sound}.
```

There is no `sorry`, no `native_decide`, and no hand-declared project axiom in the counted theorem files.

Each formal theorem file normally ships with:

- `.axioms.txt` — the axiom footprint of its declarations;
- `.sha256` — file hash;
- `.verify.json` — verification record.

One file, `theorems/erdos289-campaign-001/Erdos289Head.lean`, has its `.axioms.txt` but no `.verify.json`. Its five declarations all have the standard clean footprint; the missing item is the extra stored verification record, not the theorem source or axiom report.

A recount on 2026-09-11 confirmed **20 formal files, 79 declarations, 79 clean footprints, and zero counted declarations carrying any other axiom**.

## Mathematical contents of the formal core

The Lean files contain structural lemmas, bounds, finite results, special cases, and standalone consequences arising from work on larger Erdős problems. Each statement has the scope written in the theorem itself.

A particularly substantial formal group is the Erdős 949 material:

- `Erdos949Hindman.lean` proves a **countable analogue** via Mathlib's Hindman theorem in 13 declarations, together with a non-vacuity check;
- `Erdos949HindmanFS.lean` strengthens this to **full finite sums** in 16 declarations.

These formalize a complete countable theorem and isolate the additional step required to reach the continuum formulation of the original problem.

The countable formulation was not found on the problem page during the author's literature check; comprehensive historical priority remains a separate literature question.

## Reproducing the formal checks

Each `.lean` file under `theorems/` is self-contained against Mathlib. Compile a file and run `#print axioms` on any declaration; the result should agree with the shipped `.axioms.txt`.

## Counted formal files

| problem | file | declarations | clean axiom footprint |
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
