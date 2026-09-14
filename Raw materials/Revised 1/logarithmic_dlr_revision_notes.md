# Revision notes: logarithmic DLR uniqueness manuscript

**Revision date:** 10 September 2026  
**Source:** `logarithmic_dlr_uniqueness_corrected(1).tex`  
**Revised manuscript:** `logarithmic_dlr_uniqueness_revised.tex` and its compiled, 27-page PDF.

## Scope

This is a full-manuscript exposition and notation revision addressing the three requested concerns. The two main theorem statements, their variance and finite-energy hypotheses, the eight-section organization, the appendix, and the bibliography have been retained. All 19 theorem, proposition, and lemma environments and all original cross-reference labels remain. The revision adds 40 equation labels and one subsection label; equation numbering consequently differs from the original.

The central proof strategy is unchanged: compare two candidate conditional laws with the same finite-dimensional reference measure, eliminate the reference expectation, identify the Palm gap laws, and apply Palm inversion. The electric-energy argument remains a separate verification of the discrepancy assumptions. No limiting law for the reference measure and no uniform first-moment bound for the conditional force contribution have been added as assumptions or conclusions.

## 1. Results and intermediate steps stated as equations

| Location | Revised equations | Change |
|---|---|---|
| Canonical DLR specification | (1.3)–(1.5) | Relative Hamiltonian, partition function, ordered Gibbs kernel, and conditional-expectation identity. |
| Lattice reference energy | (2.2) | An exact gamma-function formula replaces the unspecified additive constant. |
| Entropy and Fisher information | (2.6) | Definitions, absolute-continuity convention, and the weak Sobolev domain are stated explicitly. |
| Palm notation and regularity | (3.1)–(3.6) | Campbell identity, indexed points and gaps, density limits, reciprocal principal value, and oriented discrepancy. |
| Spatial-to-Palm gap averages | (3.10)–(3.11) | The average and its limiting expectation have explicit summation indices. |
| Random-interval DLR laws | (4.1)–(4.4) | Conditional law, affine pushforward, and the uniform cutoff-center error. |
| Endpoint distance and displacement | (4.5); (4.10) | Probability quantifiers, two Chebyshev bounds, and the intermediate quadratic-displacement inequalities. |
| Half-line and exterior forces | (5.3)–(5.4); (5.9) | Scaled bounds and the exact signed left/right decomposition, including the density-mismatch term. |
| Conditional convergence | (6.6)–(6.7) | The passage from tightness to convergence in probability, followed by bounded convergence in mean. |
| Electric-field conventions | (7.1)–(7.4); (7.8) | Planar embedding, divergence constraint, truncation, energy limits, and the stationary joint law. |
| Spectral argument | (7.18)–(7.19) | The duality coefficient and resulting low-frequency bound are given explicitly. |
| Ergodic decomposition and Sobolev domain | (7.22); (A.1) | The mixing measure and the weighted weak Sobolev space are defined by formulas. |

Several short calculations were also expanded without changing the conclusions. These include the mixture-variance lower bound, the midpoint-to-lattice displacement comparison, both reflected interior-count inequalities, the Schur-test integrals for the half-line kernel, the common confinement-scale argument, and the finite-energy expectation on almost every ergodic component.

## 2. Definitions and notation

The introductory notation subsection now specifies the configuration space, translations, restrictions of counting measures, pushforwards, intensity, expectations, variance, the identity matrix, and the probabilistic asymptotic notation. The preliminary comparison formula that formerly appeared before its symbols were defined has been replaced by precise references to the estimates in Section 2.

The canonical DLR property is no longer defined only by a prose description. It is stated through a relative Hamiltonian and a normalized conditional kernel, with the exterior, particle number, reference configuration, and symmetric-cutoff convention specified. The zero-particle case is stated separately.

The oriented discrepancy `D_0` now has an explicit definition on both positive and negative arguments. The difference between the forward and backward half-open endpoint conventions is acknowledged. The Palm distribution, successor shift, two-sided point enumeration, and gap indices are introduced together. The rooted block average is distinguished from the spatially rooted average.

