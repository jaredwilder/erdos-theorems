# Shortest-cycle / ear extension bank — records 76–100

Recovered from `THEOREM-CARDS-EXTENSION.jsonl`. This is a 100-card graph-theoretic extension bank. Court candidates, finite certificates, negative-bank entries, search targets, and conditional statements remain distinct. The Erdős–Gyárfás flagship is not claimed closed.

**Records in this file:** 25

## CLAIM-0092 — Cycle-template characterization
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

For a fixed base configuration B, a candidate edge set F creates a forbidden cycle C iff F contains every edge of C absent from the base graph.

**Fingerprint:** `a9a20226d518eb609bf9386d68ac854141645b203e726068ac95504de14690e0`

## CLAIM-0093 — Minimal forbidden hyperedge characterization
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

The canonical forbidden hyperedges are exactly the inclusion-minimal nonempty absent-edge sets F(C) of forbidden cycles after individually unsafe singleton candidates are removed.

**Fingerprint:** `ab414d55002be6e9e7994a208df18cc0cf128b877675a5f4385044f4620151d2`

## CLAIM-0094 — Forbidden-hyperedge rank bound
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

If forbidden cycles have length at most L, every minimal forbidden hyperedge has rank at most L; after singleton removal, residual ranks are at least 2.

**Fingerprint:** `10e5a545e0dd33352ea95405c61c4e5bdf59f44d8951182be110a8767730bd31`

## CLAIM-0095 — Explicit minimal three-edge obstruction
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

For the fixed (4,1)⊕(4,7) packet, edges x0-w1, v1-u3, and v3-u1 are pairwise C4/C8-safe but jointly create the C8 x0-w1-x2-v3-u1-u2-u3-v1-x0.

**Fingerprint:** `f1b7d4019bb1b305c32355385060a14874bf4877892c330e0311d5bfccc6ac34`

## CLAIM-0096 — Pairwise conflict graph is incomplete
**Status:** `NEGATIVE_BANK` · **Authority:** `SOURCE_ASSERTED_UNCLASSIFIED`

The pairwise conflict graph on individually safe completion edges is not a complete model of residual compatibility.

**Fingerprint:** `540e50df5c683b484bbfbf1426d895a093a038f90ed732598b0a51eaf8fd9277`

## CLAIM-0097 — Monotone CNF completion equivalence
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

For a fixed hub configuration, residual C4/C8-free degree completion is equivalent to a monotone CNF with one positive coverage clause per uncovered deficit vertex and one negative clause per minimal forbidden hyperedge.

**Fingerprint:** `6092f8507f336abb63d4bc82e2cd7c1b1854f924d9c5b8e9a173b56df6d1697d`

## CLAIM-0098 — Hypergraph independent edge-cover theorem
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

If every feasible N-hub configuration has no candidate-edge set that covers all uncovered deficit vertices while avoiding every forbidden hyperedge, then no C4/C8-free minimum-degree-3 completion with N hubs exists.

**Fingerprint:** `97aaac1682ad3a58e400c71d5096307377e3af7f4610dbcf9a1441b4445cb3e9`

## CLAIM-0099 — Candidate-isolation sufficiency
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

If an uncovered deficit vertex has no incident individually safe candidate edge, the residual completion instance is immediately UNSAT.

**Fingerprint:** `d34eb2309ad70e931e77066f56f5d1110fde44a306f4264ae1fcf48bc25ea6ed`

## CLAIM-0100 — Exact N=0 candidate set
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

The fixed 15-vertex packet has exactly 13 individually C4/C8-safe missing edges.

**Fingerprint:** `703ef9aea1632416ae79f610b04ae981dc54246f1debb8bc79c37ba242e76ca9`

## CLAIM-0101 — Exact N=0 forbidden-hypergraph census
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

The N=0 candidate hypergraph has exactly 56 minimal forbidden hyperedges: 48 of rank 2 and 8 of rank 3, with none of higher rank.

**Fingerprint:** `2a44113dfbc7af282bce282286090e52d1d420d345d3d3c48d527af2c181ad68`

## CLAIM-0102 — Five unit-forced N=0 edges
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

At N=0, deficit vertices v1,v3,w2,u5,u6 each have exactly one incident individually safe candidate edge.

**Fingerprint:** `9367531c7a45eb49b3e352041833d390fd142bff52663835c0d41ab5852aee81`

## CLAIM-0103 — Compact N=0 hypergraph contradiction
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

N=0 completion is impossible because coverage forces edges v3-u1 and v2-w2, while that pair is a rank-2 forbidden hyperedge.

