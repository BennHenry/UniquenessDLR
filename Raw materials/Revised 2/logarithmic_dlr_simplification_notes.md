# Integration of the variance and energy simplification

**Revision date:** 10 September 2026  
**Baseline:** `logarithmic_dlr_uniqueness_revised.tex` (the previous 27-page revision)  
**New source:** `logarithmic_dlr_uniqueness_simplified.tex`  
**Compiled manuscript:** `logarithmic_dlr_uniqueness_simplified.pdf` (25 pages)

## Scope and location of changes

This revision integrates the simplification discussed in the conversation. The two main theorem numbers remain 1.1 and 1.2. The single integrated variance condition replaces the three separately stated discrepancy assumptions; its two consequences are proved immediately afterward. The stationary-field construction and covariance-spectral argument have been replaced by an intrinsic-energy calculation and Leblé's recovery sequence.

| Location in the new manuscript | Change |
|---|---|
| Abstract and introduction | State the single discrepancy hypothesis and describe the intrinsic-energy/recovery-sequence proof. |
| Theorem 1.1, equation (1.6), page 3 | The only discrepancy hypothesis is `V(P) = integral_1^infinity v_P(t)/t^2 dt < infinity`. The stationary, simple, unit-intensity, canonical DLR assumptions are unchanged. |
| Lemma 1.3, equations (1.7)–(1.9), pages 3–4 | Derives finite local second moments, the linear bound, and the sublinear limit from the integrated hypothesis. |
| Lemma 7.1, equations (7.5)–(7.8), page 19 | Retains the normalization and intensity argument; adds the explicit identification with Leblé's electric energy. |
| Section 7.2 and Lemma 7.3, pages 20–21 | Defines the reduced second factorial moment measure and intrinsic energy, proves the exact finite-window identity, and obtains the integrated bound for bounded-variance processes. |
| Proposition 7.4, equations (7.16)–(7.18), page 21 | Applies the recovery sequence and Fatou's lemma to every stationary finite-energy process, without DLR or ergodicity assumptions. |
| Proof of Theorem 1.2, page 22 | Applies Theorem 1.1 directly to the candidate and Sine-beta; removes the ergodic decomposition. |
| Section 8 and bibliography | Updates the discussion to the single-hypothesis formulation and adds the precise Leblé reference. |

The comparison calculations in Sections 2–6 remain unchanged. The introductory sentences of Sections 3 and 6 now invoke Lemma 1.3 to supply the two derived variance estimates. The appendix is unchanged. Equation labels for the integrated, linear, and sublinear estimates are retained, although their order and printed numbers have changed. The old stationary-field and spectral labels and the unused spectral-measure macro are removed.

## 1. One discrepancy hypothesis

Write

\[
\mathcal V(P)=\int_1^\infty\frac{v_P(t)}{t^2}\,dt.
\]

The new Lemma 1.3 proves

\[
\frac{v_P(t)}{t}\le18\int_t^{3t}\frac{v_P(u)}{u^2}\,du,
\qquad t>0.
\]

Its proof uses only stationarity and the decomposition of centered counts on two adjacent intervals. The tail integral tends to zero when `V(P)` is finite, giving sublinear variance. The same inequality at large scales, followed by a disjoint-interval argument at scales below one, gives the explicit admissible constant

\[
v_P(t)\le\bigl(36\mathcal V(P)+2\bigr)t,
\qquad t>0.
\]

Finite local second moments are established before the stationary-increment calculation. No uniform constant over candidate processes, power-law decay rate, or quantitative hyperuniformity theorem is added as an assumption. Thus the reformulation does not change the class of processes covered by the previous Theorem 1.1.

## 2. Imported result versus the new deduction

The added reference is:

**Thomas Leblé, _Logarithmic, Coulomb and Riesz energy of point processes_, Journal of Statistical Physics 162 (2016), no. 4, 887–923. DOI: 10.1007/s10955-015-1425-4.**

The internal reference numbers used in the revision were checked in **arXiv:1509.05253v1**, submitted 17 September 2015:

