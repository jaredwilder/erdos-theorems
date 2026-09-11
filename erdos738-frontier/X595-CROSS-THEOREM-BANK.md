# Erdős #738 × #595 — Cross-Encirclement Theorem Bank

Recovered from `ERDOS-738-X-595-CROSS-ENCIRCLEMENT-THEOREM-FORGE-2026-08-04.md`.

This bank contains **44 theorem/negative-theorem records plus 3 explicit open targets**. Status labels are load-bearing. Conditional statements assuming `#738(T)` are not independent proofs of #738, and none of this closes #595.

## PROVED-IN-PACKET STRUCTURE

### Critical Bouquet Theorem
Every Erdős #595 witness contains an induced
\[
K_1\vee\Bigl(\bigsqcup_{n<\omega}Q_n\Bigr),
\]
where the `Q_n` are pairwise anticomplete finite triangle-free vertex-critical graphs with `chi(Q_n)>n`.

### Minimal-Transversal Centeredness Suffices
For a graph `G`, `tc(G)>aleph_0` iff every countable family of inclusion-minimal triangle transversals has nonempty intersection.

### Ordered Forward-Link Coloring Theorem
For a well-order `prec` of `V(G)`, let `N_prec^+(v)` be the forward neighborhood. If every forward link has chromatic number at most `kappa`, then `tc(G)<=kappa`.

### Finite Critical Link Extraction
If `G` is finite, `K4`-free and `tc(G)>k`, then `G` contains an induced cone over a finite triangle-free vertex-critical graph `Q` with `chi(Q)>k`.

### Maximal Triangle-Free / Minimal Transversal Duality
A spanning triangle-free subgraph `H` is edge-maximal iff `E(G)\E(H)` is an inclusion-minimal triangle transversal.

### Cone Sterility Theorem
For every triangle-free graph `H` with an edge, `K1 vee H` is `K4`-free and has triangle-cover number exactly `2`, regardless of `chi(H)` or its induced-tree complexity.

### Induced-Free Refinement Failure
The ordinary cover-to-partition refinement for edge-hereditary classes does not extend to induced-tree-free layers in general: `C4` is triangle-free and induced-`P4`-free, but deleting one edge produces an induced `P4`.

### Maximal-Layer Form of Erdős #595
`tc(G)>aleph_0` iff no countable family of maximal spanning triangle-free subgraphs covers `E(G)`.

### Induced Cone Lift
If `F` is induced in `G[N(v)]`, then `G[{v} union V(F)]` is the induced cone `K1 vee F`.

### Full-Neighborhood Chromatic Bound
For every graph,
\[
tc(G)\le\sup_v\chi(G[N(v)]).
\]

### Ambient Defect-Layer Inheritance
If `G` is covered by `m` triangle-free layers and one layer induces a tree `T` on `X`, every ambient extra edge on `X` lies in one of the other `m-1` layers. Hence the ambient defect graph on `X` has triangle-cover number at most `m-1`.

### Closed-Neighborhood Two-Layer Theorem
For every `K4`-free graph and vertex `v`,
\[
tc(G[N[v]])\le2.
\]
Equality holds exactly when `G[N(v)]` contains an edge; otherwise the value is at most one.

### Hereditary Edge-Deletion Layer Refinement
For any class of edge sets closed under taking subsets, every cover by `kappa` members refines to a partition by `kappa` members. In particular this applies to triangle-free layers and to layers avoiding `T` merely as a non-induced subgraph.

### Inter-Link Obstruction Principle
In a #595 witness, no single closed neighborhood and no countable family of closed neighborhoods carries all edges. Any construction/proof must control interactions among uncountably many links.

### Vertex-Cover Bound for K4-Free Graphs
If `S` is a vertex cover of a `K4`-free graph,
\[
tc(G)\le2|S|.
\]
Hence a countable vertex cover implies countable triangle decomposability.

### Cone-Free High-Cover Counterexample Extractor
If a finite `K4`-free induced-`(K1 vee T)`-free graph has `tc(G)>k`, then it has a triangle-free induced-`T`-free neighborhood of chromatic number greater than `k`.

### Critical Bouquet Sterility
For pairwise anticomplete triangle-free `Q_i`,
\[
tc\!\left(K_1\vee\bigsqcup_iQ_i\right)\le2,
\]
with equality when some `Q_i` has an edge.

### Chi-Bounded Cone-Transfer Principle
Let `F` be a family of triangle-free graphs. If every triangle-free graph containing no induced member of `F` has chromatic number at most `kappa`, then every `K4`-free graph containing no induced cone `K1 vee F` for `F in F` satisfies `tc(G)<=kappa`.

### Closed-Neighborhood Edge-Cover Bound
Let `ell(G)` be the least size of `S` with
\[
E(G)=\bigcup_{s\in S}E(G[N[s]]).
\]
For `K4`-free `G`,
\[
tc(G)\le2\ell(G)
\]
in cardinal arithmetic.

### Type-Tensor Extremality Is Triangle-Cover Sterile
Coning the parity-defect hosts from the #738 type-tensor package gives `K4`-free graphs with extremal link tensors but triangle-cover number exactly `2`.

### K4-Free Links Are Triangle-Free
Every neighborhood, and every forward neighborhood, in a `K4`-free graph is triangle-free.

### Exact Tree-Absorption Dictionary
For a triangle transversal `D`, `X` induces `T` in `G-D` iff the designated tree edges avoid `D` and every other edge of `G[X]` belongs to `D`.

### Finite High-Cover Link Extraction
If finite `K4`-free `G` has `tc(G)>k`, some neighborhood has chromatic number greater than `k`; for any prescribed ordering one may take a forward neighborhood.

