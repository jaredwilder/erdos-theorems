# Erdős–Gyárfás power-cycle forge — TR cards

> Source packet: 2026-08-04. Status labels are preserved. `UNRUN` novelty means no historical novelty claim. Lean mission names in the source are missions, not kernel receipts.

## TR01 — Perfect-matching contraction transition quotient
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Let G be cubic with a perfect matching M. Contract every edge of M. Each quotient vertex inherits a 2+2 partition of its four incident half-edges according to the two endpoints of the matching edge.

**Proof / route.** Each endpoint of an M-edge has exactly two nonmatching incident edges.

**Claim hash.** `475bc572d1279fbad7365bbe83493457b0fb7a63b95e9443c1d0843b54a57969`

## TR02 — Switching-cycle lift
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Every simple switching r-cycle in the quotient of TR01 lifts to an M-alternating simple cycle of length 2r in G.

**Proof / route.** At each quotient vertex, switching means the cycle uses one half-edge from each endpoint class; lift through the contracted matching edge. Count r quotient edges plus r matching edges.

**Dependencies.** TR01

**Claim hash.** `3fb0d9fe59c995b87938f2c60011c9dcc326bea0ecac552c2220cac5ddafd19e`

## TR03 — Alternating-cycle contraction correspondence
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** M-alternating cycles in G correspond bijectively to simple switching cycles in the quotient, with lengths divided by 2 under contraction.

**Proof / route.** Contraction and lifting are inverse on alternating cycles.

**Dependencies.** TR01, TR02

**Claim hash.** `ec2a57a8976de669f77d248006a4af5a8da82338fb7976c5c7a32302837b134c`

## TR04 — Switching-circuit existence
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** After choosing one cross-pairing at every quotient vertex, the quotient edges decompose into closed switching circuits.

**Proof / route.** The chosen local pairings make every half-edge have a unique successor and predecessor, so the finite state set decomposes into cycles.

**Dependencies.** TR01

**Claim hash.** `f8b8845456c832827607996303b332d6881a6276d6be2614e0e61849caddae61`

## TR05 — Alternating-cycle flip
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** If C is an M-alternating cycle of length 2r, then M triangle E(C) is a perfect matching M_C with |M\M_C|=|M_C\M|=r.

**Proof / route.** Along C, exchange the matching and nonmatching edges. Every cycle vertex remains incident with exactly one selected edge.

**Claim hash.** `10d5ce1b2409a785501653de4a9024fefa8eaae389218544f0983aad68e01bf0`

## TR06 — Perfect-matching symmetric-difference decomposition
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** For any two perfect matchings M,M', the symmetric difference M triangle M' is a disjoint union of even cycles alternating between the two matchings.

**Proof / route.** Every vertex has degree 0 or 2 in the symmetric difference.

**Claim hash.** `93074856eccf969a0c93ffca35b6513777f0cc0c1b36d1ea53f455a022ef36ed`

## TR07 — Exchange-distance sum formula
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** If the components of M triangle M' have lengths 2r_1,...,2r_t, then |M\M'|=r_1+...+r_t.

**Proof / route.** Each alternating component contributes exactly half its edges from M.

**Dependencies.** TR06

**Claim hash.** `958d119bee1a4c7ff4cc65cb6741c559b746ec4c1b26bd35ce4557e4365b554f`

## TR08 — Odd-lock exchange congruence
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Let g(M) be the gcd of the half-lengths of all M-alternating cycles. Then g(M) divides |M\M'| for every perfect matching M'.

**Proof / route.** Use TR06-TR07: every symmetric-difference component is M-alternating and contributes a half-length divisible by g(M).

**Dependencies.** TR06, TR07

**Claim hash.** `a429305b7b15ba9bf843767898d1c1f8de8bbd8abc247614813e073827566448`

## TR09 — Odd-lock exact equivalence
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** For fixed M and integer g>=1, every M-alternating cycle has half-length divisible by g if and only if every perfect matching M' satisfies |M\M'| divisible by g; equivalently |M intersect M'| congruent to |M| modulo g.

**Proof / route.** One direction is TR08. For the converse, flip a single alternating cycle using TR05.

**Dependencies.** TR05, TR08

**Claim hash.** `1a3a4b9f216fcb2c5f1c3904129a8fe7b6d8505ea8895f1b8faf3ae58c4489e8`

## TR10 — Modular constant-weight formulation
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** For an odd prime p, p divides g(M) exactly when the indicator weight 1_M has the same total modulo p on every perfect matching.

**Proof / route.** The weight of M' under 1_M is |M intersect M'|. Apply TR09.

**Dependencies.** TR09

**Claim hash.** `b076ae0eb4ec5ad527dbc00a2e45ff0effd905c6f22b0a9a6e72d972251f7a16`

## TR11 — Odd-lock order divisibility
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** The odd part of g(M) divides |M|=|V(G)|/2.

**Proof / route.** Choose a complete switching-circuit decomposition of the quotient. Every circuit length is divisible by g(M), and their lengths sum to |E(Q)|=2|V(Q)|=2|M|. Any odd divisor of g(M) therefore divides |M|.

**Dependencies.** TR04, TR08

**Claim hash.** `b6351df7e698fed92cde9ac62fb9d127c94fff040997960c6aeee0aae336f70f`

## TR12 — Power-of-two matching-size exclusion
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** If |M| is a power of two, then g(M) has no odd divisor.

**Proof / route.** Immediate from TR11.

**Dependencies.** TR11

**Claim hash.** `3f82ae60578dab6cec90bfcf887485426816a5a1ec711cc61840bc03f4095708`

## TR13 — Node-potential alternating law
**Status:** `CONDITIONAL_DEDUCTION`  
**Authority:** `SEARCH_WITH_PROVED_CONSEQUENCE`  
**Novelty:** `UNRUN`

**Statement.** Assume over an odd prime field that 1_M(uv)=alpha(u)+alpha(v) for every edge. Then alpha alternates sign around every component of the 2-factor G-M.

**Proof / route.** On every nonmatching edge uv, the weight is 0, so alpha(v)=-alpha(u).

**Dependencies.** TR10

**Claim hash.** `5eec4d30793d780035d9ebbb023d57134f87d4dc21d2131b6646653be7ec2a4f`

## TR14 — Odd 2-factor component zero law
**Status:** `CONDITIONAL_DEDUCTION`  
**Authority:** `SEARCH_WITH_PROVED_CONSEQUENCE`  
**Novelty:** `UNRUN`

**Statement.** Under TR13, every vertex on an odd cycle component of G-M has alpha=0; consequently an M-edge cannot join two odd components.

**Proof / route.** After an odd number of sign changes, alpha=-alpha. In odd characteristic this gives alpha=0. Matching edges require endpoint sum 1.

**Dependencies.** TR13

**Claim hash.** `117b25d856d270a4c3da575555550167f95725b66bfd3cc220fa18ed5e5c8e86`
