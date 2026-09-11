# Erdős–Gyárfás power-cycle forge — MC cards

> Source packet: 2026-08-04. Status labels are preserved. `UNRUN` novelty means no historical novelty claim. Lean mission names in the source are missions, not kernel receipts.

## MC01 — Minimum-order connectedness
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** A counterexample of minimum order is connected.

**Proof / route.** If G has more than one component, every component inherits minimum degree at least 3. Any component is a smaller counterexample because every cycle is contained in one component.

**Claim hash.** `7e260e637af7457550b736827690266c5e7cb0bc8861473c3b063a42c0bfe2f9`

## MC02 — Proper-subgraph 2-degeneracy
**Status:** `PROVED_FROM_SOURCE_PREMISE`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** If every proper subgraph J of a minimum counterexample G has minimum degree at most 2, then every proper subgraph H of G is 2-degenerate.

**Proof / route.** Every nonempty subgraph J of H is itself a proper subgraph of G, hence has a vertex of degree at most 2.

**Claim hash.** `9f9869f0e2ff0c0aae56feef79eda508875e7c1633b462fd07df6e0afcb2dc77`

## MC03 — Universal-root elimination ordering
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** For every vertex r of a minimum counterexample G, the graph G-r admits a degeneracy ordering of width 2.

**Proof / route.** G-r is a proper subgraph, so apply MC02.

**Dependencies.** MC02

**Claim hash.** `9b782757103929f597408396d72dde59f9c6a91ed7f23b4b5d68f16c7fd4d753`

## MC14 — Three-core criticality
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** A minimum counterexample is a subgraph-minimal graph of minimum degree at least 3: its 3-core is the whole graph, while every proper subgraph has empty 3-core.

**Proof / route.** The first part is the target hypothesis. The second is equivalent to proper-subgraph 2-degeneracy.

**Dependencies.** MC02

**Claim hash.** `fb4b882ffca0ed0cfa3250e3eb661bf3d874c37887a9649f6ec456303ef60b8e`

## MC04 — Proper-set (2,3)-sparsity
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** For every proper vertex set S with |S| at least 2, e_G(S) is at most 2|S|-3.

**Proof / route.** The induced graph G[S] is 2-degenerate. A 2-degenerate graph on s>=2 vertices has at most 2s-3 edges by charging at most two later neighbors in a degeneracy ordering.

**Dependencies.** MC02

**Claim hash.** `48e9b98e823940ec327a24dbf1e16290c8de858414f5e6f3458877569f4fa7aa`

## MC05 — Global edge bound
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** If G has a degree-3 vertex, then |E(G)| is at most 2|V(G)|-2.

**Proof / route.** Delete a degree-3 vertex v. By MC04, G-v has at most 2(n-1)-3 edges. Restore the three incident edges.

**Dependencies.** MC04, DS01

**Claim hash.** `92ac0310f4bea3642653f64839e47a6973776d81c09faf7b720cd16b391b9279`

## MC06 — Average-degree barrier below four
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Every minimum counterexample satisfying MC05 has average degree strictly less than 4.

**Proof / route.** 2m/n <= (4n-4)/n = 4-4/n.

**Dependencies.** MC05

**Claim hash.** `9f0ad5aefc863c1f0527410698ffd68ae18def88d05a262ed45e7824e601e467`

## MC07 — Arboricity-two theorem
**Status:** `PROVED_USING_STANDARD_THEOREM`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Every minimum counterexample satisfying MC04-MC05 has arboricity at most 2.

**Proof / route.** For every proper nontrivial H, MC04 gives |E(H)|<=2|V(H)|-3; for H=G, MC05 gives |E(G)|<=2|V(G)|-2. Apply the Nash-Williams arboricity criterion.

**Dependencies.** MC04, MC05

**Claim hash.** `b85292cb620bd65d77dfd5106c5cbc330586aedd13684bb33889881de3071bf7`

## MC08 — Two-forest decomposition
**Status:** `PROVED_USING_STANDARD_THEOREM`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** The edge set of a minimum counterexample can be partitioned into two forests.

**Proof / route.** Equivalent formulation of MC07.

**Dependencies.** MC07

**Claim hash.** `3709e2935bec55d9e7631217d6120be1f34d0e1c0a84f3d36a0a6f49ff7f5163`

## MC09 — Two-parent orientation
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** A minimum counterexample admits an orientation with outdegree at most 2 and indegree at least 1 at every vertex; outgoing edges may be colored with two colors so that each monochromatic directed graph is acyclic and every vertex has at most one outgoing edge of each color.

**Proof / route.** Orient each of the two forest components toward arbitrary roots. Each vertex has at most one outgoing edge in either forest. Minimum degree at least 3 then gives indegree at least 1.

**Dependencies.** MC08

**Claim hash.** `4a620f2410e6e16fc7abbe794d8381b8010a07eeb5886f2d156dc2a68970678d`

## MC13 — Small-set edge-boundary lower bound
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** For every proper vertex set S with 2<=|S|<=5, the number of edges leaving S is at least 6-|S|.

**Proof / route.** The boundary size is sum_{v in S}d(v)-2e(S)>=3|S|-2(2|S|-3)=6-|S| by minimum degree 3 and MC04.

**Dependencies.** MC04

**Claim hash.** `5cf7719b294c8cd2d457c3b206a8dcc64bb77a679ec03d3bb552685d711061f5`

## MC10 — Exact degree-excess identity
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Let A be the degree-3 vertices and D=sum_{v:d(v)>=4}(d(v)-4). Then |A|-D = 4|V(G)|-2|E(G)|.

**Proof / route.** Write 2m=3|A|+4|B|+D and n=|A|+|B|, then rearrange.

**Claim hash.** `e068aeb2ddec2fb6e48cc15cd1a3be5bbc19b98c8259ecbe90440a0cb08aea22`

## MC11 — Dense-boundary cubic surplus
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** If |E(G)|=2|V(G)|-2, then |A|-D=4.

**Proof / route.** Substitute m=2n-2 into MC10.

**Dependencies.** MC10

**Claim hash.** `2e0c61aa42115c7560713150a1903b048fa2185bcd08e385b53b8508febbc663`

## MC12 — Slack cubic surplus
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** If |E(G)|<=2|V(G)|-3, then |A|-D>=6.

**Proof / route.** Substitute the edge inequality into MC10.

**Dependencies.** MC10

**Claim hash.** `0fcc049109b7392949efa5a54522cd8f3d9a173f2549c34045c02f7bfd533f79`
