# Shortest-cycle / ear extension bank — records 1–25

Recovered from `THEOREM-CARDS-EXTENSION.jsonl`. This is a 100-card graph-theoretic extension bank. Court candidates, finite certificates, negative-bank entries, search targets, and conditional statements remain distinct. The Erdős–Gyárfás flagship is not claimed closed.

**Records in this file:** 25

> Registry authority is preserved. `PROPOSED`, `FINITE_CHECKED`, `PROVED_PROSE`, and `SOURCE_ASSERTED_UNCLASSIFIED` are not interchangeable.

## CLAIM-0017 — Two-cycle ear theorem
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

If C is a simple cycle of length r and P is a C-ear of length p whose endpoints divide C into arcs of lengths a and r-a, then P together with the two arcs gives cycles of lengths p+a and p+r-a.

**Fingerprint:** `105425417deba947b0408d0209fe655748555054e1700d08a731479946143184`

## CLAIM-0018 — Shortest-cycle ear barrier
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

If C is a shortest cycle of length r and P is a C-ear of length p with endpoint arc lengths a and r-a, then p>=max(a,r-a)>=ceil(r/2).

**Fingerprint:** `c804ab8e6c94ac4c454f198309cb713924b92c3a2de45d63458cae36b88b4b9b`

## CLAIM-0019 — Shortest ear is induced
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

A shortest C-ear contains no chord between nonconsecutive vertices of the ear path.

**Fingerprint:** `beeba8125f37360e1272acb122284ec182f15fd9d554276ebd149a0cbcf13602`

## CLAIM-0020 — Long shortest-ear interior avoids C
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

Let P=x0...xp be a shortest C-ear with p>=3. No internal vertex of P has a neighbor in C outside the two ear endpoints.

**Fingerprint:** `826b3e03e2191c5f5d31672f92ba923bdb3a428cca735b6ec1a042e330f7a303`

## CLAIM-0021 — Forced escape from a long clean ear
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

In a graph of minimum degree at least 3, every internal vertex of a p>=3 shortest C-ear has a neighbor outside C union P.

**Fingerprint:** `ab363a7003ed2e02f111cc5153b6d2a455f5867c460678b3eebe373be80f944f`

## CLAIM-0022 — Common-neighbor spacing on an ear
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

If C is a shortest cycle of length r and an outside vertex z is adjacent to ear vertices xi,xj with i<j, then j-i>=r-2.

**Fingerprint:** `3781de8ca92ad56a3d60fe1631646bc817ed13d05fc505ff1b6047de3bf88f40`

## CLAIM-0023 — Ear contact multiplicity bound
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

An outside vertex has at most 1+floor((p-2)/(r-2)) neighbors among the internal vertices of a length-p ear around a shortest r-cycle.

**Fingerprint:** `4580354973d84cd8ccfb91edc89e660320499f60ded322f38c8a23e323c13369`

## CLAIM-0024 — Ear-replacement connector barrier
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

Let Q be an exterior xi-xj connector of length h through one component, with d=j-i. If P is a shortest C-ear, then h>=d.

**Fingerprint:** `e3bafd4f7ddb7e562c94116673563beef6655019635fa83d7692aabd1da906f1`

## CLAIM-0025 — Local-cycle connector barrier
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

Under the same setup, if C is a shortest cycle of length r then h>=r-d.

**Fingerprint:** `e82287c6a1f8ac7ea5162ed515d09a8693772dbb4e8006d1e0597ef4d0ced396`

## CLAIM-0026 — Double-barrier connector theorem
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

Every exterior xi-xj connector around a shortest cycle and shortest ear satisfies h>=max(d,r-d)>=ceil(r/2).

**Fingerprint:** `167d02651e80915c2f421fe4d7e41e3ba1e3aa3ea40a0ca1a6e8ad54a55a3b7d`

## CLAIM-0027 — Three-cycle connector packet
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

If the base cycle arcs have lengths a,b with a+b=r, then an exterior xi-xj connector Q of length h generates cycles of lengths h+d, h+p-d+a, and h+p-d+b.

**Fingerprint:** `7e10aa3392036e96e5000a740af02d7d860920e0bfce7a084eb94153c42501a4`

## CLAIM-0028 — Ear-tight exchange theorem
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

If an exterior connector has h=d, replacing the xi-xj segment of a shortest ear by the connector yields another shortest ear of the same length.

**Fingerprint:** `37bb7ac625f5b7420e80ce74847b154ba5665ebba86f9ca77ccd1d97232a0eb6`

## CLAIM-0029 — Cycle-tight exchange theorem
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

If an exterior connector has h=r-d, its union with the xi-xj ear segment is another shortest cycle of length r.

**Fingerprint:** `b36a51f65e92c795d9549934b08a108b74ec447532d450c9f642e64ceb3e1286`

