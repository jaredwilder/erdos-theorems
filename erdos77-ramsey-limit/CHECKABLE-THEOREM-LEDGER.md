# Erdős #77 — diagonal Ramsey exponential-limit campaign

This file releases the **23 theorem / negative-theorem assets** recovered from `CHECKABLE_THEOREM_LEDGER.md`. The campaign studies the existence/value of the exponential growth rate of diagonal Ramsey numbers and possible near-multiplicative witness constructions.

`PROVED-IN-SESSION` means the supplied argument establishes the stated mathematical lemma. `CHECKABLE-CONDITIONAL` means the implication is proved but its hypothesis is not. Diagnostic negative theorems delimit specific proof architectures; they are not universal impossibility theorems.

Throughout, `r(s,t)` is the two-colour Ramsey number and `R(k)=r(k,k)`.

## P01 — Thin-Corridor Ramsey Inequality
**Status:** `PROVED-IN-SESSION`

For integers `n>a>=0`,

\[
r(n-a,n)\le R(n)\le4^a r(n-a,n).
\]

The upper bound follows by expanding the standard Ramsey recursion from `(n,n)` and stopping each branch when one coordinate reaches `n-a`.

## P02 — Thin-Corridor Equivalence
**Status:** `PROVED-IN-SESSION`

If `a_n=o(n)`, then

\[
\frac1n\log R(n)-\frac1n\log r(n-a_n,n)\to0.
\]

Consequently the two sequences have identical exponential limsup and liminf. Convergence along any one sublinear off-diagonal corridor is equivalent to convergence on the diagonal.

## P03 — Inverse Homogeneous-Set Formulation
**Status:** `PROVED-IN-SESSION`

Define

\[
h(N)=\min_{|V(G)|=N}\max\{\omega(G),\alpha(G)\}.
\]

Then

\[
R(k)>N\iff h(N)<k.
\]

For `L>1`,

\[
R(k)^{1/k}\to L
\iff
\frac{h(N)}{\log N}\to\frac1{\log L}.
\]

## P04 — Clone Saturation Lemma
**Status:** `PROVED-IN-SESSION`

Let `G` be a red/blue colouring of `K_{R(k)-1}` with no monochromatic `K_k`. Every vertex lies in a red `K_{k-1}` and a blue `K_{k-1}`. Equivalently, each red neighborhood contains a red `K_{k-2}` and each blue neighborhood contains a blue `K_{k-2}`.

## P05 — Weighted Wrong-Pair Inequality
**Status:** `PROVED-IN-SESSION`

Let `G` have clique number at most `a`; assign nonnegative loads `s_i<=b`, put `t=sum s_i`, and let

\[
B=\sum_{ij\notin E(G),\ i<j}s_is_j.
\]

Then

\[
B\ge\frac{t(t-ab)}{2a}.
\]

This is a weighted Motzkin–Straus consequence and quantifies the threshold at which independent noisy blow-up must pay a wrong-colour penalty.

## P06 — Summable Composition Error Accumulation
**Status:** `PROVED-IN-SESSION`

Suppose a witness product multiplies vertex counts and its parameter obeys

\[
m(X\star Y)\le m(X)+m(Y)+C\frac{m(X)+m(Y)}{\log^2(m(X)+m(Y))}
\]

for sufficiently large inputs. Starting from `q` identical parameter-`K` witnesses, one can parenthesize the product so that

\[
M_q\le qK\exp(O(1/\log K))
=qK(1+O(1/\log K)),
\]

uniformly in `q>=1`. Balanced dyadic construction plus binary expansion supplies arbitrary `q`, not merely powers of two.

## P07 — Approximate Supermultiplicativity Implies Existence
**Status:** `CHECKABLE-CONDITIONAL`

Put `A(k)=R(k)-1`. Assume constants `C,k_0` such that for all large `m,n` there is

\[
0\le E(m,n)\le C\frac{m+n}{\log^2(m+n)}
\]

with

\[
A(m+n+E(m,n))\ge A(m)A(n).
\]

Then

\[
\lim_{k\to\infty}R(k)^{1/k}
\]

exists. The implication is proved; the approximate-supermultiplicativity hypothesis is not.

## P08 — Complementary Off-Diagonal Amplification
**Status:** `CHECKABLE-CONDITIONAL`

Assume a composition theorem combines a witness for `r(s,Cs)` and its colour-swapped copy with multiplicative vertex count and `o(s)` loss in both final forbidden parameters. If

