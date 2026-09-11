# MSL cumulative late-recovery ledger — assets 239–266

> Exact delta between the later 266-asset cumulative catalog and the previously released 238-row Day-2 master. The first 238 rows are byte-for-field identical in the two CSV catalogs; these 28 rows are the additional mathematical assets. Source authority/status is preserved and not upgraded.

## 239. 25 — Summable congruence avoidance has natural density
**Source:** PASS2_REMINING
**Status:** SOURCE-REPORTED UNIVERSAL THEOREM
**Priority:** HIGH
**Statement:** If one removes one residue class modulo each distinct n_i and sum_i 1/n_i < infinity, then the surviving set has an ordinary natural density; hence it also has logarithmic density.
**Effect:** Absent from 238-row catalog despite being explicitly recovered in the deep audit.
**Next:** Existence of density only; positivity is not implied.

## 240. 218 — Alternating sequence density-independence witness
**Source:** PASS2_REMINING
**Status:** KERNEL_CHECKED
**Priority:** VERY HIGH
**Statement:** For d=(1,2,1,2,...), the <= and >= comparison sets both have asymptotic density 1/2 while the equality set is not infinite.
**Effect:** Entire problem family absent from catalog; theorem and helper density lemmas live in orphan Lean surface.
**Next:** Logical-independence witness; not a close of the canonical problem.

## 241. 74 — Odd-cycle-transversal chromatic reduction
**Source:** PASS2_REMINING
**Status:** PROVISIONAL_SURVIVOR / UNIVERSAL REDUCTION
**Priority:** HIGH
**Statement:** For every finite graph G, chi(G) <= 2 + OCT(G), hence OCT(G) >= chi(G)-2, where OCT is the minimum odd-cycle-transversal size.
**Effect:** Absent problem family; latest-state audit labels the reduction LOW risk and accompanies it with exact small-graph verification.
**Next:** General graph lemma; strength relative to canonical target is separate.

## 242. 873 — Exact k=2 formula for the natural sequence
**Source:** PASS2_REMINING
**Status:** SPECIAL_SEQUENCE_ONLY / EXACT REAL ALGEBRA
**Priority:** HIGH
**Statement:** For A0={1,2,3,...}, F(A0,X,2)=ceil((sqrt(4X+1)-3)/2), and this is < sqrt(X) for every real X>0.
**Effect:** Clean all-X special-sequence theorem absent from catalog.
**Next:** Only A0 and k=2; not the uniform canonical theorem.

## 243. 454 — Universal prime-index upper envelope
**Source:** PASS2_REMINING
**Status:** PROVISIONAL STRUCTURAL SURVIVOR
**Priority:** MEDIUM
**Statement:** For n>=2, f(n) <= p_{n+1}+p_{n-1}, by taking i=1 in the defining minimum.
**Effect:** Problem family absent from catalog; a later route records the all-n theorem after finite verification.
**Next:** Strictly weaker than the target; campaign has unrelated contaminated rows, so preserve route provenance.

## 244. 683 — Stronger exponent ceiling from (10,5)
**Source:** PASS2_REMINING
**Status:** EXACT OBSTRUCTION / OUTWARD-INTERVAL VERIFIED
**Priority:** HIGH
**Statement:** Any universal exponent c must satisfy c <= log_5(7/5); the source records log_5(7/5) in [0.20905,0.20906].
**Effect:** Catalog retained only the weaker (10,3) ceiling c<=log_3(5/3).
**Next:** Necessary ceiling, not existence of an admissible positive c.

## 245. 683 — Sylvester largest-prime-factor baseline
**Source:** PASS2_REMINING
**Status:** CERTIFIED_FRAGMENT / CLASSICAL-LEMMA REDUCTION
**Priority:** MEDIUM-HIGH
**Statement:** With j=min(k,n-k), Sylvester gives a prime p>j dividing C(n,j), yielding P(C(n,k)) >= min(n-k+1,k).
**Effect:** Stronger structural baseline never promoted to the historical catalog.
**Next:** Uses the Sylvester theorem as analytic input; exact verifier checked a large finite range.

