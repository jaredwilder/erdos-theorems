# Erdős #243 — exact deviation-series reformulation

**Estate source:** MSL Day-2 audited release  
**Status:** exact structural identity; **canonical converse problem not closed**

Let

\[
2\le a_1<a_2<\cdots
\]

be integers and define the deviation from the Sylvester-type recurrence by

\[
d_n=a_{n+1}-(a_n^2-a_n+1).
\]

The campaign's strongest repaired asset is an exact telescoping identity that turns the reciprocal-series problem into a deviation-series problem.

## Theorem — exact deviation-series identity

For every finite `N`,

\[
\boxed{
\sum_{n=1}^{N}\frac1{a_n}
=
\frac1{a_1-1}
-
\frac1{a_{N+1}-1}
-
\sum_{n=1}^{N}
\frac{d_n}{a_n(a_n-1)(a_{n+1}-1)}.
}
\]

Consequently, since `a_n -> infinity`, whenever the infinite deviation series is interpreted by the convergent finite-telescope limit,

\[
\boxed{
\sum_{n\ge1}\frac1{a_n}
=
\frac1{a_1-1}
-
\sum_{n\ge1}
\frac{d_n}{a_n(a_n-1)(a_{n+1}-1)}.
}
\]

## One-step identity

The finite theorem is immediate from

\[
\frac1{a_n-1}
-
\frac1{a_{n+1}-1}
-
\frac1{a_n}
=
\frac{d_n}{a_n(a_n-1)(a_{n+1}-1)}.
\]

Indeed,

\[
a_{n+1}=a_n^2-a_n+1+d_n,
\]

and clearing denominators gives the identity by elementary algebra. Summing over `n` telescopes the first two terms.

## Why the reformulation matters

When every `d_n=0`, the recurrence is exactly

\[
a_{n+1}=a_n^2-a_n+1,
\]

and the correction series vanishes. Deviations from that recurrence contribute with explicit weight

\[
\frac1{a_n(a_n-1)(a_{n+1}-1)},
\]

which decays extremely rapidly once the sequence grows.

Thus a reciprocal-sum equality can be rewritten as an arithmetic cancellation condition on the integer deviations `d_n`. Instead of asking only about the global series, one may ask whether a nonzero integer deviation sequence can make the weighted correction sum vanish.

That is the exact structural reduction preserved by this release.

## Additional surviving irrationality barrier

The estate also keeps a separate, simpler theorem: if eventually

\[
a_n\mid a_{n+1}
\]

and

\[
\frac{a_{n+1}}{a_n}\to\infty,
\]

then

\[
\sum_n\frac1{a_n}
\]

is irrational. This is an independent denominator-growth obstruction and should not be conflated with the deviation identity.

## Correction boundary

An earlier #243 route contained a false telescoping formula. The identity displayed above was later independently algebraically reverified and is the authoritative repaired statement. The old formula remains quarantined in the MSL correction ledger.

## Formalization target

The natural Lean path is deliberately small:

1. prove the one-step field identity by clearing denominators;
2. sum it over `Finset.range N`;
3. telescope the boundary terms;
4. only afterward add the analytic limit under explicit hypotheses.

The finite identity is the kernel atom. The infinite statement should not be formalized by hiding convergence inside an algebraic rewrite.

## Boundary

This packet is a reformulation, not a solution of Erdős #243. Its value is that the canonical reciprocal condition becomes an exact deviation equation with integer numerators and rapidly shrinking rational weights.