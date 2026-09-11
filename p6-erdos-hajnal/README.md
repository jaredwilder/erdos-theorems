# P6 Erdős–Hajnal — six-vertex structural program

This directory is a **research-program mirror** for the induced-`P6` Erdős–Hajnal campaign. The flagship theorem is not certified here; the directory contains a substantial local structural theory, explicit candidates/negative results, bounded finite verification, and a map of the remaining proof obligations.

## Main mathematical record

`COURT-THEOREM-BANK-2026-08-06.md` contains **30 theorem assets**. Despite the historical filename, the useful reading order is mathematical:

- forbidden single-edge rectangle;
- crossing domination;
- common-nonneighbor / symmetric-difference completeness;
- profile-cover and near-twin clustering lemmas;
- low-degree agreement;
- trimmed exact-profile bounds;
- disjoint-defect classification;
- complete-minus-disjoint-rectangles normal form;
- sharp trace bound;
- an exact stable-slice pure-pair theorem;
- crown normal form;
- recursive-anchor structure;
- cotree bridge machinery.

The strongest local structural theorem is the crown normal form for stable interactions: after equal profiles are merged, the interaction is a blow-up of a complete bipartite graph minus a matching, with optional universal blocks.

## Finite verification

`ROUND11-LEAN-FEED-FINITE-CENSUS.md` and the theorem bank preserve exhaustive stable-matrix checks through `4 x 4`. Every bounded survivor in that census satisfies the crown normal form.

That finite verification is regression evidence for the local structure; it is not an unbounded proof of the P6 Erdős–Hajnal conjecture.

## Candidates, failed routes and remaining programs

`NEGATIVE-AND-CANDIDATE-BANK-2026-08-06.md` separates refuted routes and unproved candidates from the proved theorem bank.

`CLOSE-PROGRAMS-AND-MACHINE-MISSIONS.md` is a historical workflow document describing remaining proof programs. Its filename reflects the research process; it should not be read as the mathematical abstract of this directory.

## Repository status

This program has outgrown a broad theorem-bank mirror and warrants a dedicated P6 / Erdős–Hajnal repository. Until such a home exists, this README is the preferred human entry point and the historical files remain the detailed research record.
