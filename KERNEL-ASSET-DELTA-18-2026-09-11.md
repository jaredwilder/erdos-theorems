# Kernel Asset Delta — 18 recovered formal files

**Author:** Jared Wilder  
**Public provenance release:** 2026-09-11

This is the public disposition ledger for the recovered `07-KERNEL-ASSET-DELTA-18.csv` formal-artifact audit.

Exact recovered CSV:

```text
bytes=17997
sha256=3035dccc06b29fb20a6e75a0cc7977ddb5bd7996ac9421c4f2e80c3cb19111de
```

The CSV is the authority for exact declaration lists, axiom footprints, runner JSON and classification. This Markdown surface summarizes it without upgrading any row.

| formal file | declarations | recorded runner status | class / disposition |
|---|---:|---|---|
| `Cover20Degree.lean` | 2 | VERIFIED, 3.6s | high-actionability; degree/pair profile for hypothetical 20-cover; later ordinary theorem strengthens degree 8 to degree 9 |
| `Erdos1061Sigma.lean` | 2 | VERIFIED, 70.1s | valid sigma lemmas; parent result externally overtaken |
| `Erdos1201Rescue.lean` | 1 | no green receipt in delta | local structure; not promoted |
| `Erdos155Rescue.lean` | 2 | UNVERIFIED | `le_F` clean; target theorem not kernel-clean in this run; recovered rescue source published separately with this boundary |
| `Erdos276Corollary.lean` | 2 | VERIFIED, 3.3s | exact common-divisor / coprime-seed corollary |
| `Erdos289Head.lean` | 7 | axiom receipts present; no runner JSON in delta | exact finite fragments; not the later all-prime theorem |
| `Erdos313Head.lean` | 2 | VERIFIED, 43.9s | exact head pruning; infinitude untouched |
| `Erdos400Witness.lean` | 3 | VERIFIED, 4.5s | exact factorial witness identities |
| `Erdos412Sigma.lean` | 4 | VERIFIED, 3.7s | elementary sigma-orbit structure |
| `Erdos456Equality.lean` | 2 | VERIFIED, 3.4s | known-externally formalization; focused receipt now public |
| `Erdos477NoSquareTiling.lean` | 2 | VERIFIED, 3.7s | known quadratic obstruction; focused receipt now public |
| `Erdos479Family.lean` | 1 | VERIFIED, 3.6s | known-externally formalization |
| `Erdos479LTE.lean` | 2 | VERIFIED, 3.3s | known `k=-1` family formalization |
| `Erdos700Semiprime.lean` | 2 | VERIFIED, 52.4s | semiprime theorem formalization |
| `Erdos885Duality.lean` | 1 | VERIFIED, 4.6s | structural factor-difference/square duality; focused receipt now public |
| `Erdos936Congruence.lean` | 2 | VERIFIED, 4.6s | exact mod-9 local structure; focused receipt now public |
| `Erdos949Core.lean` | 4 | VERIFIED, 76.5s | headline sharp `q<=5` theorem; focused receipt now public |
| `Erdos949Hindman.lean` | 14 | VERIFIED, 71.8s | headline countable analogue; focused receipt now public |

## Green-receipt rule

`VERIFIED` here means the historical runner exited 0 and its declaration audit reported clean declarations with the listed ordinary Mathlib axiom footprint. It does **not** mean novelty, parent-problem closure, or that a missing source file has been reconstructed byte-for-byte.

Conversely, the #155 rescue remains explicitly `UNVERIFIED` at the recovered kernel-delta run. Its mathematical deletion proof is valid, but the formal source does not receive a green badge until a clean rerun exists.

## Source-byte debt

Several exact `.lean` source files survive only inside larger historical archives / extracted declaration ledgers rather than as standalone Library objects. Their theorem identities and green runner receipts are now public; exact byte mirroring remains a separate release-recovery task.