## 246. 101 — Four-rich-line exactness under no-five-collinear
**Source:** PASS2_REMINING
**Status:** PROVISIONAL STRUCTURAL SURVIVOR
**Priority:** MEDIUM-HIGH
**Statement:** Under the no-five-collinear hypothesis, every 4-rich line contains exactly four points.
**Effect:** Absent family; small but clean counting lemma.
**Next:** Local structural lemma only.

## 247. 208 — Unbounded squarefree gaps by CRT
**Source:** PASS2_REMINING
**Status:** PROVISIONAL STRUCTURAL SURVIVOR
**Priority:** MEDIUM-HIGH
**Statement:** Squarefree gaps are unbounded: choose distinct primes p_i and solve x ≡ -i (mod p_i^2), forcing a consecutive run of nonsquarefree integers.
**Effect:** The theorem survived in an omitted family but never entered the distinct catalog.
**Next:** Scaffolding relative to the canonical problem.

## 248. 234 — Finite jump-function structure
**Source:** PASS2_REMINING
**Status:** PROVISIONAL STRUCTURAL SURVIVOR
**Priority:** MEDIUM
**Statement:** For each fixed N, F_N is a finite sum of nondecreasing right-continuous one-jump step functions, with jumps at v_n=g(n)/log n; monotonicity and right-continuity are unconditional.
**Effect:** Structured all-N reduction absent from catalog.
**Next:** Jump-set equality needs the stated positivity condition on g(n).

## 249. 1056 — All-k modulo-2 ordered singleton blocks
**Source:** PASS2_REMINING
**Status:** PROVISIONAL SURVIVOR
**Priority:** HIGH
**Statement:** The blocks I_i={2i-1} are nonempty, disjoint, ordered, and their product is odd, hence congruent to 1 mod 2, for every k>=2.
**Effect:** Universal mod-2 construction remained only in the final-green surface.
**Next:** Only the mod-2 and interval-structure clause.

## 250. 701 — Complement-pairing child theorem survives dead route
**Source:** PASS2_REMINING
**Status:** SURVIVING CHILD THEOREM / CONTRADICTION-AWARE
**Priority:** MEDIUM-HIGH
**Statement:** A complement-pairing argument gives |F| <= 2^(n-1) for the relevant intersecting component, with equality attainable by a star.
**Effect:** The problem contains a later false universal star-containment theorem; the clean child theorem was buried with the dead route.
**Next:** Do not promote the false universal star-containment claim.

## 251. 193 — Low-dimensional infinite-range walk obstruction
**Source:** PASS2_REMINING
**Status:** SURVIVING CHILD THEOREM / SCOPE-AUDITED
**Priority:** MEDIUM
**Statement:** An infinite-range S-walk whose used-step span has dimension at most 1 has three collinear points.
**Effect:** The negative route failed because infinite sequence was confused with infinite image; this subspace lemma survives that semantic kill.
**Next:** Dimension-3 residual remains open.

## 252. 1199 — Finite van der Waerden core and affine transfer
**Source:** PASS2_REMINING
**Status:** EXACT FINITE THEOREM
**Priority:** HIGH
**Statement:** Exact exhaustive checking proves W(2,3)=9; an affine map yields a monochromatic configuration {2a,a+b,2b} in every 2-coloring of [1,66].
**Effect:** Finite theorem package was absent from the historic catalog.
**Next:** Finite only; no transference to the infinite canonical target.

## 253. 11 — Finite-certificate to deterministic-witness transfer
**Source:** PASS2_REMINING
**Status:** PROVISIONAL SURVIVOR
**Priority:** HIGH
**Statement:** For one odd n, per-l exact factor certificates p_l^2 | n-2^l through the finite logarithmic range suffice to certify n as a branch-B witness; larger l are out of range.
**Effect:** Logical transfer lemma remained in an omitted family rather than the distinct theorem catalog.
**Next:** Does not establish existence of such a witness.

## 254. 75 — Exact shift-graph independent-set characterization
**Source:** PASS3_DEEP_COMPOSITION
**Status:** SOURCE_PROVED_EXACT_FINITE_REDUCTION
**Priority:** STRUCTURAL
**Statement:** For the finite shift-graph object S_N[W], the independence number equals the maximum over 2-colorings of |W ∩ (R×B)|; every independent family has disjoint first- and second-coordinate sets and is captured by such a coloring.
**Effect:** CL000393, R006/L1 PROVED; exact-integer fail-closed verifier plus proved characterization.
**Next:** Kernelize the characterization once; use it as the base for coloring/probabilistic corollaries.

