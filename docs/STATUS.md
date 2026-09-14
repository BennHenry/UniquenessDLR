# Research and review status

Initial inventory: 14 September 2026.

This inventory describes the supplied sources and revision notes. No complete
proof or literature review has been performed as part of the repository setup.

## Starting material

The latest supplied full draft is
[`logarithmic_dlr_uniqueness_simplified.tex`](<../Raw materials/Revised 2/logarithmic_dlr_uniqueness_simplified.tex>).
The root [`main.tex`](../main.tex) is a separate working fragment. The existing
sources have been preserved without mathematical edits.

| Item | Location / label | Status and next check |
| --- | --- | --- |
| Comparison under integrated variance control | Full draft, `thm:comparison` | Proposed proof imported; review assumptions and dependencies in Sections 2–6. |
| Entropy and Fisher-information comparison | Full draft and working fragment, `prop:gap-entropy` | Compare the original proof with the unfinished alternative in `main.tex`; check each sign of the entropy estimate and the tilted-law bounds. |
| Random-interval conditioning and affine covariance | Full draft, `lem:random-dlr`, `lem:affine-covariance` | Awaiting review of conditioning and cutoff conventions. |
| Exterior-force bound and order of limits | Full draft, `prop:force`, Section 6 | Awaiting review of integrability, tightness, and the choice of confinement scale. |
| Finite energy implies integrated variance control | Full draft, `prop:energy-discrepancy` | Revision notes report prior algebraic checks; independently check the recovery-sequence hypotheses and limiting argument. |
| Convex inequalities on the singular simplex | Full draft, `lem:convex-approx` | Awaiting review of truncation and the weak Fisher-information domain. |
| Assiotis reference and comparison of DLR conventions | Full draft, Section 8; bibliography key `Assiotis` | Existing revision notes explicitly leave detailed references to arXiv:2609.06832v1 unverified. Check that version before relying on the comparison. |

## Known issues in the working fragment

- Compilation stops at line 273 with `Double superscript`: the final
  `\DLR^{\tiny pen}_{\Z}''` needs its superscript and derivative notation
  grouped correctly. Other uses of `\tiny` in math mode also produce warnings.
- `prop:gap-entropy` and `eq:fisher-gap` are each used twice.
- References to `lem:convex-approx`, `lem:varFormula`, and bibliography key
  `BEY` are unresolved within this file. The variance-formula lemma has no
  matching label.
- The section titled `New Pro` contains an unfinished proof and the placeholder
  `(trouver ref)`.
- Definitions supplied in the full draft are missing here. The fragment should
  not be read as a standalone proof of the full uniqueness claim.

These items are an initial inventory, not an exhaustive mathematical audit.

## First contributions

- Finish and check the alternative comparison proof in `main.tex`.
- Review one full-draft claim at a time and attach a record using the format in
  [CONTRIBUTING.md](../CONTRIBUTING.md).
- Verify the outstanding external citations against their precise versions.
- Assemble reviewed material into a maintained full manuscript while keeping
  the supplied revisions as provenance.

## Local build checks

Checked locally on 14 September 2026 with `latexmk` 4.87 and pdfTeX from
TeX Live 2025/Debian:

- `make manuscript`: passed; generated a 25-page PDF. The final log has no
  undefined references or citations, duplicate-label warnings, or overfull /
  underfull boxes. Nonfatal warnings concern disabled shell escape in
  `epstopdf` and font expansion.
- `make working`: failed at the pre-existing double-superscript error on
  line 273. No PDF was produced for this fragment.
- Local documentation links resolve. A source-label check found no duplicate
  labels or unresolved `\ref` / `\eqref` targets in the latest full draft.

Successful compilation does not change the mathematical review status above.
