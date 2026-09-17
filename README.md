# Erdős Lean theorem bank

**79 kernel-checked Lean 4 declarations across 20 files and 15 Erdős problems.**

The counted formal core is [`theorems/`](theorems) together with [`MANIFEST.json`](MANIFEST.json). Every counted declaration has axiom footprint

```text
{propext, Classical.choice, Quot.sound}
```

with no `sorry`, no `native_decide`, and no project-declared axiom in the counted theorem files.

## Formal core

| problem | file | declarations |
|---|---|---:|
| cover-C13-6-3 | `Cover20Degree.lean` | 2 |
| erdos1061 | `Erdos1061Sigma.lean` | 2 |
| erdos1084 | `Erdos1084Lower.lean` | 12 |
| erdos276 | `Erdos276Corollary.lean` | 2 |
| erdos289 | `Erdos289Head.lean` | 5 |
| erdos289 | `msl_erdos289_a_m01_c1.lean` | 1 |
| erdos289 | `msl_erdos289_a_m01_c2.lean` | 1 |
| erdos313 | `Erdos313Head.lean` | 2 |
| erdos400 | `Erdos400Witness.lean` | 3 |
| erdos412 | `Erdos412Sigma.lean` | 4 |
| erdos456 | `Erdos456Equality.lean` | 2 |
| erdos477 | `Erdos477NoSquareTiling.lean` | 2 |
| erdos479 | `Erdos479Family.lean` | 1 |
| erdos479 | `Erdos479LTE.lean` | 2 |
| erdos700 | `Erdos700Semiprime.lean` | 2 |
| erdos885 | `Erdos885Duality.lean` | 1 |
| erdos936 | `Erdos936Congruence.lean` | 2 |
| erdos949 | `Erdos949Core.lean` | 4 |
| erdos949 | `Erdos949Hindman.lean` | 13 |
| erdos949 | `Erdos949HindmanFS.lean` | 16 |

A recount on 2026-09-11 gives exactly **20 files, 79 declarations, and 79 clean axiom reports**.

## Erdős #949

The largest formal group is the finite-sums material:

- `Erdos949Hindman.lean` proves a countable analogue using Mathlib's Hindman theorem;
- `Erdos949HindmanFS.lean` strengthens this to full finite sums.

Together they formalize the countable theorem and isolate the additional step required for the continuum formulation.

## Verification artifacts

Formal theorem files normally include:

- `.axioms.txt` — `#print axioms` output;
- `.sha256` — source hash;
- `.verify.json` — verification receipt.

`Erdos289Head.lean` has its source, hash, and clean axiom report but lacks the extra `.verify.json` file.

Each `.lean` file under `theorems/` can be compiled independently against Mathlib; its declaration footprints should agree with the shipped `.axioms.txt`.

## Other material

Top-level research mirrors are not part of the 79-declaration kernel count. [`RESEARCH-MIRRORS.md`](RESEARCH-MIRRORS.md) maps those larger programs to their subject repositories.

Related repositories:

- [`erdos152`](https://github.com/jaredwilder/erdos152) — statement formalizations and semantic audit;
- [`lean-semantic-blades`](https://github.com/jaredwilder/lean-semantic-blades) — source-fidelity checks.

## License

Apache-2.0.

Author: Jared Wilder.