The force argument consistently uses left/right labels `L` and `R`. In particular, its outward exterior counts, discrepancy bounds, interior counts, and conditional expectations are defined separately. This removes the earlier need to infer that a plus label referred to the left endpoint while a minus label referred to the right endpoint. The directions of the Palm counts `C^+` and `C^-` remain unchanged.

The covariance spectral measure is denoted by the distinct symbol `\mathsf S_P` (source macro `\Spec`), while `S(\mu\mid\omega)` remains relative entropy. `\Id_K` replaces uses of `I` for the identity matrix, avoiding confusion with Fisher information. The temporary scalar entropy abbreviation in the optimization step is now introduced explicitly. The appendix's auxiliary information functional is denoted by `\mathscr I_D`, rather than reusing the letter associated with the quadratic displacement cost.

In Section 7, the embedded planar counting measure is distinguished from the original measure on the line. The horizontal translation of a field, the joint probability law, the expectation convention, the circle measure used for truncation, and the local negative Sobolev space are specified. The vertical cutoff is no longer named with the same symbol as the retained exterior configuration.

## 3. Terminology and explanation

Vague descriptions have been replaced by the relevant mathematical object or operation. For example, “stationary electric lift” is now a stationary joint law of a configuration and a field, together with its marginal and invariance identities. “Fibre” is replaced by the defined set of configurations with a fixed particle number. “Relative exterior move” is described as a relative exterior interaction difference. “A signed version of” the logarithmic force term is replaced by the actual signed decomposition.

Statements that a dependence is “harmless” now explain the order of limits or the event of probability one that justifies it. The phrase “uniformly in the limiting K-range” has been replaced by the precise limit-superior assertion. The point-shift, conditional-count, and Palm-inversion arguments keep their standard terminology, but the associated maps and quantities are defined.

Theorem and lemma titles have been adjusted where useful to name their actual conclusions: concentration of the endpoint distance, subquadratic expected displacement, and tightness of the conditional squared force difference. Their labels and numbering scheme have been preserved.

## 4. Mathematical clarifications distinguished from changes of hypothesis

The exact gamma-function expression includes the reference-point normalization that was formerly hidden in “constant.” It describes the same lattice Hamiltonian.

The spectral coefficient `1/(2*pi^2)` is obtained directly from the manuscript's field-pairing and test-energy identities by Cauchy–Schwarz. The low-frequency bound with coefficient `2/pi^2` is the quantitative consequence of the same calculation and the existing lower bound on the smoothing multiplier. These coefficients use the manuscript's stated Fourier and electric-energy normalizations.

In the appendix, a potential assumed only to be `C^2` is no longer described as smooth without explanation. A local mollification step is stated before the smooth-domain argument; it preserves the Hessian lower bound and permits passage back to the given `C^2` potential. The weighted Sobolev definition is formulated for a positive continuous density and still imposes no boundary trace condition.

The added algebra and quantified formulations are intended to expose the steps already used by the original argument, not to substitute a different proof or a stronger regularity hypothesis. This editorial work is not an independent certification of the complete uniqueness proof.

## 5. Reference-checking limitation

The existing comparisons with Assiotis's September 2026 preprint, `arXiv:2609.06832v1`, have been preserved. Its full text could not be retrieved through the available web access during this revision. Its detailed theorem, proposition, and definition numbering, and the asserted correspondence of conventions, therefore remain to be checked against that precise version before submission. No replacement claim was supplied from memory.

The Leblé–Serfaty corrected manuscript dated 9 May 2017 was consulted for the field/energy definitions and the cited linear-discrepancy statement. This limited inspection is not a complete verification of every external result used in the manuscript. Existing bibliography entries and their version qualifiers have not been silently updated.

## 6. Delivery checks

The revised source compiles with `pdflatex` using standard packages. The final compilation reports no undefined references or citations, duplicate labels, overfull boxes, or underfull boxes. The PDF was rendered and visually inspected; theorem, proposition, and lemma statements are kept together, with their proofs allowed to break normally. A separate word-coordinate check found no text outside the printable page bounds.

The accompanying unified patch records source-level changes against the uploaded LaTeX file. It is included, together with the revised source, PDF, and these notes, in `logarithmic_dlr_revision_package.zip`.
