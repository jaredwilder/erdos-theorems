# Erdős #885 — factor-difference / square duality, verified Lean receipt

**Author:** Jared Wilder  
**Public formal-receipt release:** 2026-09-11

Recovered source path:

```text
oracle/evidence/msl-machine/campaigns/erdos885-campaign-001/kernel/Erdos885Duality.lean
```

Kernel runner result:

```text
status=VERIFIED
backend=wsl
exitCode=0
seconds=4.6
needsMathlib=true
project=/root/erdosfire-bench/proofs
```

Verified declaration:

```text
erdos885_factor_difference_square
```

Recorded axiom footprint:

```text
[propext, Classical.choice, Quot.sound]
```

No `sorryAx` is present in the receipt.

## Mathematical theorem

For `N>=1` and `d>=0`,

\[
\boxed{
d=|a-b|\text{ for some }ab=N
\iff
\exists s\ge0,\ s^2=d^2+4N.
}
\]

Forward is `(a+b)^2=(a-b)^2+4ab`. Reverse reconstructs

\[
a=(s+d)/2,\qquad b=(s-d)/2,
\]

using the parity forced by `s^2-d^2=4N`.

This turns the canonical common-factor-difference problem into a simultaneous integral-square problem and is the correct algebraic language behind a historically failed LCM construction.

## Authority boundary

This is a green verified structural theorem. The canonical #885 problem remains open. Historical novelty is not asserted merely from the formal receipt.

The original standalone source bytes are still a source-recovery item; this public file preserves the exact green receipt and theorem identity without inventing missing bytes.