## CLAIM-0030 — P-to-C return double barrier
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

If a path Q of length h joins internal ear vertex xi to a base-cycle vertex and is otherwise disjoint from C union P, then h>=max(i,p-i).

**Fingerprint:** `dc3fc662c9a20ed9a399050902610c4e1d3710bc4e1b4f9e9e10e99bba9c4f89`

## CLAIM-0031 — Four-cycle return packet
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

A P-to-C return from xi to v creates four cycles, using either ear endpoint and either corresponding arc of C; their lengths are h+i+c, h+i+r-c, h+p-i+e, and h+p-i+r-e.

**Fingerprint:** `7689c430e67ecee27a03070cbf873b7d5c549f85bb394d06306022abaa0ea4dd`

## CLAIM-0032 — Exterior C-ear barrier
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

If Q is an exterior path of length h joining two base-cycle vertices whose arc lengths are c and r-c, and P is a shortest C-ear of length p, then h>=max(p,c,r-c).

**Fingerprint:** `2d9b56fad4f25b45ce2c3288deca0d1792185ac572355bbe86f1c4bec7f499f0`

## CLAIM-0033 — Low-degree attachment theorem
**Status:** `CONDITIONAL` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

Assume every proper subgraph of a minimum counterexample is 2-degenerate. For every component H outside K=C union P, the induced graph on H plus its attachment set has an attachment vertex of degree at most 2 in that induced graph.

**Fingerprint:** `ba63b9d636140f9a98a9cffa76311710154b5f52e00df521e043a7baf0253fa1`

## CLAIM-0034 — Singleton attachment multiplicity bound
**Status:** `CONDITIONAL` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

Under OE17, if an exterior component attaches to K at only one vertex s, then s has at most two neighbors in that component.

**Fingerprint:** `6666d58929eddacd0ebcb0bb51e447fec65cf06698be2e49dfa0d7ed1e50bd5e`

## CLAIM-0035 — Root-neighbor cubic theorem
**Status:** `CONDITIONAL` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

If a singleton component attaches through a single edge sy, every other component vertex has graph degree at least 3, and the component is 2-degenerate, then d_H(y)=2 and d_G(y)=3.

**Fingerprint:** `d4f4f8b976129606d8b6318946d6eb770500814a894457d4470aa8bdb0c6475b`

## CLAIM-0036 — Rooted degeneracy-wave ordering
**Status:** `CONDITIONAL` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

Under OE19, the singleton component has a 2-degeneracy elimination ordering beginning with y; every later vertex that first becomes removable has lost a neighbor earlier in the ordering.

**Fingerprint:** `df3ad1c6dc2304ca01ed15c1be17808934551e2b56e8ce45e8c7d7aac11c7409`

## CLAIM-0037 — Single-ear dyadic forcing is false
**Status:** `NEGATIVE_BANK` · **Authority:** `SOURCE_ASSERTED_UNCLASSIFIED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

A shortest cycle together with one ear need not generate a power-of-two cycle.

**Fingerprint:** `940892cd69dd3e84e0bdd665716d4f16e7c52c35219bb693e5936903506878a0`

## CLAIM-0038 — Bare expansion is not a finite contradiction
**Status:** `NEGATIVE_BANK` · **Authority:** `SOURCE_ASSERTED_UNCLASSIFIED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

Exponential local branching around a shortest cycle does not by itself contradict finiteness of a hypothetical counterexample.

**Fingerprint:** `a364fa16f1e2a72cb47517294183b3f3fb635f09214b6bb508afacb486ecb645`

## CLAIM-0039 — One connector packet is insufficient
**Status:** `NEGATIVE_BANK` · **Authority:** `SOURCE_ASSERTED_UNCLASSIFIED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

The double barriers and the three-cycle packet for a single connector do not force a dyadic cycle.

**Fingerprint:** `108015c7ffb42f4fd9a42385b31fd4291f284d87e29088d047783d6f505addd3`

## CLAIM-0040 — Power-of-two difference forcing is false
**Status:** `NEGATIVE_BANK` · **Authority:** `SOURCE_ASSERTED_UNCLASSIFIED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

Arbitrarily large integer attachment sets may avoid all power-of-two pairwise differences.

**Fingerprint:** `d62e35c6ecaeee51c23f61829b5f80b98a355ec8636189a66392f6f22a02ec31`

## CLAIM-0041 — Complete ordinary-ear closure theorem
**Status:** `SEARCH_TARGET` · **Authority:** `PROPOSED` · **Verification:** `INHERITED_FROM_V1_AUDIT`

Every finite minimum-degree-at-least-3 completion of the complete ear system around a shortest non-dyadic cycle creates a power-of-two cycle.

**Fingerprint:** `ff9c7db9bdd04b7e44ec3dbb8f403c31460166840a2df741a0e3d5ec5ed66833`
