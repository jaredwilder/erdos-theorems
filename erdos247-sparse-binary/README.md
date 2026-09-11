# Erdős #247 — sparse binary expansions

**Estate source:** MSL Day-2 audited mathematical release  
**Status:** rigorous partial theorem packet; **canonical transcendence target not closed**

Let

\[
a_1<a_2<\cdots
\]

be positive integers and define

\[
\alpha=\sum_{n=1}^\infty 2^{-a_n}.
\]

The campaign works under the canonical sparse-position hypothesis

\[
\limsup_{n\to\infty}\frac{a_n}{n}=\infty.
\]

## Theorem 1 — sparse binary position implies irrationality

Under the hypothesis above,

\[
\boxed{\alpha\notin\mathbb Q.}
\]

### Proof

Suppose `alpha` were rational. A rational number has an eventually periodic binary expansion (after choosing the nonterminating/terminating convention consistently).

The expansion of `alpha` has 1-bits exactly at the positions `a_n`. There are infinitely many of them. An eventually periodic binary expansion with infinitely many 1-bits has positive asymptotic density of 1-bits: once the periodic tail begins, the repeating block contains at least one 1.

Positive lower density of the 1-bit positions implies

\[
a_n=O(n),
\]

contradicting

\[
\limsup a_n/n=\infty.
\]

Therefore `alpha` is irrational.

## Theorem 2 — inverse-density equivalence

Let

\[
A(N)=\#\{n:a_n\le N\}.
\]

Then

\[
\boxed{
\limsup_{n\to\infty}\frac{a_n}{n}=\infty
\iff
\liminf_{N\to\infty}\frac{A(N)}N=0.
}
\]

### Forward direction

At `N=a_n`,

\[
A(a_n)=n,
\qquad
\frac{A(a_n)}{a_n}=\frac n{a_n}.
\]

A subsequence with `a_n/n -> infinity` therefore gives counting-density values tending to zero.

### Reverse direction

If `A(N_j)/N_j ->0`, put `n_j=A(N_j)+1`. Then `a_{n_j}>N_j`, so

\[
\frac{a_{n_j}}{n_j}
>
\frac{N_j}{A(N_j)+1},
\]

which is unbounded along a suitable subsequence.

## Workflow correction

A later registry event in the source estate marked Theorem 2 false using an alleged example with positive lower counting density but unbounded `a_n/n`. Such an example cannot exist by the identity

\[
A(a_n)/a_n=n/a_n.
\]

The mathematical theorem therefore overrides the later workflow label. This is retained as a regression test for theorem-state reconciliation.

## Base-`b` version

The same eventual-periodicity argument works for fixed integer base `b>=2`: if the nonzero digits of a base-`b` expansion occur only at positions `a_n` with `limsup a_n/n=infinity`, and the series contains infinitely many nonzero digits in a fixed finite digit alphabet, the resulting real cannot be rational unless carries/representation ambiguity change the asserted digit support. In the binary `{0,1}` series above there is no carry issue.

## Boundary

Erdős #247 asks for a substantially stronger conclusion: **transcendence**. This packet proves irrationality on the canonical sparse-position hypothesis; it does not bridge irrationality to transcendence.

Historical novelty of the irrationality milestone has not been certified by this repository. The result is released because it is clean mathematics recovered from the estate, not because a novelty claim has been granted.