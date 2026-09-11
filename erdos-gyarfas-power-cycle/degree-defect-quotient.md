# Erdős–Gyárfás power-cycle forge — DS cards

> Source packet: 2026-08-04. Status labels are preserved. `UNRUN` novelty means no historical novelty claim. Lean mission names in the source are missions, not kernel receipts.

## DS01 — Cubic-neighbor source premise
**Status:** `SOURCE_DERIVED`  
**Authority:** `COURT_SOURCE`  
**Novelty:** `UNRUN`

**Statement.** Every vertex of a minimum counterexample has a neighbor of degree exactly 3.

**Proof / route.** Imported as a source-derived premise from the minimal-counterexample campaign; this packet does not re-prove the published/source argument.

**Claim hash.** `efa920b1aa6ed79dd6fef0f4e98627e587fea130939e595516888cc8085c9463`

## DS02 — High-degree independence source premise
**Status:** `SOURCE_DERIVED`  
**Authority:** `COURT_SOURCE`  
**Novelty:** `UNRUN`

**Statement.** Vertices of degree at least 4 form an independent set in a minimum counterexample.

**Proof / route.** Imported as a source-derived premise from the minimal-counterexample campaign.

**Claim hash.** `a129a9d6356ebf6b1bf280f51a8f5177b9bc7c120a277d46f39c79f1f6c7740b`

## DS03 — Two-thirds cubic dominance
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Let A be the degree-3 vertices and B the vertices of degree at least 4. Then |A|>=2|B|.

**Proof / route.** Every a in A has at least one A-neighbor by DS01, so at most two B-neighbors; hence e(A,B)<=2|A|. By DS02, e(A,B)=sum_{b in B}d(b)>=4|B|.

**Dependencies.** DS01, DS02

**Claim hash.** `4592e2092d66e255a963c0c0936636368883f69488f873d96d898d0bd5668919`

## DS04 — High-degree mass bound
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Under DS01-DS02, sum_{b in B}d(b)<=2|A|; in particular |{b:d(b)>=r}|<=2|A|/r for every r>=4.

**Proof / route.** The crossing-edge count equals the degree sum over B and is at most two incidences per A-vertex.

**Dependencies.** DS01, DS02

**Claim hash.** `b8ae825177f7e6f977c4171b3fa8e2c92a016e5b4ad8e0ead696e9124736f8e1`

## DS05 — Exact cubic-surplus identity
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Let D=sum_{b in B}(d(b)-4) and S=sum_{a in A}(d_A(a)-1). Then 2(|A|-2|B|)=D+S.

**Proof / route.** Use e(A,B)=4|B|+D and 3|A|=2e(A)+e(A,B), while 2e(A)=sum d_A(a)=|A|+S.

**Dependencies.** DS01, DS02

**Claim hash.** `bfba841b9cf11143144733556e826033e1555fc5d7fc84de2ead0acf5b4a3761`

## DS06 — Cubic-skeleton parity law
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** The internal branching surplus S satisfies S congruent to |A| modulo 2.

**Proof / route.** S=sum(d_A(a)-1)=2e(G[A])-|A|.

**Dependencies.** DS05

**Claim hash.** `8fd11cd6107b100283b5ce83ae41f70bb8f7c0a8a55f02f178db0faafce1966b`

## DS07 — Component surplus formula
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Let c be the number of components and beta the cyclomatic number of G[A]. Then S=|A|-2c+2beta.

**Proof / route.** Since e(A)=|A|-c+beta, substitute into S=2e(A)-|A|.

**Dependencies.** DS06

**Claim hash.** `c2649c4d531a17391ce4436fbdcff569195325682fcbfb2c7aa3515795a1c8b8`

## DS14 — Strict cubic dominance
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Every noncubic minimum-order counterexample satisfies |A|>2|B|.

**Proof / route.** Combine DS03 and DS13.

**Dependencies.** DS03, DS13

**Claim hash.** `fff1b7b198be11965e393754063e8b093788f9b9ec4c871559c7c987e7d67e98`

## DS18 — Second ratio-branch elimination
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Every noncubic minimum-order counterexample satisfies |A|>=2|B|+2.

**Proof / route.** If |A|=2|B|+1, DS05 gives D+S=2. Parity forces D=S=1, contradicting DS17.

**Dependencies.** DS05, DS06, DS17

**Claim hash.** `aaa9871a27bc01ac1cc4ebc091b8f6690c24b3bca0e72fdb2aec9a7a758d5f21`

## DS08 — Nonmatching-component count bound
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Every connected component of G[A] other than K2 contributes at least 1 to S. Hence G[A] has at most S components that are not single matching edges.

**Proof / route.** A connected minimum-degree-at-least-1 graph has contribution 2e-v=0 exactly for K2; every other such component has contribution at least 1. Sum contributions to S.

**Dependencies.** DS07

**Claim hash.** `2cc09d4c126d37dc3e21359a2a3e2afec3716199f6efedfa381d8d62a896545e`

