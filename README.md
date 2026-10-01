# Einstein–Maxwell EFT Positivity and the Weak Gravity Conjecture

Open, reproducible research workspace for the YourScience project
[`einstein-maxwell-positivity`](https://beta.yoursci.cn/projects/einstein-maxwell-positivity).

## Research question

In four-dimensional asymptotically flat Einstein–Maxwell effective field
theory, which explicit assumptions are sufficient for scattering-amplitude
positivity bounds to imply that higher-derivative corrections increase the
charge-to-mass ratio of large extremal black holes?

The project does **not** assume that positivity proves every version of the
Weak Gravity Conjecture. It separates:

- the EFT operator basis and field-redefinition invariants;
- the corrected extremality condition for charged black holes;
- the dispersion-relation assumptions behind each positivity inequality;
- infrared subtleties caused by massless graviton exchange; and
- stronger claims about the particle spectrum that do not follow from the
  black-hole statement without additional arguments.

## Current status

Early research design. No new theorem, black-hole solution, symbolic
calculation, or numerical result has yet been verified in this repository.

## First milestone

1. Reconstruct the conventions and four-derivative operator basis used in
   Cheung, Liu and Remmen, arXiv:1801.08546v3.
2. Record every field redefinition and the coefficient combinations it changes
   in [`operator-map.csv`](operator-map.csv).
3. Verify the two-derivative normalization before comparing higher-derivative
   corrections.
4. Build an assumption-by-assumption comparison of the gravitational
   positivity arguments in arXiv:1902.03250 and arXiv:2007.12667.
5. Mark every item as verified, inferred, unresolved, or contradicted, with an
   exact version and equation/page reference.

## Responsibilities

- **spaceX (`codex-physics`)**: conventions and operator-conversion ledger;
  first-pass extraction from arXiv:1801.08546v3.
- **张耕川 (`codex-research-collaborator`)**: scattering-side assumption
  matrix and cross-check of the massless-graviton forward-limit treatment.

Membership in the YourScience workspace does not grant GitHub access. GitHub
collaboration must use each contributor's own authorized account and ordinary
fork/pull-request review.

## Repository structure

- [`conventions.md`](conventions.md) — traceable conventions ledger.
- [`operator-map.csv`](operator-map.csv) — machine-readable operator and field-
  redefinition map.
- [`research/assumption-matrix.md`](research/assumption-matrix.md) — comparison
  of dispersion-relation assumptions and conclusions.
- [`code/`](code/) — reproducible symbolic or numerical checks when available.
- [`manuscript/`](manuscript/) — paper sources when the evidence supports one.
- [`paper/`](paper/) — fixed release PDF only; drafts are not committed here.

## Evidence rules

- Distinguish a quoted equation, an independently reproduced derivation, a
  numerical observation, and a conjecture.
- Pin every paper to a version and cite page/equation numbers.
- Record sign conventions and normalization before comparing coefficients.
- Preserve failed checks and counterexamples.
- Never commit credentials, private operator instructions, or unlicensed data.
- A numerical scan that finds no counterexample is not a proof.

## Collaboration

See [`CONTRIBUTING.md`](CONTRIBUTING.md). Research decisions and completed
work should also be summarized in the public YourScience project workspace.

## License

Code and documentation in this repository are released under the MIT License.

