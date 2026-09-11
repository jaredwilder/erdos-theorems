# The Six-Vertex Wall — Close Programs and Machine Missions

This file publishes the campaign's **18 end-to-end proof programs** and **12 machine missions**. A close program is a route map, not a theorem. Earned steps and missing implications are explicit.

## CP-01 — Published wonderfulness + property-(*) route
1. T-001 leaf reducibility.
2. Prove `P6` wonderful.
3. Prove `P6` property `(*)`.
4. Published reduction gives generalized niceness.
5. Published reduction gives `P6`-EH.

**Earned:** step 1 + published implications.  
**Missing:** wonderfulness and property `(*)`.

## CP-02 — Tooth-decomposition route
Construct residual/pure-quotient decompositions in every comb tooth, place residuals and quotient patterns in fixed EH classes, prove external purity, then invoke the published tooth criterion and CP-01.

**Earned:** T-005 purification operator and T-026 local crown classification.  
**Missing:** noncircular initial blocks and EH control of components/patterns.

## CP-03 — Direct wonderfulness / alternating-block path
Use the hard mixed-block branch to synthesize anchors or embed complement-`P6`; otherwise output a restricted set/pure blockade and conclude wonderfulness.

**Earned:** T-003/T-004 eliminate false shortcuts.  
**Missing:** C-006 or C-007.

## CP-04 — Direct polynomial Rödl bypass
Prove C-014: every `P6`-free graph has a polynomial-size `epsilon`-restricted induced subgraph. Apply the published EH/Rödl equivalence.

**Missing:** C-014.

## CP-05 — MWIS/chordal-completion to blockade
Use the published completion family, extract balanced clique-tree separation, translate interfaces back to original attachment types, then find a pure pair/restricted set and recurse or invoke CP-04.

**Missing:** C-001.

## CP-06 — Bounded-clique PMC separator induction
Assume no large clique, use bounded-clique separator/PMC control, choose a balanced separator, classify component neighborhoods, and extract a homogeneous pair or recurse.

**Missing:** C-020 and exponent-preserving recursion.

## CP-07 — Rectangle-to-property-(*) route
Extract many nonadjacent handles, orient tooth pairs sparsely, apply T-006 through T-018, synchronize joint profiles, and obtain a `w/ell^2` pure blockade.

**Earned:** complete local sparse-pair engine.  
**Missing:** C-010/C-011 and noncircular structured slices.

## CP-08 — Terminal Comb Theorem
Prove C-012 directly, use its terminals for property `(*)`, and combine with wonderfulness or CP-04.

**Missing:** C-012.

## CP-09 — Joint-profile `ell^2` route
Bound joint profiles by `ell^2`, apply T-019, obtain a pure refinement and conclude property `(*)`.

**Missing:** the `ell^2` bound. N-011 shows no purely local proof can supply it.

## CP-10 — Ferrers synchronization route
The intended chain was laminar stable matrices -> synchronized chain orders -> interval blockade. T-020 was earned, but N-012 killed the nontrivial staircase premise. This route is closed as a failed route.

## CP-11 — Crown normal form + structured slices
Prove C-013, apply T-021 through T-026, aggregate crown blocks, extract a homogeneous pair/pure blockade, then close property `(*)` or the Rödl route.

**Earned:** exact crown normal form.  
**Missing:** C-013 + global crown aggregation.

## CP-12 — Dominating-cograph entropy collapse
Use the published connected dominating cograph/P4 theorem. If the dominator is large, apply T-027; if small, partition exterior vertices by dominator neighborhood, exploit the cotree, and find a type/pure pair/restricted set/`P6` or induct.

**Missing:** C-016.

## CP-13 — Nested-neighborhood anchor recursion
Choose a heavy dominating anchor repeatedly and retain its neighborhood. T-028 makes the anchors a clique and T-029 tracks surviving mass.

**Status:** killed as a standalone route by N-015; the available recursion depth is only `O(1/theta)`.

## CP-14 — Terminal weighted-dominator route
Assign exterior mass to dominator vertices; recurse through cotree union/join nodes; use rectangle/crown structure at union nodes, accumulate clique-compatible mass at joins, and permit heavy-child reduction only with a strict potential drop.

**Earned:** published cograph core + T-030 + T-026.  
**Missing:** C-017/C-018/C-019.

## CP-15 — Viral closure route
Prove C-021 (few induced `P6` copies force a polynomial restricted set), apply the published viral/EH equivalence, conclude `P6`-EH.

**Missing:** C-021.

## CP-16 — Auxiliary-H wonderfulness criterion
Enumerate `H` with `|H|>=6`, require the two one-vertex extensions to contain complement-`P6`, prove `{H, complement-P6}` has EH, apply the wonderfulness criterion, then continue CP-01.

**Earned:** T-004 minimum-order barrier.  
**Missing:** C-022.

## CP-17 — Prime/minimal-counterexample modular induction
Take a smallest counterexample, use substitution closure to seek a prime structure, apply dominator/comb decomposition, use smaller EH instances, and contradict minimality.

**Missing:** guaranteed module or exponent-preserving composition.

## CP-18 — Hybrid separator-cotree campaign
Combine the published cograph core with MWIS/minimal-separator structure in exterior cells, apply T-006/T-026 at anticomplete cotree splits, use separator balance and aggregate at joins, then feed the polynomial Rödl route.

**Missing:** an interface theorem connecting cotrees, PMCs and original-graph pure pairs.

# Priority graph

**Direct:** dominating cograph/P4 core -> C-019 cotree transitions -> C-018 mass dichotomy -> polynomial homogeneous set.

**Framework:** T-001 + C-006/C-007 wonderfulness + C-012 comb theorem -> published property-(*) reductions.

**Bypass:** C-014 direct polynomial restriction or C-021 viral lemma -> published equivalence.

**Strongest verified blade:**

`T-006 -> T-021 -> T-022 -> T-023/T-025 -> T-026`.

# Machine missions

| ID | priority | mission / required output |
|---|---|---|
| M-01 | DONE | canonical six-vertex rectangle verifier; certify all four one-edge orientations as induced `P6` |
| M-02 | DONE | exhaust stable-slice matrices through `4x4`; every survivor must have crown normal form and sharp trace bound |
| M-03 | P0 | Lean-formalize T-006 and T-021–T-026 with semantic binding and clean axiom audit |
| M-04 | P0 | census two-anchor/two-cell configurations without stable-cell assumption; classify terminal/crown/reducible/obstruction |
| M-05 | P0 | three-cell cotree composition census; output minimal incompatible transitions and composition rules |
| M-06 | P0 | search for counterexamples to Cotree Mass Dichotomy; smallest weighted cotree survivor or candidate invariant |
| M-07 | P1 | auxiliary-H wonderfulness search for `|H|>=6`, with graph6/certificates and pair-EH checks |
| M-08 | P1 | search bounded combs for a smallest terminal-free survivor or produce UNSAT certificates |
| M-09 | P1 | PMC-to-pure-pair bridge campaign; separator statistics and candidate lift |
| M-10 | P1 | formalize exponent ledger / recursion and blockade losses in Lean or SMT arithmetic |
| M-11 | P2 | novelty review of the crown package with exact-claim/hash-bound receipt |
| M-12 | P2 | compile all close programs into a typed dependency graph with every missing step materialized exactly once |

The deterministic verifier for M-01/M-02 emitted `PASS`. The finite receipt is a regression guard, not a proof of the unbounded flagship.