\[
r(s,Cs)\ge B(C)^{s+o(s)},
\]

then

\[
\liminf_{k\to\infty}R(k)^{1/k}
\ge B(C)^{2/(1+C)}.
\]

## P09 — Bradač-input optimization constant
**Status:** algebra proved in-session; Ramsey consequence conditional on P08

Using the external fixed-ratio lower-bound exponent

\[
r(s,Cs)\ge2^{(1-1/(2C))s},
\]

P08 would give

\[
f(C)=\frac{2-1/C}{1+C}.
\]

The unique maximizer is

\[
C_*=\frac{1+\sqrt3}{2},
\qquad
f(C_*)=4-2\sqrt3,
\]

and the corresponding conditional diagonal base is

\[
2^{4-2\sqrt3}\approx1.4498447105>\sqrt2.
\]

## P10 — Explicit binary nonedge-polarity digraph
**Status:** `PROVED-IN-SESSION`

For `p>=1`, define

\[
V(D_p)=\{(a,b)\in(\mathbb F_2^p\setminus\{0\})^2:a\cdot b=1\},
\]

with arc

\[
(a,b)\to(a',b')\iff a\cdot b'=0.
\]

Then `D_p` is loopless and `T_{p+1}`-free, with exact size

\[
|D_p|=(2^p-1)2^{p-1}.
\]

Hence

\[
\frac{|D_{p_1+p_2+1}|}{|D_{p_1}||D_{p_2}|}\to8.
\]

The source audit notes a finite-count discrepancy with a displayed formula in the external source defining the related ordered-nonedge construction; this campaign relies on its direct count, not that external finite formula.

## P11 — Tagged direct-sum / XOR identity
**Status:** `PROVED-IN-SESSION`

For factor vertices `(a_1,b_1)` and `(a_2,b_2)`, set

\[
A=(a_1,a_2,1),\qquad B=(b_1,b_2,1).
\]

Then `A·B=1`; if `e_i(x,y)` are factor arc bits, the product arc bit is

\[
e(x,y)=e_1(x,y)\oplus e_2(x,y).
\]

## P12 — Exact pattern-collision identity for XOR product
**Status:** `PROVED-IN-SESSION`

For an ordered `t`-tuple `X`, let `F_X` be its upper-triangular arc pattern and `c_D(F)` the number of ordered tuples with pattern `F`. Then

\[
I_t(D_1\otimes D_2)=\sum_F c_{D_1}(F)c_{D_2}(F).
\]

Cauchy–Schwarz yields the corresponding `L^2` pattern-count upper bound.

## P13 — Pattern collision implies triangular orthogonality
**Status:** `PROVED-IN-SESSION`

If two factor tuples have the same arc pattern, then for `i<j`, after doubling coordinates

\[
A_i=(a_i,a_i'),\qquad B_j=(b_j,b_j'),
\]

one obtains

\[
A_i\cdot B_j=0.
\]

Thus pattern collision becomes a triangular bilinear-system count.

## P14 — Exact tensor-flag rank formula
**Status:** `PROVED-IN-SESSION — TERMINAL ALGEBRA ASSET`

Let

\[
L_1\subseteq\cdots\subseteq L_t\subseteq U
\]

be a nested flag, let `b_1,...,b_t in W`, choose a basis `e_1,...,e_d` adapted to the flag, and let

\[
\tau_r=\min\{j:e_r\in L_j\}.
\]

Then

\[
\dim\left(\sum_{j=1}^tL_j\otimes\langle b_j\rangle\right)
=
\sum_{r=1}^d
\dim\operatorname{span}\{b_j:j\ge\tau_r\}.
\]

## P15 — Mixed bilinear product theorem
**Status:** `PROVED-IN-SESSION algebraically`

For factor vertices satisfying `a_i·b_i=1`, put `u=(a_1,a_2)`, `v=(b_1,b_2)` and choose

\[
Q=\begin{pmatrix}I&M\\N&I\end{pmatrix}.
\]

After adjoining one tag coordinate, the campaign constructs a bilinear form for which every product vertex remains valid and whose cross matrices `M,N` alter the product arc relation linearly. This is an exact algebraic mixer theorem.

**Important limitation:** P21 below shows that on the full Cartesian polarity product this construction has huge exact independent coordinate fibers. P15 is not by itself a viable SCC operator.

## P16 — One-sided mixer affine equations
**Status:** `PROVED-IN-SESSION`