## DS09 — Bounded cubic defect kernel
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** All but at most 3S vertices of A lie in K2 components of G[A].

**Proof / route.** For a non-K2 tree component H, its surplus is |V(H)|-2, so |V(H)|=surplus+2; there are at most surplus such components. For a cyclic component, surplus=2e-v>=v. Summing gives at most 3S vertices outside K2 components.

**Dependencies.** DS08

**Claim hash.** `5c388d65862d356829fe7516569affe221ea1189c3e7d2e2b46fe34c0f2c5c78`

## DS10 — Ratio-surplus finite-kernel theorem
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** If |A|=2|B|+t, then D+S=2t, total high-degree excess is at most 2t, and all but at most 6t vertices of A lie in K2 components of G[A].

**Proof / route.** Apply DS05 and DS09.

**Dependencies.** DS05, DS09

**Claim hash.** `0f88a35c36a1b0ebd1cb33fbd8a3bffa3d0596e1f9462c1133afad0a2e5f5b36`

## DS17 — Minimum branching surplus
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Every noncubic minimum-order counterexample has S>=2.

**Proof / route.** DS16 gives at least two vertices in C. Every vertex in C contributes at least 1 to S.

**Dependencies.** DS16

**Claim hash.** `92f580c29760813b5070ddb0960e4db2c0e6d409d628f4d4f50fde388c0fb8a7`

## DS11 — Equality paired-incidence representation
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** If |A|=2|B|, then every b in B has degree 4, every a in A has d_A(a)=1, G[A] is a perfect matching, and G is obtained by subdividing every edge of a simple 4-regular graph H on B once and adding a perfect matching among the subdivision vertices.

**Proof / route.** DS05 forces D=S=0. Each a has two B-neighbors and defines an edge of H; parallel edges would create a 4-cycle. Degree four follows from D=0.

**Dependencies.** DS05, CY01

**Claim hash.** `33114cd254b238a6b23e83c90c418e0566c759aec58875dcb434f665a725f32a`

## DS12 — Equality quotient cycle doubling
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Every r-cycle of the quotient H in DS11 lifts to a 2r-cycle in G.

**Proof / route.** Insert the unique subdivision vertex on every quotient edge.

**Dependencies.** DS11

**Claim hash.** `46258891c352af829ce15f33b55ec1f6ce730d1b455961fde0cb813f81c7d164`

## DS13 — Equality branch elimination
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** A minimum-order counterexample cannot satisfy |A|=2|B|.

**Proof / route.** The quotient H from DS11 is a smaller 4-regular graph. Any power-of-two cycle in H doubles to a power-of-two cycle in G by DS12, so H would be a smaller counterexample.

**Dependencies.** DS11, DS12

**Claim hash.** `c30ebc7efa5bbcf76e4656133ea297f1da1ad4f86a6fd5354ffbab26ee82dba6`

## DS15 — Ordinary-cubic quotient
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Let M={a in A:d_A(a)=1} and C={a in A:d_A(a)>=2}. Form Q on B by replacing each a in M by an edge between its two B-neighbors. Then Q is simple, d_Q(b)=d_G(b)-|N(b) intersect C|, and every r-cycle of Q lifts to a 2r-cycle in G.

**Proof / route.** Each a in M has exactly two B-neighbors. Duplicate quotient edges create a 4-cycle. The degree and cycle-lift formulas are immediate.

**Dependencies.** DS01, DS02, CY01

**Claim hash.** `b43581dcd883ec5af2c499e2dc2ca45d36b268d7bde5f16e14e5ccedd25c4d51`

## DS16 — Branching-defect concentration
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** In every noncubic minimum-order counterexample, some b in B satisfies |N(b) intersect C|>=d_G(b)-2.

**Proof / route.** If every quotient degree in DS15 were at least 3, Q would be a smaller counterexample because quotient power-of-two cycles lift by doubling. Therefore some d_Q(b)<=2; use the degree formula.

**Dependencies.** DS15

**Claim hash.** `0ecd6178fef7328fed3aa3e21cb4c2a8250ee6486bda4b85e6904661d6265cca`

## DS19 — External branch escape
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** For the concentrating vertex b from DS16 and every x in N(b) intersect C, x has a cubic neighbor outside N[b].

**Proof / route.** x has at least two A-neighbors. CY02 says x has at most one neighbor inside N(b), so another A-neighbor lies outside N[b].

**Dependencies.** DS16, CY02

**Claim hash.** `0e4947105d2bc707c545c0aec9e2dc294656b30ec899eb2be7da5ed1fcc3becd`

## DS20 — Distinct external branch escape
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Distinct x,y in N(b) intersect C cannot share an external neighbor; hence their selected escape vertices may be chosen pairwise distinct.

**Proof / route.** A common external neighbor z creates b-x-z-y-b, a 4-cycle.

**Dependencies.** DS19, CY01

**Claim hash.** `8be620024e909c46b244378cd78a0739f9a90bd5590f951937288626e7d8d390`
