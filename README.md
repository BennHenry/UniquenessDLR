# Uniqueness of DLR equations in the continuum

A collaborative study of uniqueness for the Dobrushin–Lanford–Ruelle (DLR) equations for point processes in the continuum, mainly in dimension 1.

Every result, method, or proof on this Git repository is completely free to use (under a very permissive license). If you want to take it, write your own article, and add to the noise, you are free to do so. However, we believe that the current capabilities of AI should push us toward a more collaborative, less ego-driven way of doing mathematics. We generally believe that there is no point in claiming for yourself results that are or can be easily AI-generated (more info in the manifesto). You are very welcome to join us.

It is still not very clear how we will work together, but there is a Discord server available for discussion.

https://discord.gg/fcsYGk7NT

The final aim is to build a coherent, checked, reader-friendly account of the mathematics: what is known, which arguments work, and which questions remain. The ultimate goal could be a future manuscript under a collective name, online videos, or anything that allows us to share this mathematics. All of this comes with the idea of rejecting ownership of results or proofs, as well as individual credit.

## History

* This project started with an attempt to produce a fully automated proof of uniqueness for the DLR equations of $\mathrm{Sine}_\beta$. The goal was to prove that this was possible. To avoid contamination from a recent preprint, the first attempt was produced without internet access for the model, allowing it to generate what we think is a very simple proof. Extensions were then produced for different models under different hypotheses.

## Promised results

Promised results are results claimed to be proved but that have not yet been checked or rewritten.

The notes associated with the claimed results are placed in Raw materials.

* For every $\beta>0$, the one-dimensional canonical logarithmic DLR equations have at most one stationary simple solution of intensity one satisfying $\int_1^\infty \text{Var}(N_{(0,t]})t^{-2},dt<\infty$ ([comparison theorem](Raw materials/Revised 2/logarithmic_dlr_uniqueness_simplified.tex)).

* Every stationary canonical logarithmic DLR solution with finite expected renormalized energy, under the draft's unit-background and truncation conventions, equals $\mathrm{Sine}_\beta$ ([finite-energy uniqueness](Raw materials/Revised 2/logarithmic_dlr_uniqueness_simplified.tex)).

* Finite expected renormalized logarithmic energy with unit background implies integrated number-variance control and hence sublinear number variance for any stationary simple point process ([energy-to-variance bound](Raw materials/Revised 2/logarithmic_dlr_uniqueness_simplified.tex)).

* Every canonical logarithmic DLR law is stationary if its sums of squared unit-interval counts grow at most linearly almost surely ([automatic stationarity](Raw materials/nonstationary_dlr_extension.tex)).

* The finite-energy identification with $\mathrm{Sine}_\beta$ extends to canonical logarithmic DLR laws without assuming stationarity, under the same energy conventions ([nonstationary uniqueness](Raw materials/nonstationary_dlr_extension.tex)).

* At $\beta=2$, a canonical logarithmic DLR law equals $\mathrm{Sine}_2$ if its ordered points satisfy $p_k/k\to1$ in both directions and its symmetric reciprocal sum converges ([conditional-universality consequence](Raw materials/nonstationary_dlr_extension.tex)).

* For smooth exponentially decaying perturbations of the logarithmic interaction that preserve the stated curvature bound, stationary simple unit-intensity canonical DLR solutions are unique under integrated number-variance control and the additional Palm crowding moment ([conditional extension](Raw materials/dlr_generalization_note.tex)).

* For every $\beta>0$ and $V(r)=-a_0\log r+W(r)$ with $a_0>0$, $W\in C^2([0,\infty))$ of finite range and $V''(r)>0$, there is at most one stationary simple unit-intensity canonical DLR solution satisfying linear and sublinear number-variance bounds, integrated number-variance control, and $\mathbb E_P N_{[0,1]}^3<\infty$ ([finite-range perturbations](Raw materials/dlr_generalizations.tex)).

* For every $s,\beta>0$, the one-dimensional Riesz interaction $V_s(r)=r^{-s}$ has at most one stationary simple unit-intensity solution to its relative-energy canonical DLR equations satisfying linear and sublinear number-variance bounds ([Riesz uniqueness](Raw materials/dlr_generalizations.tex)).

* For every $\beta,\rho>0$, the one-dimensional Coulomb interaction $g(x)=-|x|$ has exactly one translation-invariant solution of intensity $\rho$ to the stated symmetric Cesàro canonical particle DLR equations ([Coulomb uniqueness](Raw materials/coulomb_particle_dlr_uniqueness.tex)).

## Checked results

Results that have been verified and digested.

* We are currently looking at the proof of uniqueness for the DLR equations of $\mathrm{Sine}_\beta$ by Dereudre, Hardy, Leblé, and Maïda. Our goal is to understand it deeply and produce a complete rewriting.

## Disclaimer

By participating in this project, you withdraw any claim of ownership over the results that you provide. We believe that ownership of a proof or a mathematical result has become a nonsensical concept and, as such, should be rejected.

## Working principles

* Not clear at the moment. It will depend on the dynamics of the group.