### Ordered Link Parameter Upper Bound
Define
\[
\lambda_\triangle(G)=\min_{\prec}\sup_v\chi(G[N_\prec^+(v)]).
\]
Then
\[
tc(G)\le\lambda_\triangle(G).
\]

### Defect-Depth Descent
In an `m`-layer triangle-free cover, a tree induced in one layer has ambient defect cover depth at most `m-1`. Ambient purification can therefore be organized inductively by layer depth.

### Erdős #595 Link Theorem
Every `K4`-free graph with `tc(G)>aleph_0` has, under **every** well-order, an uncountably chromatic triangle-free forward link.

### Witness Link-Cover Dispersion
Every #595 witness has uncountable closed-neighborhood edge-cover number `ell(G)` and therefore no countable vertex cover.

### Arbitrarily High Link Chromatic Number with `tc=2`
For every cardinal `kappa` realized as `chi(H)` by a triangle-free graph `H`, there is a `K4`-free `G` with `tc(G)=2` and a vertex whose neighborhood has chromatic number `kappa`.

### Critical-Bouquet Complexity Is Still Two-Layer
The critical bouquet forced inside a #595 witness is itself two-layer coverable. The #595 obstruction lies in interaction with the rest of the witness, not in the bouquet alone.

### Localization–Dispersion Dichotomy
Every #595 witness simultaneously has an uncountably chromatic triangle-free forward link under every well-order and no countable closed-neighborhood family covering all edges. Vertex-chromatic complexity localizes while triangle-cover complexity remains globally dispersed.

### High-Cover Forward-Link Obstruction
If `tc(G)>kappa`, then for every well-order there is `v` with
\[
\chi(G[N_\prec^+(v)])>\kappa.
\]

## CONDITIONAL ON #738

### Conditional Forest-Bouquet Universality
Assuming the triangle-free Gyárfás–Sumner statement for every tree in a sequence `T_0,T_1,...`, every #595 witness contains an induced cone over the pairwise-antocomplete forest `bigsqcup_i T_i`.

### Transversal-Absorbed Tree Theorem
Assume #738(`T`) with chromatic bound `c(T)`. If `D` is a triangle transversal and `chi(G-D)>c(T)`, then some `X` induces `T` in `G-D`, and every ambient chord of that copy belongs to `D`.

### Conditional Cone Universality of #595 Witnesses
If #738 holds for a finite tree `T`, every #595 witness contains an induced `K1 vee T`.

### Tree-Rich Layer Product Theorem
Assume every triangle-free induced-`T`-free graph is `c`-colorable. If `G` is covered by `m` triangle-free induced-`T`-free layers, then
\[
\chi(G)\le c^m.
\]

### Induced-Tree-Free Layer-Cover Bound
Let `itc_T(G)` be the least number/cardinal of layers that are both triangle-free and induced-`T`-free. Under #738(`T`) with bound `c`,
\[
\chi(G)\le c^{itc_T(G)}.
\]

### Tree-Rich Maximal-Layer Interface
Conditional on #738(`T`), every maximal triangle-free spanning subgraph `H` with `chi(H)>c(T)` contains induced `T`; its ambient defects are exactly edges of the corresponding minimal transversal.

### Erdős #738-to-#595 Tree-Cone Transfer
If every triangle-free induced-`T`-free graph is `c(T)`-colorable, then every `K4`-free induced-`(K1 vee T)`-free graph has `tc(G)<=c(T)`.

### All-Finite-Trees Bouquet Consequence
Conditional on full #738, every #595 witness contains an induced cone over a countable forest having one component isomorphic to every finite tree.

### Countable-Layer Forced-Tree Corollary
Under #738(`T`), if a graph is countably covered by triangle-free layers and
\[
\chi(G)>c(T)^{\aleph_0},
\]
then every such cover has a layer containing induced `T`.

### Finite-Layer Forced-Tree Corollary
Under #738(`T`), if `G` has an `m`-layer triangle-free cover and `chi(G)>c(T)^m`, every such cover has a layer containing induced `T`.

## OPEN TARGETS

### Layer-Colored Defect Tensor Target
For a type-uniform path-induced tree copy in one layer, color each ambient defect by the first other layer containing it. Determine sharp support bounds, realizability and induced-subtree criteria for this `(m-1)`-colored tensor.

### Two-Layer Purification Target
Classify when a tree induced in one triangle-free layer can have its entire ambient defect graph in one other triangle-free layer without an induced copy surviving after reselection.

### Finite-Layer Gyárfás Hierarchy
Conjectural target: for every finite tree `T` and integer `m>=1`, there is `f(T,m)` such that every graph with `tc(G)<=m` and `chi(G)>f(T,m)` contains induced `T`. The case `m=1` is Erdős #738.

## NEGATIVE THEOREMS / KILLED ROUTES

### Local-Complexity Non-Sufficiency
No lower bound on chromatic number, criticality, induced-tree richness or type-tensor complexity of **one** `K4`-free link can by itself force `tc(G)>2`.

### No Automatic Blocker Duality for `itc_T`
Induced-`T`-freeness is not generally preserved under edge deletion, so blocker-centeredness duality and least-layer partition refinement for ordinary `tc(G)` cannot be imported unchanged.

### Local #738 Richness Does Not Carry #595 Complexity
A `K4`-free graph may contain in one link every finite configuration/critical block/contact-code/type-tensor pattern available in triangle-free graphs while the full graph still has `tc=2`.

## Court

This bank is a bridge between two open programs. The unconditional theorems describe triangle-cover structure and transfer mechanisms. The conditional tree results remain conditional on #738. Neither #738 nor #595 is declared closed.