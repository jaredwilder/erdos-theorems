# Shortest-cycle / ear extension bank — records 26–50

Recovered from `THEOREM-CARDS-EXTENSION.jsonl`. This is a 100-card graph-theoretic extension bank. Court candidates, finite certificates, negative-bank entries, search targets, and conditional statements remain distinct. The Erdős–Gyárfás flagship is not claimed closed.

**Records in this file:** 25

> Registry authority is preserved. `PROPOSED`, `FINITE_CHECKED`, `PROVED_PROSE`, and `SOURCE_ASSERTED_UNCLASSIFIED` are not interchangeable.

## CLAIM-0042 — C4-free cubic-neighborhood matching
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

In a C4-free graph, the subgraph induced by the three neighbors of a cubic vertex has maximum degree at most 1.

**Fingerprint:** `5f933018d94d6d6c2ea2da5965a825d210833d99688b7d8822efd493891a0c96`

## CLAIM-0043 — Valid suppression neighbor exists
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

At every cubic vertex y in a C4-free graph, one neighbor a is nonadjacent to the other two neighbors b,c.

**Fingerprint:** `d45fc459ed9ca6236bf61269eba2fd91ffcfa49bf7ce1eac52e0b3ccb8e8dd75`

## CLAIM-0044 — Y-to-V suppression preserves minimum degree
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

Delete a cubic vertex y with neighbors a,b,c where ab and ac are absent, and add ab,ac. The resulting simple graph has minimum degree at least 3 whenever the original graph does.

**Fingerprint:** `6259c1cda971c5adb2fefdc9d63aa9d6638f25ececddca89ba89d95ac2ca1116`

## CLAIM-0045 — Suppression cycle-lift dictionary
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

For the Y-to-V suppression centered at neighbor a, a cycle using zero artificial edges lifts unchanged, a cycle using both artificial edges lifts with the same length, and a cycle using exactly one artificial edge lifts to a cycle one edge longer.

**Fingerprint:** `61a96726f79e3ed496cffe283d76ff67fd742020f8a92a702203e9567966061e`

## CLAIM-0046 — Single-artificial-edge obstruction
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

In a minimum-order counterexample, every dyadic cycle in a valid suppressed graph uses exactly one artificial edge.

**Fingerprint:** `74aa5f54b19cdba7341b4f6383e2d9b121336b6f84b4b4071cd58f4f76230d21`

## CLAIM-0047 — Near-dyadic cycle at every cubic vertex
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

Every cubic vertex of a minimum-order counterexample lies on a cycle of length 2^k+1 for some k>=2.

**Fingerprint:** `d610ebf83e0ef553260a99f23233280655bfaa3a5098944e85aedfcb5771c2a3`

## CLAIM-0048 — Mersenne path certificate
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

For every cubic vertex y in a minimum-order counterexample, two of its neighbors are joined in G-y by a simple path of length 2^k-1.

**Fingerprint:** `f511f86301257ce8e4cad2214259d0a18a0cffd740e1e658cb2631db44b68e60`

## CLAIM-0049 — Triangle-completion suppression
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

If a cubic vertex has an independent neighborhood {a,b,c}, deleting it and adding the triangle ab,bc,ca gives a smaller simple graph of minimum degree at least 3.

**Fingerprint:** `56c6968c5aca16179bc562ef25828546e0bde94b7c235d57d64e57afafc52b96`

## CLAIM-0050 — Triangle-completion one-edge obstruction
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

In a minimum-order counterexample with independent cubic neighborhood, every dyadic cycle in the triangle-completed graph uses exactly one added triangle edge.

**Fingerprint:** `34dcea665fb26db2542e8533ea5cd72be046e2f3f36a81f89d477a1bd5ce8e47`

## CLAIM-0051 — Local Mersenne coverage theorem
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

For an independent cubic neighborhood {a,b,c}, at least one of the three neighbor pairs has a path of length 2^k-1 in G-y.

**Fingerprint:** `2f9a4958be71fd6c154e2c81ae1a4855e41935ea19f0e2f25d793889c09bce99`

## CLAIM-0052 — Equal-exponent fan kill
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

If two length-(2^k-1) certificates share one terminal and are internally disjoint away from it, then together with the two edges through the cubic center they form a cycle of length 2^(k+1).

**Fingerprint:** `916921a4105198e295d118741ae08eb63b6d4ee91a8fdaf1f4f356d791ed6dab`

## CLAIM-0053 — Bottleneck complementary-cycle theorem
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

Two equal-length Mersenne certificates with first common interior vertex split into two simple cycles of lengths s and 2q-s, where q=2^k.

**Fingerprint:** `7323b591bf3b207f921cf6656d218a3ec8e8d2880cbbf3fd7335048df110118f`

