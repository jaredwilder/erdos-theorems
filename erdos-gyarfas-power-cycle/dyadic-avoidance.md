# Erdős–Gyárfás power-cycle forge — CY cards

> Source packet: 2026-08-04. Status labels are preserved. `UNRUN` novelty means no historical novelty claim. Lean mission names in the source are missions, not kernel receipts.

## CY01 — Global codegree-one theorem
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** In a graph with no 4-cycle, any two distinct vertices have at most one common neighbor.

**Proof / route.** Two common neighbors x,y of u,v create the 4-cycle u-x-v-y-u.

**Claim hash.** `ebc4f4cb084b5979e41cf9bba10ae364853d85dcfbe23939cbad98a2d6baf533`

## CY02 — Neighborhood matching theorem
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** In a graph with no 4-cycle, the graph induced by every open neighborhood has maximum degree at most 1.

**Proof / route.** If x in N(v) had two neighbors y,z in N(v), then v-y-x-z-v is a 4-cycle.

**Dependencies.** CY01

**Claim hash.** `a8c06af043c15839547d68fe71f45ae3f0cf101fffdd56d9c28b327aafdbe1a6`

## CY03 — Disjoint second-neighbor fans
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** For v and distinct u,w in N(v), the sets N(u)\N[v] and N(w)\N[v] are disjoint in a C4-free graph.

**Proof / route.** A common vertex z outside N[v] would create v-u-z-w-v.

**Dependencies.** CY01

**Claim hash.** `8427a2213db08fd7483ece4e167c4553351a478d209e2805e2d53fd7843f6e78`

## CY04 — Second-neighborhood expansion bound
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** In a C4-free graph of minimum degree at least 3, |N_2(v)| >= sum_{u in N(v)}(d(u)-1-d_{G[N(v)]}(u)) >= 2d(v)-2e(G[N(v)]). Hence |N_2(v)|>=d(v), and if d(v) is odd then |N_2(v)|>=d(v)+1.

**Proof / route.** The outside-neighbor fans are pairwise disjoint by CY03. Sum their exact sizes. Use d(u)>=3 and CY02, where e(G[N(v)])<=floor(d(v)/2).

**Dependencies.** CY02, CY03

**Claim hash.** `ff3185c541a8d00bcab5663c2e9a008f7e0bfd5f067d7fe9506445c23391be3f`

## CY05 — Dyadic connector exclusion at a root
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** If G has no cycle of power-of-two length, then for every vertex v, every two distinct neighbors x,y of v, and every k>=2, G-v contains no simple x-y path of length 2^k-2.

**Proof / route.** Such a path plus vx and vy forms a cycle of length 2^k.

**Claim hash.** `9db26aa2a5ab26a1552794223b50d9b5db157471028c5b092481fe7c5d7c9978`

## CY06 — Edge return-spectrum exclusion
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** If G has no power-of-two cycle, then for every edge uv and every k>=2, G-uv contains no simple u-v path of length 2^k-1.

**Proof / route.** The path plus uv forms a cycle of length 2^k.

**Claim hash.** `9c2e44a59bee8f4b19f9ea0e24a43de83f7ac19d739d12b31d9a57f1eb1fe871`

## CY07 — Closed-neighborhood local triangle bound
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** In a C4-free graph, the triangles containing a fixed vertex v correspond to the matching edges of G[N(v)] and are pairwise edge-disjoint outside v; their number is at most floor(d(v)/2).

**Proof / route.** Use CY02. Each edge xy in N(v) gives triangle vxy, and every triangle through v arises this way.

**Dependencies.** CY02

**Claim hash.** `2f9028cb04785d40c999d8dd0c76c686e30f65ff7f4f1424350bdc01476710d5`

## CY08 — Four-step branch separation
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Let b-x-f(x) and b-y-f(y) be distinct two-edge arms with x,y in N(b). If G has no 8-cycle, then there is no simple length-4 path from f(x) to f(y) internally disjoint from {b,x,y}.

**Proof / route.** Such a path closes with f(y)-y-b-x-f(x) to form an 8-cycle.

**Dependencies.** CY05

**Claim hash.** `f62689241e54bb267d5e5f06e4e80a5e07985bb9333c62e313b5eb2e0a3592b7`
