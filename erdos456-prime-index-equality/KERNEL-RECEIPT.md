# Erdős #456 — prime-index equality family, verified Lean receipt

**Author:** Jared Wilder  
**Public formal-receipt release:** 2026-09-11

Recovered source path:

```text
oracle/evidence/msl-machine/campaigns/erdos456-campaign-001/kernel/Erdos456Equality.lean
```

Kernel runner result:

```text
status=VERIFIED
backend=wsl
exitCode=0
seconds=3.4
needsMathlib=true
project=/root/erdosfire-bench/proofs
```

Verified declarations:

```text
erdos456_m_eq_p
erdos456_p_eq_p
```

Both were reported clean with the ordinary Mathlib footprint

```text
[propext, Classical.choice, Quot.sound]
```

and no `sorryAx`.

## The theorem

For every odd prime `p`, at `n=p-1` the two frozen campaign quantities satisfy

\[
\boxed{m_n=p_n=p.}
\]

The first declaration proves the totient-preimage side: `(p-1)|phi(p)` and no smaller positive `m<p` has `(p-1)|phi(m)`. The second proves the prime-in-residue-class side: `p≡1 mod (p-1)` and no smaller prime has that congruence.

The endpoint `p=2` is deliberately excluded; under the campaign convention it is exceptional.

## Authority / novelty boundary

The audit classifies this as `KNOWN_EXTERNALLY_FORMALIZATION`: the mathematics was already present in public remarks, while this Lean artifact supplies formal provenance. The parent problem is not claimed solved.

The original standalone `.lean` bytes remain to be mirrored exactly; this receipt records the verified artifact without fabricating missing source text.