## CLAIM-0054 — Forbidden bottleneck-sum ladder
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

In a counterexample, the bottleneck sum s in CS12 avoids every value 2^j and 2q-2^j.

**Fingerprint:** `71c67b2b910d939014743893238a7429a4bb3861a9d20235536e38209c320b48`

## CLAIM-0055 — Same-scale symmetric-difference ledger
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

For two cycles C1,C2 of length q+1 sharing m edges, the total length of the edge-disjoint cycles in C1 symmetric-difference C2 equals 2(q+1-m).

**Fingerprint:** `b6eca74bc2a9d2f306bc710058746738b339b505186da3ed1d0d21bfb0d6222c`

## CLAIM-0056 — Connected symmetric-difference cycle theorem
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

If the symmetric difference in CS14 is connected, it is one cycle of length 2(q+1-m).

**Fingerprint:** `580ff00af945e4903ae36e8c6e650ec2fffde0bd6c3c850d6e72571ac4706df1`

## CLAIM-0057 — Dyadic overlap-path theorem
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

Two (q+1)-cycles sharing exactly one path of length s and otherwise edge-disjoint produce a cycle of length 2(q+1-s), dyadic whenever s=q+1-2^j.

**Fingerprint:** `0dfa7196771f21b43c2a4fc2446490153cf43a12d1b41fa99ac60d207cb01c7f`

## CLAIM-0058 — One-edge local collision theorem
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

Two equal-exponent suppression cycles at one cubic center that share only their common center edge force a cycle of length 2q.

**Fingerprint:** `4e18a46f1f32bf71b527cf10452be9613538d0ead045bdb037b50072e9c7a56c`

## CLAIM-0059 — Global exponent repetition
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

If one Mersenne certificate exponent is chosen at each of M cubic vertices of an n-vertex graph, some exponent occurs at least M/(floor(log2 n)-1) times.

**Fingerprint:** `87d41fea067db33069970f4a5e5eba23b2ee2095ab9cd61f2fe2a6cabe1322e6`

## CLAIM-0060 — Same-scale edge-overlap threshold
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

In a graph with m edges, more than m/(q+1) distinct cycles of length q+1 force two cycles to share an edge.

**Fingerprint:** `3c2adaa9f058064104c1251a543e61273b200d73ace3f1ae2c02c1c541534719`

## CLAIM-0061 — Exponent repetition alone is insufficient
**Status:** `NEGATIVE_BANK` · **Authority:** `SOURCE_ASSERTED_UNCLASSIFIED`

Repetition of the same near-dyadic exponent at many cubic vertices does not by itself produce a dyadic cycle.

**Fingerprint:** `6adf8d77f58d84b33810caca25680bd2a135b725f8f6d3d53bcf6a063e6ce44b`

## CLAIM-0062 — Suppression-spectrum intersection theorem
**Status:** `SEARCH_TARGET` · **Authority:** `PROPOSED`

Across the valid suppressions of a cubic vertex, either one dyadic cycle lifts exactly or two hostile one-edge sectors share an exponent and combine into a dyadic cycle.

**Fingerprint:** `4597ffba5bd881ec802fa5be0f404175f16c640f37c76861dda30485be837e4c`

## CLAIM-0063 — Cubic suppression branch close
**Status:** `SEARCH_TARGET` · **Authority:** `PROPOSED`

No cubic minimum-order counterexample survives all valid Y-to-V and triangle-completion suppressions.

**Fingerprint:** `5de1ab4bf8117ec45aec54568640bf08804ca2476833a34509306f213d981e06`

## CLAIM-0064 — Ordered lens decomposition
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

Two equal-length paths whose common vertices occur in the same order decompose into a series of lens pairs (ri,si), with total signed imbalance sum_i(ri-si)=0.

**Fingerprint:** `dd4b10b81c6413917d51ad7d0a72fff9fe5a61ccc6f2382915204e894c25cc62`

## CLAIM-0065 — Equal-arm lens elimination
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

In an ordered equal-length certificate pair chosen with a minimum number of lenses, no nonfatal lens has equal arm lengths.

**Fingerprint:** `cf7b3b83d6973cfd77125fadcfb092810a4aaf8e7d548bdd86b417ad09c9066b`

## CLAIM-0066 — Proper zero-sum block exclusion
**Status:** `COURT_CANDIDATE` · **Authority:** `PROPOSED`

In a minimum-lens ordered equal-length pair, no nonempty proper consecutive block of lens imbalances has sum zero.

**Fingerprint:** `1d34b69bcf907f8027f5d2dedd1fc21e827c1bfea6d5d5e1a31d25bb2bc654d2`