## 255. 145 — Möbius squarefree-counting identity and exact N(10^7)
**Source:** PASS3_DEEP_COMPOSITION
**Status:** SOURCE_PROVED_IDENTITY_PLUS_FINITE_CERTIFICATE
**Priority:** UNIVERSAL_IDENTITY
**Statement:** For x≥1, the squarefree counting function satisfies N(x)=Σ_{d≤√x} μ(d)⌊x/d²⌋. The archive also exactly certifies N(10^7)=6,079,271 by the Möbius sum and an independent d²-sieve.
**Effect:** CL000550, R006/L1 PROVED. Asymptotic gap-moment claims are outside this promotion.
**Next:** Formalize the universal Möbius identity separately from the large finite count.

## 256. 317 — Signed harmonic granularity via LCM denominator
**Source:** PASS3_DEEP_COMPOSITION
**Status:** SOURCE_PROVED_UNIVERSAL_CORE; KERNEL_FINITE_CORE_ONLY
**Priority:** STRUCTURAL
**Statement:** Let L_n=lcm(1,…,n). Every signed sum Σ_{k=1}^n δ_k/k with δ_k∈{-1,0,1} is an integer multiple of 1/L_n; hence every nonzero such sum has magnitude at least 1/L_n.
**Effect:** CL001197 PROVED. CL005690 kernel-checks the δ-independent divisibility core only for n≤30 and explicitly excludes analytic corollaries.
**Next:** Lean the all-n divisibility theorem; keep analytic consequences separate.

## 257. 535 — Strict divisibility chains avoid equal-pairwise-gcd bad sets
**Source:** PASS3_DEEP_COMPOSITION
**Status:** SOURCE_PROVED_UNIVERSAL
**Priority:** GENERALIZES_EXISTING_CONSTRUCTION
**Statement:** If x1|x2|…|xr is a strict divisibility chain with r≥3, then gcd(x1,xr)=x1 and gcd(x2,xr)=x2 with x1≠x2. Therefore every strict divisibility chain is admissible for the equal-pairwise-gcd avoidance problem.
**Effect:** CL002213, R005/L1 PROVED; finite certificate exhausts r≤8, xi≤64, while the proof is N-independent.
**Next:** Promote this over the powers-of-two-only construction; formalize the two gcd identities.

## 258. 1049 — Lambert divisor-counting identity
**Source:** PASS3_DEEP_COMPOSITION
**Status:** SOURCE_PROVED_UNIVERSAL_IDENTITY
**Priority:** STRUCTURAL
**Statement:** For |x|<1, Σ_{n≥1} x^n/(1-x^n)=Σ_{m≥1} τ(m)x^m by absolute convergence and divisor reindexing. Specializing x=1/t gives Σ_{n≥1}1/(t^n-1)=Σ_{m≥1}τ(m)/t^m for t>1.
**Effect:** CL003507/CL003508 PROVED. This promotion is identity-only; irrationality is not inferred.
**Next:** Formalize the Tonelli/divisor reindexing identity; quarantine coefficient-as-digit arguments.

## 259. 509 — Bernoulli lemniscate explicit two-disc cover
**Source:** PASS3_DEEP_COMPOSITION
**Status:** SOURCE_PROVED_EXPLICIT_COVER
**Priority:** CONCRETE_GEOMETRIC_CERTIFICATE
**Statement:** For L={z:|z²-1|≤1}, the archive certifies L⊆D(-a,a)∪D(a,a) with a=9√2/16, so the two radii sum to 9√2/8<2.
**Effect:** CL002151, R010/L1 PROVED; exact Z[x,y] identities and integer verifier.
**Next:** Package the exact polynomial inequalities independently from the broken R002 complex-interval target.

## 260. 972 — Exact integerization of floor(p√2)
**Source:** PASS3_DEEP_COMPOSITION
**Status:** SOURCE_PROVED_REDUCTION_PLUS_FINITE_CENSUS
**Priority:** EXACT_REDUCTION
**Statement:** For integers p,n, floor(p√2)=n iff n²≤2p²<(n+1)². Using this exact reduction, the archive recomputes all primes p≤100 and obtains the hit set {2,5,29,31,59,73,97} for its campaign predicate.
**Effect:** CL003364, R007/L1 PROVED; integer isqrt and exact postconditions, zero floats.
**Next:** Use the integer inequalities as the canonical verifier interface for larger searches/formalization.

