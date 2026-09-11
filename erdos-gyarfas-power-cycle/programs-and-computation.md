# Erdős–Gyárfás power-cycle proof programs and finite targets

> Research-program provenance, **not theorem claims**. The flagship remains open.

## 14 proof programs

### PP01 — Sparse-circuit branch close
**Authority:** SEARCH_PROGRAM  
**Conclusion target:** Dense branch contradicts minimum order.  
**Unsupported steps at freeze:** 3, 4

### PP02 — Slack discharge close
**Authority:** SEARCH_PROGRAM  
**Conclusion target:** Slack branch closes.  
**Unsupported steps at freeze:** 3

### PP03 — Equality quotient close
**Authority:** COURT_PROGRAM  
**Conclusion target:** |A|=2|B| is impossible.  
**Unsupported steps at freeze:** none

### PP04 — Ordinary quotient concentration close
**Authority:** SEARCH_PROGRAM  
**Conclusion target:** Noncubic branch closes through concentration.  
**Unsupported steps at freeze:** 4

### PP05 — Bounded defect-core close
**Authority:** SEARCH_PROGRAM  
**Conclusion target:** Every fixed-surplus noncubic branch closes.  
**Unsupported steps at freeze:** 2, 3

### PP06 — Cubic transition quotient close
**Authority:** SEARCH_PROGRAM  
**Conclusion target:** Cubic branch closes.  
**Unsupported steps at freeze:** 1, 3

### PP07 — Odd-lock destruction close
**Authority:** SEARCH_PROGRAM  
**Conclusion target:** Some perfect matching has no odd lock.  
**Unsupported steps at freeze:** 3, 4

### PP08 — Actual dyadic member close
**Authority:** SEARCH_PROGRAM  
**Conclusion target:** Cubic graph contains a power-of-two cycle.  
**Unsupported steps at freeze:** 1, 2

### PP09 — Odd shortest-cycle steering close
**Authority:** SEARCH_PROGRAM  
**Conclusion target:** Odd shortest switching cycle yields a dyadic switching cycle.  
**Unsupported steps at freeze:** 2

### PP10 — Even residue descent close
**Authority:** SEARCH_PROGRAM  
**Conclusion target:** Even non-dyadic shortest cycle descends to a dyadic one.  
**Unsupported steps at freeze:** 3

### PP11 — Length-displacement exchange close
**Authority:** SEARCH_PROGRAM  
**Conclusion target:** Every shortest switching cycle yields a dyadic member or smaller quotient.  
**Unsupported steps at freeze:** 3, 4

### PP12 — Flat plateau close
**Authority:** SEARCH_PROGRAM  
**Conclusion target:** Flat plateaus cannot support a minimal counterexample.  
**Unsupported steps at freeze:** 1, 2, 3

### PP13 — Finite hostile-system adjudication
**Authority:** SEARCH_PROGRAM  
**Conclusion target:** The exchange-steering bridges are finitely stress-tested and refined.  
**Unsupported steps at freeze:** 1, 2, 3

### PP14 — Full flagship terminal close
**Authority:** SEARCH_PROGRAM  
**Conclusion target:** The Erdős-Gyárfás power-of-two cycle conjecture is proved.  
**Unsupported steps at freeze:** 2, 3

## 24 computational / finite targets

### CT01 — Minimum-order graph search
**Target:** For each n, enumerate graphs with delta>=3 and forbid cycles of lengths 4,8,...<=n; return a witness or an exhaustive certificate.  
**Method:** canonical graph generation + lazy cycle cuts

### CT02 — Cubic-only frontier
**Target:** Enumerate cubic graphs avoiding all dyadic cycle lengths up to order n.  
**Method:** nauty/traces-style canonical generation + cycle census

### CT03 — Universal-root filter
**Target:** Add the requirement that G-v is 2-degenerate for every v.  
**Method:** incremental degeneracy checker

### CT04 — Sparse-circuit dense branch
**Target:** Enumerate (2,3)-sparse circuits of minimum degree 3 avoiding dyadic cycles.  
**Method:** Henneberg/circuit generation

### CT05 — Slack-surplus census
**Target:** Enumerate candidates by exact value |A|-D=6,8,10.  
**Method:** degree-sequence constrained generation

### CT06 — Defect-core generation
**Target:** For t<=T, generate all cores from TG21 and all ordinary quotient attachments.  
**Method:** kernel-first canonical generation

### CT07 — Power-safe Henneberg audit
**Target:** For every generated dense circuit, test all inverse Henneberg-II reductions and exact cycle-lift maps.  
**Method:** symbolic path replacement

### CT08 — Concentrated branch expansion
**Target:** Generate rooted neighborhoods satisfying DS16, DS19, DS20 and forbid connectors 2,6,14,...  
**Method:** rooted canonical backtracking

### CT09 — Cubic edge radius-3 census
**Target:** Classify local extensions around an adjacent cubic pair avoiding C4 and C8.  
**Method:** SAT/backtracking with isomorph rejection

### CT10 — Perfect matching distance matrices
**Target:** For every bridgeless cubic graph, enumerate perfect matchings and row gcds of exchange distances.  
**Method:** matching enumeration + integer gcd

### CT11 — Odd-lock counterexample search
**Target:** Search for a graph with oddpart(g(M))>1 for every perfect matching M.  
**Method:** CT10 filter

### CT12 — Three-matching coprimality test
**Target:** Test TG10 and emit the smallest failing graph/base matching.  
**Method:** distance-matrix row pair gcd

### CT13 — Transition-system direct generation
**Target:** Generate connected loopless 4-regular multigraphs with every 2+2 transition assignment.  
**Method:** canonical multigraph + local partition generation

### CT14 — Shortest switching-cycle census
**Target:** Record the complete spectrum and all shortest switching cycles for CT13 systems.  
**Method:** state graph cycle enumeration

### CT15 — Odd steering falsifier
**Target:** Search for a shortest odd switching cycle violating TG15 under every exterior pairing.  
**Method:** pairing hypercube exhaustive traversal

### CT16 — Residue descent falsifier
**Target:** Search for a shortest even non-dyadic cycle violating TG16.  
**Method:** residue-class route analysis

### CT17 — Length-displacement exchange audit
**Target:** Build the exchange graph, route labels, and local moves; test TG17.  
**Method:** complete finite state traversal

### CT18 — Flat plateau detector
**Target:** Find positive-error connected plateaus and test periodicity predictions.  
**Method:** objective-level component analysis

### CT19 — Periodic quotient extractor
**Target:** Given an exchange-rigid system, identify repeated cells and construct candidate quotients.  
**Method:** automorphism and equitable partition search

### CT20 — Boundary residue leakage census
**Target:** Measure BR09-BR10 sharpness and classify equality systems.  
**Method:** pairing enumeration

### CT21 — Induced path contact compiler
**Target:** Enumerate outside contact signatures on induced paths and list all generated cycle lengths.  
**Method:** finite signature automaton

### CT22 — Bridge completion gadget search
**Target:** Enumerate small cubic caps and test power-safe lift properties for TG01.  
**Method:** gadget synthesis + universal cycle check

### CT23 — Lean-first microtheorem suite
**Target:** Formalize all difficulty-1/2 Court cards and use them as regression anchors.  
**Method:** Lean 4

### CT24 — Novelty-binder batch
**Target:** Run all 102 exact statements and their normalized variants through the local novelty checker.  
**Method:** semantic reviewer + literature binder

## Terminal court boundary

The source packet earns a theorem-forge result, **not** a flagship closure. Search programs exist for cubic and noncubic branches; Court closure still requires the unsupported steps in PP14 or a certified counterexample.
