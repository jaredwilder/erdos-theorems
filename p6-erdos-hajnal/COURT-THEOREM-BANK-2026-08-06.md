# The Six-Vertex Wall — P6 Erdős–Hajnal Court Theorem Bank

**Campaign:** 2026-08-06  
**Flagship:** every induced-`P6`-free graph has a polynomial-size clique or stable set  
**Court:** **FLAGSHIP NOT CERTIFIED**  
**Certified local frontier in this campaign:** stable two-tooth crown normal form.

This file publishes all **30 Court theorem assets** from the ten-round campaign. Published inputs, negative/retracted routes, candidates and close programs are separated into companion files so dependency boundaries remain visible.

## T-001 — P6 leaf-reducibility
**Status:** `COURT — elementary proof`

The singleton family `{P6}` is leaf-reducible: deleting an endpoint leaves `P5`, for which the Erdős–Hajnal property is a published input.

## T-002 — Correct two-wall reduction
**Status:** `COURT — conditional reduction`

If `{P6}` is wonderful and has property `(*)`, then `P6` has the Erdős–Hajnal property. This is a dependency composition, not a claim that either missing wall has been discharged.

## T-003 — Diameter-four wonderfulness barrier
**Status:** `COURT — elementary proof`

A one-subdivision of `K_{1,t}` contains no induced `P6`: its diameter is at most four, while the endpoints of an induced `P6` are at graph distance five.

## T-004 — Small auxiliary-witness barrier
**Status:** `COURT — elementary proof`

No graph `H` on at most five vertices can witness the second wonderfulness criterion for `{P6}`. For fewer than five vertices the required extensions are too small; at five vertices the added vertex has degree two while the complement of `P6` has minimum degree three.

## T-005 — Mixed-component purification
**Status:** `COURT — elementary proof`

Contracting connected components of a blockade mixedness graph gives pairwise pure quotient blocks: a mixed quotient pair would contain an original mixed pair joining two components.

## T-006 — Forbidden single-edge rectangle
**Status:** `COURT — proved and bounded-verified`

Under nonadjacent comb handles, stable pairs `x,x'` and `y,y'` cannot have exactly one cross-edge. With unique edge `x'y`, the order

`x – a_j – x' – y – a_i – y'`

forms an induced `P6`. All four orientations were exhaustively checked in the campaign verifier.

## T-007 — Crossing domination
**Status:** `COURT — corollary`

A distinguishing vertex across a nonadjacent pair forces adjacency on every suitable common-nonneighbor column; otherwise T-006 appears.

## T-008 — Stable-handle rectangle exclusion
**Status:** `COURT — corollary`

Every tooth pair indexed by a stable handle family satisfies T-006 on internal nonedges.

## T-009 — Common-nonneighbor / symmetric-difference completeness
**Status:** `COURT — proved`

For nonadjacent `x,x'`, their common nonneighbors in `Y` are complete to the vertices distinguishing `x` and `x'`. A missing edge would make a forbidden one-edge rectangle.

## T-010 — Canonical pure-pair trichotomy
**Status:** `COURT — quantitative corollary`

For a threshold `t`, either a `t`-by-`t` complete pair exists, or the common-nonneighbor set has size `<t`, or the neighborhood symmetric difference has size `<t`.

## T-011 — Sparse-neighborhood twin forcing
**Status:** `COURT — quantitative corollary`

If every `x` has at most `rho |Y|` neighbors, `rho<1/2`, then absent a large complete pair every internal nonedge has small `Y`-neighborhood symmetric difference.

## T-012 — Separated profiles form a clique
**Status:** `COURT — metric lemma`

If every internal nonedge has profile distance `< epsilon |Y|`, then any `epsilon |Y|`-separated profile family is a clique.

## T-013 — Neighborhood profile cover
**Status:** `COURT — metric lemma`

The profile family is covered by at most `omega(X)` Hamming balls of radius `epsilon |Y|`: a maximal separated set is a clique by T-012.

## T-014 — Polynomial near-twin cluster
**Status:** `COURT — quantitative corollary`

If `omega(X)<|X|^gamma`, one profile ball contains more than `|X|^(1-gamma)` vertices.

## T-015 — Error crossing domination
**Status:** `COURT — proved`

On a template-zero region, a distinguishing error between nonadjacent rows forces secondary errors across every suitable column nonedge; otherwise T-006 occurs.

## T-016 — Low-degree agreement
**Status:** `COURT — proved`