## 261. 513 — Exact coefficient-maximizer for e^z
**Source:** PASS3_DEEP_COMPOSITION
**Status:** SOURCE_PROVED_UNIVERSAL_INSTANCE_STRUCTURE
**Priority:** ANALYTIC_CORE
**Statement:** For r>0, the terms r^n/n! are controlled by the exact ratio r/(n+1): the maximum occurs at n=floor(r), with the adjacent tie at floor(r)-1 precisely when r is an integer, and the tail is strictly decreasing beyond ceil(r).
**Effect:** CL002199, R015/L1 PROVED; exact rational ratio argument.
**Next:** Formalize the unimodality/argmax lemma as reusable entire-function infrastructure.

## 262. 513 — Exact instance value Q(e^z)=0
**Source:** PASS3_DEEP_COMPOSITION
**Status:** SOURCE_PROVED_INSTANCE_THEOREM
**Priority:** EXACT_INSTANCE
**Statement:** For f(z)=e^z, max_n r^n/n! ~ e^r/√(2πr), while max_{|z|=r}|e^z|=e^r; therefore the campaign functional satisfies Q(e^z)=0.
**Effect:** CL002187, R003/L1 PROVED; source uses Stirling with signed control. Formal certificate only checks one finite decay instance, not the asymptotic.
**Next:** Keep as an instance theorem; do not confuse with the supremum-over-functions target.

## 263. 508 — Plane chromatic number isolated to {5,6,7}
**Source:** PASS3_DEEP_COMPOSITION
**Status:** SOURCE_PROVED_KNOWN_BOUND
**Priority:** KNOWN_STRUCTURAL_BOUND
**Statement:** The archive combines a finite 5-chromatic unit-distance obstruction with an explicit 7-color periodic hexagonal tiling to certify 5≤χ(R²)≤7, i.e. χ(R²)∈{5,6,7}.
**Effect:** CL002123, R005/L1 PROVED; exact finite-graph restriction plus rational tiling check.
**Next:** Preserve as exact known infrastructure, not as a new close.

## 264. 386 — Finite k=2 consecutive-prime-product classification
**Source:** PASS3_DEEP_COMPOSITION
**Status:** SOURCE_PROVED_FINITE_CLASSIFICATION
**Priority:** FINITE_EXACT
**Statement:** For every consecutive-prime block product P≤30020, the equation n(n-1)/2=P has solutions exactly n∈{4,15,21}; universal finiteness beyond this range remains unproved.
**Effect:** CL001508, R006/L1 PROVED; exact discriminant/perfect-square scan.
**Next:** Retain finite scope literally; search for a genuine finite-reduction theorem before extrapolation.

## 265. 137 — No three consecutive powerful integers through 10^7
**Source:** PASS3_DEEP_COMPOSITION
**Status:** SOURCE_PROVED_FINITE_CENSUS
**Priority:** FINITE_EXACT
**Statement:** Exact factorization certifies that no n,n+1,n+2 are all powerful for 1≤n≤10^7; the maximum consecutive powerful run in that range is 2, with witnesses 8–9 and 675–676.
**Effect:** CL000530, R007/L1 PROVED; deterministic fail-closed exact factorization.
**Next:** Preserve finite census independently from the false pairwise-coprime reduction used elsewhere in the route.

## 266. 279 — Finite one-class-per-prime uncovered-density bound
**Source:** PASS3_DEEP_COMPOSITION
**Status:** SOURCE_PROVED_FINITE_SYSTEM_THEOREM
**Priority:** STRUCTURAL
**Statement:** For a finite collection of one residue class per prime with Σ 1/p<1, the uncovered set has density at least 1-Σ1/p>0, uniformly in the chosen residues; this does not supply the missing all-primes transference.
**Effect:** CL001106/CL001107, R006/L1 PROVED; explicitly marked weaker than the target.
**Next:** Formalize the finite density lemma and isolate the infinite-prime transference as the sole residual.