**Fingerprint:** `00815045a2eed311a6242f57a80555876e2a8a99f88fde9fdbb1a7a51c194cfe`

## CLAIM-0104 — N=0 packet UNSAT
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

No simple graph on the 15 packet vertices contains the fixed packet, has minimum degree at least 3, and avoids C4 and C8.

**Fingerprint:** `76547d7209a8c0a2b8bad7a5265b9791da5c087713b6160b271f931b2e083c3f`

## CLAIM-0105 — Complete N=1 hub-configuration census
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

There are exactly 21 complete one-hub base configurations that are C4/C8-free and give the hub degree at least 3.

**Fingerprint:** `91f6da78511b12627d86c072a64211029c632c1d9935758083255e198c3f346c`

## CLAIM-0106 — Complete N=2 hub-configuration census
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

There are exactly 24 complete two-hub base configurations: 16 with nonadjacent hubs and 8 with adjacent hubs.

**Fingerprint:** `c6b480dbcd64186089ac973be347203422de30159180e5b86db5fd26a49bba6b`

## CLAIM-0107 — N=2 adjacency split
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

The 24 complete N=2 configurations split exactly into 16 nonadjacent-hub and 8 adjacent-hub configurations.

**Fingerprint:** `4d944391dc0d74d33dd4d92cf46318972248e332e10ace583389efe417d97f6d`

## CLAIM-0108 — N=1 candidate-isolation theorem
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

Every one of the 21 complete N=1 configurations leaves an uncovered deficit vertex with no incident individually C4/C8-safe candidate edge.

**Fingerprint:** `6e9244eddef1efaeda08979e91e280f86906b863f46814f203e92c2344dbbb98`

## CLAIM-0109 — N=2 candidate-isolation theorem
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

Every one of the 24 complete N=2 configurations leaves an uncovered deficit vertex with no incident individually C4/C8-safe candidate edge.

**Fingerprint:** `fcba28ef2db7b269185c96fe9aaa58bb95099ef8b716a68045169faf1a6efe4b`

## CLAIM-0110 — Bounded packet realization lower bound
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

Any C4/C8-free minimum-degree-3 completion of the fixed packet requires at least three added vertices.

**Fingerprint:** `349bd0e915e074011860cb2afd211b5b41b295440220151dcd678339ff8089fd`

## CLAIM-0111 — Exact deficit conflict-graph edge count
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

The common-hub conflict graph on the 12 deficit vertices has exactly 40 edges.

**Fingerprint:** `f54ce1c4d5b797f8f8e55368a293dff3a86cc3c0613df7980fd4ed3dc38981f4`

## CLAIM-0112 — Exact hub-capacity theorem
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

The deficit conflict graph has independence number 4 and unique maximum independent set {v1,v2,u1,u2}.

**Fingerprint:** `770584b6fb33aee380108b388d2918a65bc2d0ec67e84725d59e3df9631781fb`

## CLAIM-0113 — Exact two-hub coverage theorem
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

Two hub neighborhoods that are independent in the deficit conflict graph and overlap in at most one vertex cover at most seven deficit vertices; the maximizing pair is uniquely {v1,v2,u1,u2} and {w3,u4,u5}, up to order.

**Fingerprint:** `84defa30a2855937ee968db464f2d35950e4c4f9ef1c28d384d0a2e67a0fc8f1`

## CLAIM-0114 — Exact distance-three exclusion count
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

The fixed packet has exactly 26 nonedges whose endpoints have shortest packet distance 3; every such direct edge creates a C4.

**Fingerprint:** `09f75aad968d385be567fa7af840a57156a404cff560d7536f97a48d2d85dea6`

## CLAIM-0115 — Canonical candidate-isolation witness object
**Status:** `FINITE_CERTIFICATE` · **Authority:** `FINITE_CHECKED`

The canonical serialized witness object for all 21 N=1 and 24 N=2 configurations has SHA-256 fe2adefe67664121baaf3b8b4a6cf7cafaa5a62ebcc7c8fb2a69ca41aa2ac179 and every record contains at least one isolated uncovered deficit vertex.

**Fingerprint:** `b435bf62ff216a56578b037262ba0cdf2424a129cc92bdbec30aee4e7d72bdf7`

## CLAIM-0116 — Human candidate-isolation class theorem
**Status:** `SEARCH_TARGET` · **Authority:** `PROPOSED`

The 45 machine-certified N=1/N=2 configurations admit a short exhaustive human classification in which explicit length-3 or length-7 paths block every missing edge incident to one named uncovered vertex.

**Fingerprint:** `b9d56de17fd43361a05554cb5238b2c2c66ceef215416e2784c236828a578e3f`