After removing columns within `2 epsilon |Y|` of complete, nonadjacent rows in a near-twin cluster have identical error supports. A disagreement plus T-015 would force too many nonneighbors into the two sparse error sets.

## T-017 — Trimmed exact-profile clique bound
**Status:** `COURT — proved`

Representatives of distinct trimmed exact profiles form a clique, so the number of profiles is at most `omega(C)`.

## T-018 — Trimmed type-to-pure-pair bridge
**Status:** `COURT — proved`

A large near-twin cluster and a large trimmed region contain a large complete or anticomplete pair under a clique bound: choose a large exact-profile class and then its common neighborhood or common nonneighborhood.

## T-019 — Joint-profile quadratic sufficiency
**Status:** `COURT — conditional bridge`

If each tooth has at most `ell^2` exact joint profiles, choosing a largest class gives a pure refinement of width at least `w/ell^2`. The implication is exact; the `ell^2` premise was not proved.

## T-020 — Stable-tooth laminarity
**Status:** `COURT — true but superseded`

Stable-slice row nonneighbor traces are laminar. T-021 strengthens this.

## T-021 — Disjoint-defect classification
**Status:** `COURT — proved and bounded-verified`

Any two distinct nonempty stable-slice row defect sets are disjoint. Laminarity plus the fact that proper nonempty containment itself gives T-006 eliminates the nesting branch. Exhaustively checked through `4x4` stable matrices.

## T-022 — Complete-minus-disjoint-rectangles normal form
**Status:** `COURT — proved and bounded-verified`

Every stable interaction is a complete bipartite graph minus disjoint complete bipartite holes `S_r x D_r`, obtained by grouping rows by their common defect set.

## T-023 — Sharp trace bound
**Status:** `COURT — proved and bounded-verified`

The number of distinct row traces is at most `|T|+1`: each nonempty disjoint defect consumes a distinct column, plus the empty trace.

## T-024 — Dual pure-pair certificate
**Status:** `COURT — proved`

Every nonuniversal row class `S_r` is anticomplete to its defect block `D_r` and complete to `T\D_r`.

## T-025 — Guaranteed stable-slice pure pair
**Status:** `COURT — exact quantitative theorem`

There exists a pure pair with side sizes at least

\[
\frac{|S|}{|T|+1}
\quad\text{and}\quad
\frac{|T|}{2}.
\]

Choose a largest trace class using T-023 and the larger of its defect and complement using T-024.

## T-026 — Crown normal form
**Status:** `COURT — proved`

After merging equal profiles, the stable interaction is a blow-up of `K_{q,q}` minus `q` matching edges, with optional universal blocks.

## T-027 — Dominator size dichotomy
**Status:** `COURT — conditional on published dominating-core theorem`

A connected `P6`-free graph with a `P4`-free dominating set `D` of size at least `n^(2 theta)` contains a homogeneous set of size at least `n^theta`. The reason is that cographs are perfect, so `alpha(D) omega(D) >= |D|`.

## T-028 — Recursive anchors form a clique
**Status:** `COURT — proved`

In nested open-neighborhood recursion, all selected anchors are pairwise adjacent because every later anchor lies in every earlier retained neighborhood.

## T-029 — Nested-neighborhood size ledger
**Status:** `COURT — schema with rounding caveat`

Under denial of an `n^theta` homogeneous set, `r` nested-neighborhood recursion rounds retain roughly `n^(1-2r theta)` vertices. Exact floors and `+/-1` terms remain to be formalized.

## T-030 — Cotree union-node activation
**Status:** `COURT — conditional local bridge`

At an anticomplete split of a dominating cograph, subordinate stable pairs with the required anchor incidences obey T-006. Every incidence needed by the assignment must be certified.

## Bounded verifier receipt

The packaged deterministic verifier reports `PASS` on the canonical local witness and exhaustively checks stable matrices through `4x4`:

| rows | cols | matrices | survivors | result |
|---:|---:|---:|---:|:---:|
| 2 | 2 | 16 | 12 | PASS |
| 2 | 3 | 64 | 34 | PASS |
| 2 | 4 | 256 | 96 | PASS |
| 3 | 2 | 64 | 34 | PASS |
| 3 | 3 | 512 | 128 | PASS |
| 3 | 4 | 4,096 | 466 | PASS |
| 4 | 2 | 256 | 96 | PASS |
| 4 | 3 | 4,096 | 466 | PASS |
| 4 | 4 | 65,536 | 2,100 | PASS |

Every bounded survivor satisfies the crown normal form. This is finite Court evidence and a regression guard; it is **not** an unbounded proof of P6-Erdős–Hajnal.
