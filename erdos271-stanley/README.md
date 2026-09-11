# Erdős #271 — Stanley sequences

**Campaign:** 2026-08-06  
**Target:** explicit terms and growth of the greedy Stanley sequence `A(n)`, centered on `A(4)`  
**Status:** **NOT CLOSED**

This directory publishes the audited mathematical estate of the campaign. The source dossier contains **184 ledger entries** with the following statuses:

- `RETAINED_PROVED`: 111
- `RETAINED_PROVED_WITH_CORRECTION`: 27
- `RETAINED_PROVED_SUBSUMED`: 1
- `CONDITIONAL_THEOREM`: 13
- `CONJECTURE_OR_TARGET`: 18
- `REFUTED_OR_RETIRED`: 7
- `COMPUTATIONALLY_VERIFIED_FINITE`: 4
- `EXPLORATORY_UNVERIFIED`: 2
- `EXTERNAL_DEPENDENCY`: 1

No historical novelty review was completed for the main reductions, and finite computations are not promoted to asymptotic theorems.

## Canonical notation

For the Stanley sequence seeded by `a_0=0, a_1=n`, write

\[
A_k=\{a_0,\dots,a_k\},\qquad g_k=a_{k+1}-a_k,
\]

\[
\Delta_k=\{a_k-a_i:0\le i\le k\},
\]

\[
U_k=\{2a_j-a_i:0\le i<j<k\},
\]

\[
m_k(x)=\#\{(i,j):0\le i<j<k,\ 2a_j-a_i=x\},
\]

and

\[
\mu_k=\frac{\binom{k}{2}}{|U_k|}.
\]

For `A(4)`, the seed omissions `1,2,3` must be treated explicitly:

\[
|U_k\cap[0,a_k)|=a_k-k-3.
\]

## Strongest retained compression

The campaign reduces fixed-seed Stanley growth to oriented-reflection multiplicity:

\[
a_k=\Theta\!\left(k+\frac{k^2}{\mu_k}\right).
\]

Using the external zero-density/superlinearity input for infinite Stanley sequences, this becomes

\[
a_k=\Theta\!\left(\frac{k^2}{\mu_k}\right).
\]

For `A(4)`, the historic growth claim is therefore equivalent to

\[
a_k=\Theta(k^2/\log k)
\iff
\mu_k=\Theta(\log k)
\iff
|U_k|=\Theta(k^2/\log k).
\]

The final machine minimum cut is to prove matching support bounds

\[
c\frac{k^2}{\log k}\le |U_k|\le C\frac{k^2}{\log k}
\]

for all sufficiently large `k`.

## Exact retained dynamics

The campaign banked, among other statements:

- **Single-State Obstruction:** `g_k` is the least positive integer absent from `Δ_k-2Δ_k`.
- **Decimated autocorrelation:** `C_k(d)=#{ε∈Δ_k:2ε+d∈Δ_k}` and `g_k=min{d≥1:C_k(d)=0}`.
- **Correlation transport:** `C_{k+1}(d)=C_k(d+g_k)+1_{Δ_k}(d-g_k)`.
- **Hole survival:** `r∈H_{k+1}` iff `r+g_k∈H_k` and `r∉g_k+Δ_k`.
- **Gap-drop law:** `g_{k+1}<g_k` iff `H_k∩(g_k,2g_k)≠∅`.
- **Reflection-union recurrence:** `a_k=min{m>a_{k-1}:m∉U_k}` and `U_{k+1}=U_k∪(2a_k-A_{k-1})`.
- **First-kill partition:** reflection-killed nonmembers decompose into unique first-kill sets, with the seed omissions handled separately.
- **Collision-cover theorem:** colliding indices are exactly `A_j ∩ ⋃_{r<j}(2(a_j-a_r)+A_r)` with the temporal-prefix convention.
- **Asymptotic reservoir elimination:** for every fixed seed, `liminf η_k≥1/2`.
- **Multiplicity-growth law:** in the superlinear regime, term growth is exactly comparable to `k^2/μ_k`.

## Correction / refutation bank

The release preserves failed routes rather than deleting them. In particular:

- a single primitive finite transition matrix cannot explain permanently different power-law peak/trough exponents;
- bounded physical windows do not determine the decimated correlations;
- the visible `A(4)` gap blocks do not obey a simple literal one-scale substitution in the tested data;
- the converse of the large-gap maximal-yield theorem is false;
- frontier-fresh yield does not dominate total first-kill yield in the tested range;
- the future-reservoir escape cannot change the growth order because utilization has asymptotic lower bound `1/2`;
- the proposed **Ternary Scale Mixing Lemma** was not promoted: its absolute per-scale multiplicity clause conflicts with exact checkpoint maxima `7,9,10,11,15,19` through `k=2048`.

## Exact finite audit

The dependency-free packaged audit regenerated 2,049 terms of `A(4)` and checked reflection support/multiplicity at six checkpoints. At `k=64,128,256,512,1024,2048`, the reported mean multiplicities were approximately `2.1515, 2.6772, 3.0743, 3.2878, 4.0795, 4.2782`; maximum multiplicity rose from `9` to `21`; within-scale maximum rose from `7` to `19`; utilization stayed above `0.51`. These are exact finite observations only, not asymptotic proof.

## Files

The full 184-entry ledger is published in round-ordered chunks in this directory. Status labels are load-bearing. `RETAINED_PROVED`, `CONDITIONAL_THEOREM`, `COMPUTATIONALLY_VERIFIED_FINITE`, `CONJECTURE_OR_TARGET`, and `REFUTED_OR_RETIRED` must not be conflated.
