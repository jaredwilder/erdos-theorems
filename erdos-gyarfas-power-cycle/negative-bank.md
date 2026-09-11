# Erdős–Gyárfás power-cycle forge — NG cards

> Source packet: 2026-08-04. Status labels are preserved. `UNRUN` novelty means no historical novelty claim. Lean mission names in the source are missions, not kernel receipts.

## NG01 — Attachment-hypergraph non-universality
**Status:** `REFUTED_ROUTE`  
**Authority:** `NEGATIVE_BANK`  
**Novelty:** `UNRUN`

**Statement.** The high-degree attachment hypergraph cannot be a universal primary representation of a minimum counterexample.

**Proof / route.** A minimum counterexample may be cubic, in which case the high-degree set and attachment hypergraph are empty while the entire flagship difficulty remains.

**Claim hash.** `66ceacc89b1c6ad1d69a92f872f0599c7bcf2ec5e8f226a0b570198fb8141470`

## NG02 — Width-two three-terminal forcing is false
**Status:** `REFUTED_ROUTE`  
**Authority:** `NEGATIVE_BANK`  
**Novelty:** `UNRUN`

**Statement.** Two-degeneracy plus three degree-2 terminals does not force a connector of length 2^k-2.

**Proof / route.** Use the 11-cycle with terminals at cyclic positions 0,3,7. Pairwise path lengths are {3,8}, {4,7}, {4,7}, avoiding 2 and 6 (and all larger forbidden lengths by order).

**Claim hash.** `289fde2794a6d8a7b07d3c99087b13adf3219b819ba3353b56d18d086207c43a`

## NG03 — Two-forest word doubling is false
**Status:** `REFUTED_ROUTE`  
**Authority:** `NEGATIVE_BANK`  
**Novelty:** `UNRUN`

**Statement.** Being the union of two forests does not by itself force a dyadic cycle or binary doubling law.

**Proof / route.** The triangle C3 is the union of two forests and has only cycle length 3. Mixed-color cyclic words can have arbitrary non-dyadic lengths.

**Claim hash.** `0ae488eedfff8b0c90a1d2b0a3f3c3c7a194512ea7a495c7faf378ef963553f3`

## NG04 — Sparse rigidity alone is insufficient
**Status:** `REFUTED_ROUTE`  
**Authority:** `NEGATIVE_BANK`  
**Novelty:** `UNRUN`

**Statement.** The density inequalities m<=2n-2 and e(S)<=2|S|-3 alone do not determine dyadic cycle lengths.

**Proof / route.** Small sparse graphs such as C3 satisfy the inequalities but have no dyadic cycle. Minimum degree, criticality, and lifting structure are indispensable.

**Claim hash.** `b4f5ed29a2f9ec65b7b1cd99740a6519fcb4472d7fb02105a8695ea3bee88614`

## NG05 — Edge-spectrum primacy sterility
**Status:** `REFUTED_ROUTE`  
**Authority:** `NEGATIVE_BANK`  
**Novelty:** `UNRUN`

**Statement.** The edge return-spectrum reformulation is not a compression without a theorem selecting an edge with sufficiently rich return paths.

**Proof / route.** It is an exact restatement of cycles through an edge and provides no global coupling by itself.

**Claim hash.** `14adce9ed551e74366dfe21cd4afc66cf02b653c2c179c2a18f3c0482c87a104`

## NG06 — Integer splicing cannot break an odd lock
**Status:** `PROVED_NEGATIVE_THEOREM`  
**Authority:** `NEGATIVE_BANK`  
**Novelty:** `UNRUN`

**Statement.** If every available switching-circuit length is divisible by an odd integer p, then any length obtained solely by integer sums and differences remains divisible by p; such arithmetic splicing cannot produce a power of two.

**Proof / route.** Divisibility by p is preserved under integer linear combinations.

**Claim hash.** `4c98df963b9440d8cb80bced70fec3fc29a17cedd21bc14d7e3b93538645fccd`

## NG07 — Power-of-two gcd does not imply a dyadic member
**Status:** `PROVED_NEGATIVE_THEOREM`  
**Authority:** `NEGATIVE_BANK`  
**Novelty:** `UNRUN`

**Statement.** A set of positive integers may have gcd a power of two while containing no power of two.

**Proof / route.** The set {6,10} has gcd 2 and no power-of-two member.

**Claim hash.** `cfbaaf55d3b12669d4479ae40ef4f6a18b0d511ee2e89e018034bb6ab79b98e4`

## NG08 — Transition-cocycle equivalence withdrawn
**Status:** `WITHDRAWN_UNSUPPORTED`  
**Authority:** `NEGATIVE_BANK`  
**Novelty:** `UNRUN`

**Statement.** The proposed equivalence between odd lock and a nontrivial transition cocycle is not established and must not be used as a Court edge.

**Proof / route.** No canonical potential or cohomology class was constructed whose existence is equivalent to the matching-overlap congruence.

**Claim hash.** `4c70e300d6521e7fd2946ab8ac2033826491fc1b0056b95712b2818abaa0d69c`

## NG09 — Two-arc ear compatibility is impossible
**Status:** `PROVED_NEGATIVE_THEOREM`  
**Authority:** `NEGATIVE_BANK`  
**Novelty:** `UNRUN`

**Statement.** For an external switching ear attached to a switching cycle in a 2+2 transition system, at most one of the two boundary arcs is compatible with the ear.

**Proof / route.** At each endpoint, the entering exterior port can switch onto exactly one incident cycle edge. The two arcs require opposite endpoint choices.

**Dependencies.** BR02

**Claim hash.** `5f45c40cc07c4e4784976cf08e8555acbe1f728e408dd4ff70869fba2a064c96`

## NG10 — Local minimum does not imply path independence
**Status:** `REFUTED_ROUTE`  
**Authority:** `NEGATIVE_BANK`  
**Novelty:** `UNRUN`

**Statement.** A local minimum in the exterior pairing-exchange graph does not imply commuting squares, zero discrete curvature, or path-independent objective changes.

**Proof / route.** General discrete optimization admits strict local minima and nonintegrable local increments.

**Claim hash.** `30bba8a6b789b2dc380e621a229e4d46b491bc3d1b9e995425954b9852a1d196`

## NG11 — Canonical-ear continuity withdrawn
**Status:** `WITHDRAWN_UNSUPPORTED`  
**Authority:** `NEGATIVE_BANK`  
**Novelty:** `UNRUN`

**Statement.** Shortest external returns from neighboring boundary ports need not vary continuously in endpoint or total cycle length.

**Proof / route.** Outside transition choices can branch, and tie-breaking can cause discontinuous changes in the selected return endpoint and compatible arc.

**Claim hash.** `a5c346afbf841a1b0ea1fce3062fb16929e2b182744c9ce003c446ab8c67676e`