With `N=0`, forward-independence of an ordered product tuple requires, for every `i<j`,

\[
(a_{1i}+a_{1j})^T M b_{2j}
=
a_{1i}\cdot b_{1j}+a_{2i}\cdot b_{2j}.
\]

The coefficient tensor is

\[
(a_{1i}+a_{1j})\otimes b_{2j}.
\]

## P17 — Exact mixer rank via affine prefix flags
**Status:** `PROVED-IN-SESSION`

Let

\[
L_j=\operatorname{span}\{a_{1i}+a_{1j}:i<j\}.
\]

These form a nested flag. Applying P14 gives the exact mixer-equation rank

\[
R_M(X)=
\sum_{r=1}^{d_A}
\operatorname{rank}\{b_{2j}:j\ge\tau_r\}.
\]

In particular, if `d_j=dim L_j` and `rho_j=rank{b_{2ell}:ell>=j}`, then

\[
R_M(X)\ge d_j\rho_j.
\]

## P18 — Rank-weighted mixer first moment
**Status:** `PROVED-IN-SESSION`

For independent uniform mixer bits, a candidate tuple with a consistent affine system of rank `R(X)` survives with probability

\[
2^{-R(X)}.
\]

Thus

\[
\mathbb E_M I_t(M)\le\sum_X2^{-R(X)}.
\]

With a random-permutation factor the bound becomes `(1/t!) sum_X 2^{-R(X)}`, and independent vertex retention contributes the corresponding `theta^t` factor.

## P19 — Uniform-rank first-moment barrier
**Status:** diagnostic negative theorem; architecture-specific

If a proof only uses `N^t` candidate ordered tuples with

\[
N=2^{\beta t+o(t)}
\]

and at most one independent binary equation per unordered pair, so `R(X)<=binom(t,2)`, then the strongest raw estimate has exponent

\[
(\beta-1/2)t^2+o(t^2).
\]

Therefore this **raw-count + uniform-rank** architecture cannot close once `beta>1/2`. This is not a universal impossibility theorem for all constructions.

## P20 — Two-cross-matrix bit ceiling
**Status:** diagnostic negative theorem

For `p_1~t/(1+C)` and `p_2~Ct/(1+C)`, the two cross matrices `M,N` contain asymptotically

\[
\frac{2C}{(1+C)^2}t^2
\]

bits. At `C_*=(1+sqrt3)/2` the coefficient is approximately `0.4880338717`, below the conditional target exponent `0.5358983848` by approximately `0.0478645131`. This is an information-budget diagnostic, not a theorem that all mixer constructions fail.

## P21 — Full mixed-product fiber obstruction
**Status:** `PROVED-IN-SESSION — TERMINAL FALSIFICATION ASSET`

On the full Cartesian product `D_{p_1} x D_{p_2}` under P15, fixing the right-coordinate pair `(b_1,b_2)` leaves a large fiber of all `(a_1,a_2)` satisfying `a_i·b_i=1`. The campaign proves that this is an exact independent-coordinate fiber for the mixed product, so the unthinned full Cartesian construction cannot be the desired high-quality SCC operator.

## P22 — Perfect matching in the valid-pair incidence graph
**Status:** `PROVED-IN-SESSION`

Let `H_p` be the bipartite graph with both sides `F_2^p\{0}` and

\[
a\sim b\iff a\cdot b=1.
\]

It is `2^{p-1}`-regular on both sides and therefore has a perfect matching. Hence there is a bijection

\[
\pi:\mathbb F_2^p\setminus\{0\}
\to
\mathbb F_2^p\setminus\{0\}
\]

with

\[
a\cdot\pi(a)=1
\]

for every nonzero `a`.

## P23 — Matching-restricted polarity digraph
**Status:** `PROVED-IN-SESSION`

Using a bijection `pi` from P22, define a digraph on `F_2^p\{0}` by

\[
a\to a'\iff a\cdot\pi(a')=0.
\]

Then the digraph is loopless, `T_{p+1}`-free, has exactly `2^p-1` vertices, and eliminates the repeated `a`- and `b`-coordinate fibers present in the full pair construction.

## Court

The campaign did **not** prove the approximate-supermultiplicative composition theorem required by P07, so it did **not** close the Erdős #77 limit question. Its public assets are the exact thin-corridor equivalence, the conditional closure theorem, the polarity/XOR/mixer algebra, the exact tensor-rank machinery, and the explicit falsifiers showing why the naive full-product and raw uniform-rank routes are insufficient.