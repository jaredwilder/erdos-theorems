# Erdős–Gyárfás power-cycle forge — BR cards

> Source packet: 2026-08-04. Status labels are preserved. `UNRUN` novelty means no historical novelty claim. Lean mission names in the source are missions, not kernel receipts.

## BR01 — Complementary-channel lemma
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** At every vertex of a switching cycle C, the two edges not used by C form the complementary permissible switching transition.

**Proof / route.** C uses one half-edge from each transition class; one remains in each class.

**Dependencies.** TR01

**Claim hash.** `9dde92e3bd8d2a7d0f9dda9c0ac5a465d8f7c6dbb9104333c46b1794bf657be6`

## BR02 — Opposite-port compatibility
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Orient C and label its unused ports + and - according to which incident cycle edge they can switch onto. An external switching route combines with an arc of C exactly when its endpoint signs are opposite.

**Proof / route.** Check the required incident edge at the route departure and arrival endpoints for each oriented arc.

**Dependencies.** BR01

**Claim hash.** `f7f07aff36bbf2a4740510d9f1457d6d86962af0474cae38fbfb2613f18d32de`

## BR03 — Odd-cycle compatible-return theorem
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** For an odd switching cycle C, every complete deterministic pairing of the exterior transitions contains an opposite-sign boundary route and hence a compatible return trail.

**Proof / route.** There are r positive and r negative ports. If every paired route joined equal signs, each sign class would be partitioned into pairs, impossible for odd r.

**Dependencies.** BR02

**Claim hash.** `971ba25497ea06dbe739f655fc4fe5b93520e2aa9614bec92aeddb39cf38eba7`

## BR04 — Return-trail shortestness bound
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Let C be a shortest switching cycle of length r. If a compatible return route P plus its compatible arc A decomposes into t simple switching cycles, then |P|+|A|>=tr.

**Proof / route.** Every simple switching cycle in the decomposition has length at least r by shortestness; sum their lengths.

**Dependencies.** BR03

**Claim hash.** `301ae4ad6070a82c9b8b1a2377d46a28443f35adb315a5560bf6f79e54a1127f`

## BR05 — Subdouble-return simplicity
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Under BR04, if |P|+|A|<2r, then P union A is a single simple switching cycle.

**Proof / route.** Two or more simple cycles would have total length at least 2r.

**Dependencies.** BR04

**Claim hash.** `7c17457a6c0ec4371f45a2ac1ff1ecf1260b01c91d4a8ed01dca6fe134bb4756`

## BR06 — Route-mass conservation
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Switching the local exterior pairing at one vertex preserves the sum of the lengths of the two affected boundary routes.

**Proof / route.** The switch cuts and re-pairs the same four route segments, using exactly the same exterior edges.

**Claim hash.** `c1995db9f0a0233a0f26ad71c1d569a7f23a83374f3d2bee8dfbf264ae4b08dd`

## BR07 — Endpoint-displacement conservation
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** A local exterior pairing switch preserves the multiset of four boundary endpoints; with a fixed orientation convention, the signed sum of the two affected boundary displacements is conserved modulo |C|.

**Proof / route.** The switch changes partners but not endpoints. Expand the signed endpoint differences before and after.

**Claim hash.** `41ccc059f615b5fd7739ab993f88c69117cea14bda70f9e7ed6006a650fbf19a`

## BR08 — Boundary sign-exchange identity
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** At the pairing level, re-pairing one (+,+) route and one (-,-) route crosswise creates two opposite-sign routes.

**Proof / route.** This is the elementary re-pairing identity {(+1,+2),(-1,-2)} -> {(+1,-1),(+2,-2)}.

**Claim hash.** `30ce044c055b3bdb01028143215fcc27f9633a3a64f41f7d6ced096a707bf8a4`

## BR09 — Residue-class leakage dichotomy
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** Let |C|=2^s u with u odd, and partition boundary positions by residue modulo 2^s. For each residue class, every complete boundary pairing either contains an opposite-sign pair internal to that class, or has at least one positive and at least one negative port paired outside the class.

**Proof / route.** Each residue class contains u positive and u negative ports, both odd. If there is no internal opposite-sign pair, same-sign internal pairs consume even numbers of each sign, leaving an odd positive and an odd negative number to exit.

**Dependencies.** BR02

**Claim hash.** `b95ad1761b2382cf8ca63fa5b5980abba9b76c1d2dc8805a3e61a2f376ba4f53`

## BR10 — Residue leakage lower bound
**Status:** `PROVED_IN_PACKET`  
**Authority:** `COURT_CANDIDATE`  
**Novelty:** `UNRUN`

**Statement.** If no residue class in BR09 contains an internal opposite-sign pair, then at least 2^s boundary routes connect different residue classes.

**Proof / route.** Each of the 2^s classes contributes at least two crossing incidences by BR09. Every crossing route is counted at two endpoint classes.

**Dependencies.** BR09

**Claim hash.** `c901dd64c6e961fffd0a64119d828293ba3a8758577241d739b8a2866d731792`
