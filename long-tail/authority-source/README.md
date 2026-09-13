# Canonical 56-asset gold registry — full authority source

This directory preserves the **exact recovered authority source** behind `../CANONICAL-GOLD-56-STATEMENTS.md`.

The statement page is the reader-facing theorem/status index. The authority source is different: it preserves the per-asset proof/certificate paragraph, kernel receipt name where present, formal-scope warning, correction, blacklist, and semantic-quarantine note.

## Exact source identity

- source filename: `01-CANONICAL-GOLD.md`
- source bytes: `31,556`
- source SHA-256: `a5eada56610ec5c8fbb6a2146cb9d56813dbd4d1900d9f8079a33a0c0b90b7f4`
- deterministic gzip filename: `01-CANONICAL-GOLD.md.gz`
- gzip bytes: `9,961`
- gzip SHA-256: `f06161773e53b4db06bf7eb8e3d4664edd8c8f28e31db438920b64bd6c9e8508`

Reconstruct the exact Markdown source with:

```bash
gzip -dc 01-CANONICAL-GOLD.md.gz > 01-CANONICAL-GOLD.md
sha256sum 01-CANONICAL-GOLD.md
```

The expected SHA-256 is the source hash above.

## Authority rule

The source begins: **“Curated assets: 56. This registry supersedes all earlier promotion lists.”**

Its status vocabulary is load-bearing:

- `KERNEL_CHECKED` means the listed theorem scope was previously audited as matching the kernel artifact.
- `KERNEL_CHECKED_FINITE_ONLY`, `KERNEL_CHECKED_SINGLE_INSTANCE_ONLY`, and similar scope notes do **not** certify a universal theorem.
- `MISLEADING_RECEIPT_QUARANTINED` means a green-looking formal receipt is semantically unfit to support the listed mathematical claim.
- `MATHEMATICALLY_AUDITED_LEAN_READY` is mathematical/prose authority, not a claim of completed universal Lean certification.

Examples preserved in the source include #359's semantically quarantined receipt, #153's single-instance-only receipt, #394/#727 finite-only receipts, the corrected #291 and #377 criteria, and explicit blacklists for false stronger rows in #145, #241, #406 and #885.

This publication therefore closes the previous gap between the **56-statement surface** and the **full recovered proof/authority record**. It does not make any historical-novelty claim and does not upgrade any asset beyond the status recorded in the source.