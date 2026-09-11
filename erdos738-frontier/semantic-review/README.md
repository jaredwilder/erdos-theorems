# Erdős #738 — semantic review and formal-authority map

**Release date:** 2026-09-10  
**Source review:** deterministic semantic/novelty/relevance/Lean reviewer v0.3.0  
**Bank size:** 74 theorem-bank entries  
**Corpus manifest SHA-256:** `b024af1616220ba063c0d00e5ce66e6ebbd31cea6ccfbfb7bff66a565bcd3d7c`

This directory records the **authority map** for the already-public 74-entry Erdős #738 theorem bank. It does not upgrade any theorem, finite computation, or proposal. The purpose is the opposite: keep mathematical truth, kernel authority, novelty evidence, and target relevance separated.

## Review outcome

The frozen review inventory classified the 74 rows as follows:

| Novelty / relevance decision | Count |
|---|---:|
| `CERTIFIED_REFORMULATION | LOCAL_LEMMA` | 1 |
| `INSUFFICIENT_CORPUS | FINITE_ONLY` | 3 |
| `INSUFFICIENT_CORPUS | LOAD_BEARING_ADVANCE` | 1 |
| `INSUFFICIENT_CORPUS | LOCAL_LEMMA` | 49 |
| `INSUFFICIENT_CORPUS | REUSABLE_TECHNIQUE` | 6 |
| `INSUFFICIENT_CORPUS | STRUCTURAL_ADVANCE` | 6 |
| `INSUFFICIENT_CORPUS | TRIVIALIZED_BY_HYPOTHESES` | 8 |
| **Total** | **74** |

The reviewer produced **no global novelty claim** from the small literature seed corpus. That conservative outcome is intentional.

## Formal authority states

The review distinguishes the following states. They must not be conflated.

- `VERIFIED` — a general theorem built and passed the axiom policy.
- `FINITE_INSTANCE_ONLY` — a bounded certificate built; this is never promoted to a universal theorem.
- `COMPILED` — deterministic Lean project emitted, but kernel execution was intentionally skipped.
- `TOOLCHAIN_UNAVAILABLE` — runnable project emitted but no local Lake binding was available.
- `NO_RECIPE` — no deterministic formalization recipe; an exact formalization plan/obligation was emitted.
- `FAILED` — kernel, timeout, or axiom-policy failure.

A source theorem marked `PROVED_IN_PACKET` can therefore still have review authority `COMPILED`, `NO_RECIPE`, or `FINITE_INSTANCE_ONLY`. Source proof status and kernel status are different axes.

## Novelty states

The reviewer uses corpus-bound novelty decisions:

- `CERTIFIED_KNOWN`
- `CERTIFIED_REFORMULATION`
- `CERTIFIED_STRICTLY_STRONGER`
- `CERTIFIED_STRICTLY_WEAKER`
- `ORTHOGONAL_STRUCTURAL_ADVANCE`
- `NO_COLLISION_FOUND`
- `INSUFFICIENT_CORPUS`
- `UNDECIDED`

`NO_COLLISION_FOUND` is **not** global novelty. `INSUFFICIENT_CORPUS` means exactly what it says.

## Representative authority examples

### X12 — load-bearing target, not formalized

The frozen review assigns X12:

- source proof status: `UNPROVED_CHECKABLE_TARGET`;
- relevance: `LOAD_BEARING_ADVANCE`;
- novelty: `INSUFFICIENT_CORPUS`;
- Lean/formal authority: `NO_RECIPE`;
- magnitude card: proposal-only.

The reviewer records that X12 matches one registered load-bearing closure obligation semantically, but no formal implication certificate or general Lean theorem exists. It must therefore remain a **target**, not be quoted as a proved advance.

### P07 / P08 — reusable techniques, compiled route only

Representative P-series rows were classified as reusable techniques with `INSUFFICIENT_CORPUS` novelty. Their deterministic Lean projects were emitted with status `COMPILED`; that status is weaker than kernel verification.

### T09 — bounded formal authority only

A representative T-series construction received `FINITE_INSTANCE_ONLY`. The bounded Lean artifact cannot certify the universal statement.

## Reviewer invariants

The released reviewer contract enforced the following distinctions:

1. semantic theorem identity is normalized before comparison;
2. mathematical truth is never inferred from novelty or importance;
3. finite and universal authority are distinct;
4. undeclared axioms fail the Lean route;
5. literature comparison is corpus-bound;
6. hypothesis trivialization is audited separately from correctness;
7. target leverage is measured against a registered obligation graph, not prose similarity;
8. magnitude is orthogonal to validity.

## What this means for the #738 public bank

The 74 theorem-bank rows are useful mathematical ore, but they are **not 74 equivalent-strength theorems**. The public bank contains local lemmas, structural reductions, reusable proof techniques, finite-only objects, hypothesis-trivialized rows, and live targets. This authority map is the required companion to the raw bank.

The full Gyárfás–Sumner / Erdős #738 problem is not declared solved by this review.
