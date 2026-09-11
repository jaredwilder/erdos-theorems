# Canonical long-tail gold registry — 56 curated mathematical assets

**Author:** Jared Wilder  
**Source court:** September 2026 estate reconstruction.  
**Release rule:** this is the statement/status surface of the canonical 56-asset registry, which supersedes older promotion queues. `KERNEL_CHECKED` means the stated scope was matched to a kernel artifact. `KERNEL_CHECKED_FINITE_ONLY` or single-instance notes do **not** certify the universal statement. `MATHEMATICALLY_AUDITED_LEAN_READY` means the mathematical statement/proof was audited but universal Lean certification is still pending.

This is deliberately a long-tail release: many of these are structural lemmas, exact slices, reductions, negative closes, or known/classical mathematics reconstructed during attacks on larger open problems. Presence here is not a claim that the parent Erdős problem is solved or that the theorem is historically novel.

1. **G001 · #276 · `KERNEL_CHECKED` — Common divisors of Fibonacci/Lucas-type recurrences.** For every `a:ℕ→ℕ` satisfying `a(n+2)=a(n+1)+a(n)`, `d` divides every term iff `d | gcd(a0,a1)`.
2. **G002 · Sidon-8 · `KERNEL_CHECKED` — No 5-element Sidon subset of `Fin 8`.** Every 5-element subset has a nontrivial equal pair-sum; together with a 4-element witness this gives finite optimum `f(8)=4` under the campaign convention.
3. **G003 · #400 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Factorial-divisibility logarithmic bound.** For fixed `k≥2`, `g_k(n) ≤ k(⌊log₂ n⌋+1)`, hence `g_k(n)=O_k(log n)` and `Σ_{n≤x}g_k(n)=O_k(x log x)`; also `g_k(m!)≥m+k−3`.
4. **G004 · #1142 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Multiplicative-order modular sieve.** Let `Good(n)` mean `n−2^j` is prime for every `1<2^j<n`. For odd prime `p`, `r=ord_p(2)`: if `n>p+2^r` and `n mod p∈<2>`, `Good(n)` is impossible. Thus `Good(n), n>21 ⇒ 15|n`; `105` passes the required differences.
5. **G005 · #1052 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Two-prime-factor unitary-perfect classification.** No odd unitary-perfect `n>1` exists; among unitary-perfect numbers with at most two distinct prime factors, the only one is `6`.
6. **G006 · #247 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Sparse binary-position irrationality.** If `a_n` is strictly increasing and `limsup a_n/n=∞`, then `Σ 2^(−a_n)` is irrational.
7. **G007 · #826 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Divisor-bound tail elimination.** For `k>√n`, `τ(n+k)<3k`; therefore any `Ck` bound proved for `k≤√n` extends globally with constant `max(C,3)`.
8. **G008 · #1061 · `MATHEMATICALLY_AUDITED_LEAN_READY` — No diagonal sigma solutions.** `σ(a)+σ(a)=σ(2a)` has no positive solution. Hence all solutions to `σ(a)+σ(b)=σ(a+b)` are off-diagonal, so ordered and unordered counts differ by factor `2`.
9. **G009 · #1073 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Factorial-plus-one divisor shape.** If `u>1` and `u | n!+1`, then every prime `p|u` satisfies `p>n`; if `u` is composite then `u>n²`.
10. **G010 · #936 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Powerful-number square-cube congruence restriction.** Every odd powerful `m=a²b³` with `b` squarefree. For `n≥3`, if `2^n−1` is powerful then `b≡7 (mod 8)`; if `2^n+1` is powerful then `b≡1 (mod 8)`.
11. **G011 · #477 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Square-value tiling slice obstruction.** For `B={k²:k≥0}`, there is no finite `A⊂ℤ` with unique representation `ℤ=A+B`.
12. **G012 · #700 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Exact semiprime binomial gcd formula.** For primes `p≤q` and `n=pq`, `f(n)=p` for `f(n)=min_{1<k≤n/2} gcd(n,C(n,k))`.
13. **G013 · #479 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Infinite k-family for `n | 2^n−k`.** For `j≥0` and every odd prime `p`, `k=2^(2^j)`, `n=2^j p` satisfies `2^n≡k (mod n)`.
14. **G014 · #885 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Factor-difference square criterion.** For `N≥1,d≥0`, `d` is a factor difference `|a−b|` with `ab=N` iff `d²+4N` is a square.
15. **G015 · #456 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Prime-index equality family.** For every prime `p`, at `n=p−1` the two campaign quantities satisfy `m_n=p_n=p`.
16. **G016 · #289 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Unique maximal 2-adic denominator barrier.** Every reciprocal sum over a nontrivial consecutive integer interval is nonintegral. More generally, in an integral sum of interval-block reciprocal sums, the number of blocks attaining the global maximal denominator `v₂` must be even.
17. **G017 · #243 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Eventual divisibility irrationality barrier.** If eventually `a_n|a_(n+1)` and `a_(n+1)/a_n→∞`, then `Σ1/a_n` is irrational.
18. **G018 · #985 · `MATHEMATICALLY_AUDITED_LEAN_READY` — 3 primitive modulo Fermat-prime subfamily.** For every Fermat prime `p≥5`, `3` is a primitive root modulo `p`.
19. **G019 · #274 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Infinite-group reduction for distinct-cardinality exact coset covers.** Any nontrivial finite exact coset cover with pairwise-distinct part cardinalities cannot live in an infinite group; any `>1`-part counterexample must be finite.
20. **G020 · C(13,6,3) · `MATHEMATICALLY_AUDITED_LEAN_READY` — Degree lower bound for a hypothetical 20-block cover.** Every pair occurs in at least `3` blocks, every point has degree at least `8`, and total degree excess above `8` is exactly `16`.
21. **G021 · #1085 · `MATHEMATICALLY_AUDITED` — One-dimensional exact unit-distance extremum.** In dimension `1`, `f_1(n)=n−1` for `n≥1`.
22. **G022 · #376 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Kummer no-carry criterion for `gcd(C(2n,n),105)`.** The gcd is `1` iff doubling `n` has no carries in bases `3,5,7`; equivalently base-3 digits are ≤1, base-5 digits ≤2, and base-7 digits ≤3.
23. **G023 · #681 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Witness geometry and finite search window.** For `k=1`, the witness condition holds iff `n+1` is composite. Every witness `k` satisfies `k^4<n+k`.
24. **G024 · #238 · `MATHEMATICALLY_AUDITED_CITATION_DEPENDENT` — Complete `c2<2` parameter slice.** For every fixed `c1>0` and `0<c2<2`, the requested prime block exists for all sufficiently large `x`.
25. **G025 · #821 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Odd totient targets have no preimages.** For every odd `n>1`, `g(n)=0` where `g(n)=#{m:φ(m)=n}`.
26. **G026 · #936-mod9 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Exact mod-9 periodicity for `2^n+1`.** `9 | 2^n+1` iff `n≡3 (mod 6)`.
27. **G027 · #413 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Exact `O(log n)` finite-window reduction.** For `n>1`, `[∀m<n, m+ω(m)≤n]` iff `ω(n−1)≤1` and `ω(n−k)≤k` for `2≤k≤ceil(log₂(n−1))`; larger `k` are automatic.
28. **G028 · #406 · `MATHEMATICALLY_AUDITED_LEAN_READY` — 3-adic exponent sieve for ternary `{0,1}` powers.** If the ternary digits of `2^n` are all `0/1`, then `n mod 18 ∈ {0,2,6,8}`. More generally modulo `3^r` the allowed exponents form exactly `2^(r−1)` classes modulo `2·3^(r−1)`.
29. **G029 · #683 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Necessary ceiling on the universal exponent c.** Any constant `c` satisfying the canonical binomial largest-prime-factor inequality must obey `c≤log_3(5/3)`.
30. **G030 · #913 · `MATHEMATICALLY_AUDITED_CITATION_DEPENDENT` — Exact `ω=2` stratum classification.** If `ω(n(n+1))=2` and the two nonzero prime exponents are distinct, then `n` is `8`, a Fermat-prime predecessor `2^a` with `2^a+1` prime, or a Mersenne prime `2^b−1`.
31. **G031 · #1212 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Infinite family of admissible dead ends.** For every `k≥2`, `v_k=(2,3^k)` is a graph vertex of degree `1`, and its unique neighbor `(1,3^k)` lies outside the admissible `min>1` subgraph.
32. **G032 · #145 · `MATHEMATICALLY_AUDITED_CITATION_DEPENDENT` — Squarefree-gap moments for `0≤α≤1`.** For every fixed `0≤α≤1`, the normalized squarefree-gap α-moment has a finite limit; at `α=1` the limit is `1`.
33. **G033 · #486 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Finite-A periodicity for the avoidance set.** For finite `A` and `L=lcm(A)`, the positive integers divisible by no `a∈A` are eventually periodic mod `L`; natural and logarithmic densities exist and are equal.
34. **G034 · #539 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Exact value `h(2)=2`.** For the quotient-set extremal function in #539, `h(2)=2`.
35. **G035 · #168 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Two-thirds construction for avoiding `{n,2n,3n}`.** `F(N)≥ceil(2N/3)`.
36. **G036 · #120 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Unbounded-A positive-measure subcase.** If `A` is unbounded, `E=[0,1]` has positive measure and contains no affine copy `aA+b` with `a≠0`.
37. **G037 · #503 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Exact one-dimensional answer.** In `ℝ`, the largest set for which every three points determine an isosceles triangle has size exactly `3`.
38. **G038 · #849 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Exact t=1 and t=2 binomial slices.** `a=3` has exactly one admissible representation `C(n,k)=a`; `a=10` has exactly two.
39. **G039 · #241 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Exact elementary counting bound.** If `|A|=m` and all 3-multiset sums are distinct, then `C(m+2,3)≤3N−2`; in particular `m^3<18N`.
40. **G040 · #930 · `MATHEMATICALLY_AUDITED_LEAN_READY` — r=2 threshold obstruction.** Any `k` valid for `r=2` must satisfy `k≥4`; the disjoint length-3 intervals `{1,2,3}` and `{48,49,50}` have product `705600=840²`.
41. **G041 · #385 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Parity baseline and reduction to even n.** `F(n)≥n` for every `n≥5`, and `F(n)>n` automatically for every odd `n≥5`; the first question therefore reduces to even `n`.
42. **G042 · #341 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Exact seed `A={1}`.** The #341 greedy pair-sum sequence is `1,3,5,7,…` with constant gap `2`.
43. **G043 · #579 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Common-neighborhood `K_{2,2}` reduction.** In a `K_{2,2,2}`-free graph, the common neighborhood of any two vertices is `K_{2,2}`-free.
44. **G044 · #291 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Correct leading-base-p harmonic criterion.** Let `p≤n` be prime, `p^e` the largest power of `p≤n`, and `q=floor(n/p^e)`. For `a_n=Σ_{k≤n} L_n/k`, `p | gcd(a_n,L_n)` iff the reduced numerator of `H_q` is `0 mod p`.
45. **G045 · #377 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Corrected large-prime Kummer interval criterion.** For prime `p≤n` with `p>√(2n)`, `k=floor(n/p)`: `p∤C(2n,n)` iff `p>2n/(2k+1)`.
46. **G046 · #394 · `MATHEMATICALLY_AUDITED_LEAN_READY`; finite kernel only — Exact prime slice.** For every odd prime `p`, `t_2(p)=p−1`. The existing kernel receipt checks only primes below `100`.
47. **G047 · #727 · `MATHEMATICALLY_AUDITED_LEAN_READY`; finite kernel only — Infinite k=2 obstruction family.** For every prime `p≥7`, with `k=2`, `n=2p−2`, `(n+2)!² ∤ (2n)!`. Existing green receipt covers eight concrete primes only.
48. **G048 · #887 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Explicit two-nearby-divisor family.** For `n=m(m−1)(m+1)(m+2)`, `m≥2`, the divisors `m²+m` and `m²+2m` both lie in `(√n, √n+2n^(1/4))`.
49. **G049 · #359 · `MATHEMATICALLY_AUDITED_LEAN_READY`; misleading receipt quarantined — Universal quadratic upper bound for the true greedy sequence.** For the `n=1` greedy consecutive-block-sum sequence, `a_{k+1}≤k(k+1)/2+1`. The old green receipt used a semantically wrong seed and is not authority for this theorem.
50. **G050 · #153 · `MATHEMATICALLY_AUDITED_LEAN_READY`; single-instance kernel only — Universal Sidon sumset bookkeeping and gap inequality.** For finite Sidon `A`, `|A|=n`, `A+A={s_1<…<s_t}`, `t=n(n+1)/2` and `(s_t−s_1)²≤(t−1)Σ_{i<t}(s_{i+1}−s_i)²`.
51. **G051 · #51 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Elementary totient-preimage size bound.** If `φ(n)=a` and `r=ω(n)`, then `r!≤a` and `n/a≤2^r`; hence `n≤a·2^{R(a)}`, where `R(a)=max{r:r!≤a}`.
52. **G052 · #313 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Finiteness for every fixed number k of primes.** For fixed `k`, `Σ_{i=1}^k 1/p_i = 1−1/m` with distinct primes has only finitely many solutions. Any infinite family must have `k` unbounded.
53. **G053 · #371 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Largest-prime-factor ties are impossible.** For every `n≥2`, `P(n)≠P(n+1)`.
54. **G054 · #412 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Sigma orbits strictly increase above 1.** For every `n≥2`, `σ(n)≥n+1>n`; every forward sigma-orbit starting at `n≥2` is strictly increasing and has no repetitions.
55. **G055 · #655 · `MATHEMATICALLY_CLOSED_NEGATIVE_LITERAL`; finite kernel only — Regular polygons refute the literal frozen distance bound.** For every `n≥3`, the regular `n`-gon satisfies the circle condition and determines exactly `floor(n/2)` distinct distances. Therefore no `c>0` can make the frozen lower bound `(1+c)n/2` hold for all sufficiently large `n`. The available receipt checked only a finite instance; the universal negative theorem is mathematical rather than universally kernel-certified.
56. **G056 · #68 · `MATHEMATICALLY_AUDITED_LEAN_READY` — Exact geometric-series reformulation.** For `n≥2`, `1/(n!−1)=Σ_{j≥1}(n!)^(−j)`; every finite truncation has an exact positive geometric remainder.

## Court boundary

This file releases the canonical statement surface without erasing the proof-status distinctions. Several entries are known/classical subcases, some are citation-dependent, and many remain Lean-promotion targets. The parent open problems remain open unless separately and explicitly closed in a dedicated repository.

The full canonical source additionally contains proof/certificate paragraphs, receipt names, formal-scope notes, and corrections. That source is release material too; this statement registry exists so that the mathematical identities are public immediately while the full canonical bytes are moved into the public provenance layer unchanged.