- Equations (3.1)–(3.4) give the electric-energy definitions and normalization.
- Equation (3.12) gives the intrinsic-energy expression for stationary processes.
- Proposition 5.3 and equation (5.7) supply the recovery sequence with convergent intrinsic energies.
- Equation (2.3) uses the stronger bounded-number-variance meaning of hyperuniformity in dimension one. The proof needs this bound separately for each approximation, not uniformly across the sequence.
- Section 5.2.1 regularizes the finite configurations by separating close points; the recovery processes can consequently be taken simple.

The integrated estimate is **not attributed to Leblé as a verbatim theorem**. The manuscript proves the interval-counting identity and the passage to the limit explicitly. No planar hyperuniformity theorem is applied to the one-dimensional logarithmic model.

## 3. Exact intrinsic-energy identity and normalization

Section 7.2 defines the positive reduced second factorial moment measure `alpha_Q`, without assuming that it has a density. With ordered pairs,

\[
A_Q(t)=\mathbb E_Q[N_{(0,t]}(N_{(0,t]}-1)]
      =v_Q(t)+t^2-t
      =\int(t-|h|)_+\,\alpha_Q(dh).
\]

Writing `e_R(Q)` for the finite-window intrinsic energy per unit length and

\[
w_R(t)=t^{-2}+(Rt)^{-1},
\]

the new equation (7.14) is

\[
e_R(Q)+\frac{\log R}{R}v_Q(R)+2-\frac1{2R}
 =\int_0^1w_R(t)A_Q(t)\,dt
  +\int_1^Rw_R(t)v_Q(t)\,dt.
\]

The argument applies Tonelli to a nonnegative logarithmic kernel before subtracting finite background terms. It does not integrate by parts through the singularity, assume a pair-correlation density, or assume the desired variance integrability. Bounded variance makes the boundary term vanish, yielding

\[
\mathcal V(Q)\le W^{\mathrm{int}}(Q)+2.
\]

Leblé's approximations and lower semicontinuity of the centered squared interval counts then give, by Fatou,

\[
\mathcal V(P)\le W^{\mathrm{elec}}(P)+2
               =2+\frac1{2\pi}\mathbb E_PW.
\]

The last equality uses the retained unit-background convention and the new explicit normalization identity (7.6). No uniform integrability of squared counts is asserted or needed.

## 4. Consequence for the finite-energy uniqueness proof

The new Proposition 7.4 applies to any stationary finite-energy law, not merely an ergodic DLR component. Therefore a candidate and Sine-beta can be placed directly in the class of Theorem 1.1. The existing DLR and finite-energy existence inputs for Sine-beta are retained, but the decomposition into ergodic components and its associated citation are no longer needed in this proof. The remaining discussion of regularity in Section 8 was also updated to apply directly to a stationary law.

## 5. Checks and retained limitations

The source compiles with `latexmk -pdf` / `pdflatex` using the existing standard packages. The final PDF has 25 pages. Checks found no undefined citations, undefined cross-references, duplicate labels, overfull boxes, or underfull boxes. All pages were rendered; the layout was inspected, including the new theorem, lemma, energy identity, recovery-sequence proof, and bibliography. A coordinate check found no text outside the page bounds. A nonfatal pdfTeX font-expansion warning occurs when the bibliography's sans-serif math font is first loaded; no missing-glyph or layout problem was observed.

The logarithmic kernel identity and background integrals were checked symbolically. As an independent algebraic check, the exact finite-window identity was evaluated for the uniformly translated unit lattice at several integral and nonintegral window lengths; the residual was at floating-point rounding level. These checks support the displayed calculation, but are not a certification of the complete uniqueness proof.

**The earlier limitation concerning the detailed Assiotis citations remains.** The original manuscript's assertions and reference numbers for arXiv:2609.06832v1 have been preserved; those details were not independently reverified in this integration. The present work verifies and integrates the new Leblé-based argument, rather than rechecking every external reference or every part of the manuscript.

## Files in the package

The package contains the new LaTeX source, its compiled PDF, these notes, and `logarithmic_dlr_simplification.diff`, a unified source diff against the immediately preceding revised LaTeX file. The earlier files remain unchanged.

To compile the new source:

```sh
latexmk -pdf -interaction=nonstopmode -halt-on-error logarithmic_dlr_uniqueness_simplified.tex
```
