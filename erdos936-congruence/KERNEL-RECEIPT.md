# Erdős #936 — exact mod-9 congruence, verified Lean receipt

**Author:** Jared Wilder  
**Public formal-receipt release:** 2026-09-11

Recovered source path:

```text
oracle/evidence/msl-machine/campaigns/erdos936-campaign-001/kernel/Erdos936Congruence.lean
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

Verified declarations:

```text
erdos936_period
erdos936_nine_dvd_iff
```

Recorded footprints:

```text
erdos936_period        : [propext, Quot.sound]
erdos936_nine_dvd_iff : [propext, Classical.choice, Quot.sound]
```

No `sorryAx` is present in the receipt.

## Mathematical theorem

The powers of 2 modulo 9 have period 6, and consequently

\[
\boxed{9\mid 2^n+1\iff n\equiv3\pmod6.}
\]

This is an exact local structural theorem used in the campaign's study of powerful values of `2^n+1`. It does not establish the global finiteness statement.

## Authority boundary

The formal artifact is green/verified at the recorded environment. The result is elementary local structure, not a parent-problem close or novelty claim. The exact original `.lean` file bytes remain to be mirrored when recovered as a standalone file; this ledger preserves the verified receipt meanwhile.
