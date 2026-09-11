# P6 Erdős–Hajnal — Round 11 Lean Feed / Finite Census

**Source:** `P6-LEAN-FEEDSTOCK-2026-08-06.json`  
**Flagship status:** `NOT CLOSED`  
**Historical novelty:** not established  
**Rule:** bounded exhaustive computations below are finite theorems about the stated finite models, **not** unbounded P6-Erdős–Hajnal results.

This packet is the later formalization-first continuation of the Six-Vertex Wall campaign. It adds four promoted finite packages and five new negative/falsification blades to the earlier 30-theorem Court bank.

## T11.1 — Anchored P5 interval-attachment classification
**Authority:** `BOUNDED EXHAUSTIVE + SYMBOLIC WITNESSES`

In the exact anchored complement-P6-free model used by the Round 11 verifier, suppose:

- `u` is adjacent to `x` and nonadjacent to `y`;
- `x,y` are nonadjacent;
- both `x,y` are complete to an induced `P5`;
- `u` has a nonempty proper neighborhood on that `P5`.

Then `N_{P5}(u)` is either a singleton or two consecutive path vertices.

Among the 30 nonempty proper signatures on the five path vertices, the exact surviving supports are

`{p1}`, `{p2}`, `{p1,p2}`, `{p3}`, `{p2,p3}`, `{p4}`, `{p3,p4}`, `{p5}`, `{p4,p5}`.

The source formalization plan is to encode signatures by `Finset (Fin 5)`, decide all 30 cases, and retain explicit complement-P6 witnesses for every rejected signature.

## T11.2 — Correct rank-three complement-comb obstruction census
**Authority:** `COMPLETE 2^15 ENUMERATION`

For the source-bound three-tooth complement-comb model with stable handles and two vertices per tooth, exhaustive enumeration of all

\[
2^{15}=32768
\]

Boolean configurations gives:

| class | count |
|---|---:|
| all configurations | 32,768 |
| P6-free | 27,088 |
| pairwise-rectangle-law compatible | 27,328 |
| contains induced P6 | 5,680 |
| rejected already by pairwise rectangle law | 5,440 |
| **pairwise-legal but still contains P6** | **240** |

The inclusion-minimal forcing patterns number **252**, falling into **8 symmetry orbits**.

This is an exact finite census. The unbounded lift is deliberately not promoted.

## T11.3 — H5 surviving attachment supports are local cliques
**Authority:** `COMPLETE 2046-SIGNATURE ENUMERATION`

For the tested 11-vertex `H5` seed, among all

\[
2^{11}-2=2046
\]

mixed attachment signatures:

- **2,015** force an induced complement-P6;
- **31** survive.

Every surviving support is a clique of size at most three and belongs to the following structural family:

- a rim singleton or rim edge, optionally together with the hub;
- the hub alone;
- a pendant leaf, optionally together with its parent.

This is a finite seed-classification theorem, not an arbitrary-graph attachment theorem.

## T11.4 — Dominating K3,3 private-representative cluster classification
**Authority:** `COMPLETE 2^15 ENUMERATION`

In the exact induced dominating `K_{3,3}` private-representative model of Round 11, exhaustive enumeration of the 15 possible edges among the six private representatives yields only **four** P6-free full extensions.

All four private graphs are cluster graphs:

1. empty;
2. X-side clique only;
3. Y-side clique only;
4. complete.

Exact census:

| class | count |
|---|---:|
| all private graphs | 32,768 |
| P6-free full extensions | 4 |
| private P4-free | 4 |
| private cluster graphs | 4 |
| private complete multipartite | 2 |

The corresponding homogeneous-set sizes are `6` for two survivors and `4` for two survivors.

---

# Round 11 negative / falsification blades

## N11.1 — P5 reduced-type purity is false

Every ordered pair of the **nine** surviving P5 interval types admits **both** adjacency states in the tested anchored model. Thus reducing individual attachments to nine interval types does not make the interaction between types pure.

There are `9^2=81` ordered type pairs, and every one has an edge witness and a nonedge witness in the finite model.

## N11.2 — Full local comb handles do not rescue P5-type purity

After restoring the full three-handle local comb system, all **81** surviving P5 type pairs still admit both adjacency states. The finite search checks **1,296** states.

Thus the missing global theorem cannot be obtained merely by adding the local handle incidences to the nine-type reduction.

## N11.3 — One-leaf H5 escalation is attachment-nonrigid

For all three one-leaf extension orbit types of the H5 seed—new leaf at the hub, at a rim vertex, or at an existing pendant—mixed attachment signatures remain. The survivor counts are respectively

\[
33,\quad35,\quad33.
\]

Each orbit search exhausts all `4094` mixed signatures.

## N11.4 — Pairwise complement-comb laws are incomplete

There exist exactly **240** source-bound three-cell configurations satisfying every pairwise rectangle rule while still containing an induced P6.

This is the finite falsifier explaining why the Round-9 pairwise crown machinery, although exact, is not by itself the global three-cell theorem.

## N11.5 — Private cluster components are not full modules

A P6-free extension of a surviving `K_{3,3}` private-layer cluster exists in which one nonprivate exterior vertex mixes on a connected private component.

One explicit source witness has private-edge mask `35`; the added vertex is adjacent to all three dominators and to private vertices `x0,y0,y1,y2`, while the private components are

`{x0,x1,x2}`, `{y0}`, `{y1}`, `{y2}`.

Hence “private layer is a cluster graph” does **not** imply those cluster components are modules of the full graph.

---

# Lean/formalization feed

The feed specifies a core API around:

- `InducedP6`;
- `OppositeAnchors`;
- `StableOn`;
- `defect`;
- `PurePair`.

Its highest-priority kernel sketches are:

1. `oneEdgeRectangle_forces_inducedP6` — T-006;
2. `defects_eq_or_disjoint` — T-021;
3. `trace_count_le_card_add_one` — T-023;
4. `stableSlice_large_purePair` — T-025.

Formalization order begins with T-006 and T-021–T-026, then the local corollaries, then T11.1/T11.3/T11.4/T11.2 and explicit negative witnesses.

## Court

Round 11 strengthens the finite local picture but does **not** solve the flagship. Its main message is sharper: the crown theorem is exact locally, and several tempting routes from local types to global purity have explicit finite falsifiers. Future progress must therefore exploit genuinely multi-cell/cotree/separator structure rather than re-proving pairwise purity.