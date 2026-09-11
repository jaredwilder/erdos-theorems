# Erdős #885 — factor differences as square conditions

**Estate source:** MSL Day-2 audited release  
**Status:** exact structural theorem; **full #885 remains open**

For a positive integer `N`, define a factor difference to be a nonnegative integer

\[
d=|a-b|
\]

for positive integers `a,b` satisfying `ab=N`.

The campaign's strongest repaired asset is the exact conversion of this factorization condition into a square condition.

## Theorem 1 — factor-difference square criterion

For `N>=1` and `d>=0`, the following are equivalent:

1. there exist positive integers `a,b` with `ab=N` and `|a-b|=d`;
2. `d^2+4N` is a perfect square, with the corresponding parity needed to recover the factors.

More explicitly, after ordering `b=a+d`,

\[
N=a(a+d).
\]

Then

\[
(2a+d)^2=d^2+4N.
\]

Conversely, if

\[
s^2=d^2+4N
\]

and

\[
2\mid(s-d),
\]

put

\[
a=\frac{s-d}{2},
\qquad
b=\frac{s+d}{2}.
\]

Then

\[
ab=\frac{s^2-d^2}{4}=N
\]

and `b-a=d`.

Thus the clean integer core is

\[
\boxed{
N=a(a+d)
\iff
\exists s:\ s^2=d^2+4N\ \land\ 2\mid(s-d),
}
\]

with positivity conditions on the recovered factor as appropriate.

## Why this is a useful change of language

The original factor-difference condition couples two unknown factors. The theorem replaces it with an integral-point condition

\[
s^2-d^2=4N.
\]

For several integers `N_i` and desired common differences `d_j`, the target becomes a simultaneous system

\[
d_j^2+4N_i=s_{ij}^2.
\]

That is a family of conics / difference-of-squares equations. Structured approaches can therefore use Pell equations, common integral points, congruence obstructions, or exact Diophantine search rather than repeatedly enumerating factorizations.

## Killed construction

An earlier campaign branch proposed

\[
N_i=i\operatorname{lcm}(1,\ldots,2k)
\]

and implicitly relied on `0` being a common factor difference.

That route is false because

\[
0\text{ is a factor difference of }N
\iff
N\text{ is a perfect square}.
\]

The proposed `N_i` are not all squares. The construction is quarantined; the square-duality theorem survives independently and was the useful mathematics hidden underneath the failed route.

## Concrete next target from the campaign

The source audit records the problem as open beyond the small solved values known to the campaign. A natural exact next step is to construct or rule out a `k=5` configuration by solving the simultaneous square system above with a replayable certificate.

This repository does **not** claim such a construction.

## Formalization target

Avoid `Nat.sqrt`. Formalize the integer equivalence directly:

- forward witness `s=2a+d`;
- reverse witness `a=(s-d)/2` using the parity hypothesis;
- `nlinarith`/ring arithmetic after clearing the division by two.

This is both stronger and cleaner than a bounded square-root computation.

## Boundary

The theorem is exact and elementary. Its historical novelty is not asserted. Its release value is as a durable structural interface for the open factor-difference problem and as a repaired replacement for a false LCM construction.