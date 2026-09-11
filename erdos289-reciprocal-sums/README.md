# Erdős #289 — reciprocal-sum p-adic obstruction packet

**Estate source:** MSL Day-2 audited release  
**Status:** structural theorem packet + finite obstruction; **full Erdős #289 not closed**

The strongest general asset recovered from this campaign is a simultaneous all-prime necessary condition for finite integral reciprocal sums.

## Theorem 1 — all-prime p-adic obstruction

Let

\[
S\subset\{2,3,\ldots\}
\]

be finite and suppose

\[
\sum_{n\in S}\frac1n\in\mathbb Z.
\]

For a prime `p`, define

\[
U_p=
\sum_{\substack{n\in S\\p\mid n}}
\frac1{n/p}.
\]

Then

\[
\boxed{v_p(U_p)\ge1.}
\]

Equivalently, `U_p/p` is `p`-adically integral.

### Proof

Split the integral reciprocal sum as

\[
\sum_{n\in S}\frac1n
=
\sum_{\substack{n\in S\\p\nmid n}}\frac1n
+
\frac1p
\sum_{\substack{n\in S\\p\mid n}}\frac1{n/p}.
\]

The total is `p`-adically integral. The first sum is also `p`-adically integral because none of its denominators is divisible by `p`. Therefore

\[
\frac{U_p}{p}
\]

is `p`-adically integral, which is exactly `v_p(U_p)>=1`.

This turns one rational residual condition into a vector of local conditions, one for every prime appearing in the denominators.

## Theorem 2 — consecutive reciprocal intervals are nonintegral

Every nontrivial consecutive interval

\[
\sum_{n=a}^{b}\frac1n,
\qquad a<b,
\]

is nonintegral.

The classical 2-adic proof chooses a denominator with uniquely maximal power of two; after putting the sum over a common denominator, that term contributes odd parity at the maximal 2-adic level while all others contribute even parity.

A useful block version follows: in an integral sum of consecutive reciprocal blocks, the number of blocks attaining the global maximal denominator `v_2` signature must obey the corresponding parity cancellation requirement.

## The `[2,3]` head / `1/6` tail reduction

In the campaign branch where a decomposition of 1 contains the denominator 2, the run containing 2 is forced to be exactly

\[
[2,3],
\]

whose reciprocal sum is

\[
\frac12+\frac13=\frac56.
\]

Thus the remaining blocks must sum to

\[
\boxed{\frac16}
\]

and begin at denominator at least 5.

This is a structural reduction, not a complete classification.

## Exact finite obstruction

The audited estate records an exhaustive exact check that no single interval

\[
[a,b],
\qquad 5\le a<b\le60,
\]

satisfies

\[
\sum_{n=a}^{b}\frac1n=\frac16.
\]

Therefore within this finite frontier the `1/6` tail cannot be completed by one additional consecutive block; any candidate requires more block complexity or lies beyond the checked range.

**Scope:** finite exact obstruction only. It is not a proof that no such interval exists for arbitrary `a,b`.

## Search implication

A candidate should not be tracked only by its remaining rational sum. The all-prime theorem supplies a simultaneous local state:

\[
\bigl(v_p(U_p)\bigr)_p.
\]

That local-global vector can prune proposed reciprocal blocks before expensive global enumeration.

## Formalization target

The minimal reusable formal theorem is:

> if a finite reciprocal sum is integral, splitting at a prime `p` forces the `p`-divisible sub-sum, after removing one factor of `p` from each denominator, to have `p`-adic valuation at least one.

The proof is local and should not depend on the rest of the #289 problem machinery.

## Boundary

This packet does not solve Erdős #289. It releases a clean all-prime obstruction, a classical interval obstruction, a rigid `[2,3]` reduction, and a finite certified tail exclusion. Historical novelty of the general p-adic packaging remains to be adjudicated separately from its mathematical correctness.