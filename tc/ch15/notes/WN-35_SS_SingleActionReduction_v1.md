> **Public edition of evidence note WN-35.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `SS_SingleActionReduction_v1.md`, a working note dated 9 November 2026. Not peer reviewed.
> - **Source content hash:** `4f30dc0d9503f21c09bacd1c3a8c12604060421add8f8d8c33f2dc6d94ab643e` (15955 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# Single-action metric–localizer–material reduction: explicit odd-mode coupling and its universality gate

**Programme:** Scale Space / SSC — working scientific note  
**Date:** 9 November 2026  
**Authority:** noncanonical, unregistered research candidate; **not** a modification or derivation of the adopted SS-DYN v8 [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) action  
**Files:** [WN-35](WN-35_SS_SingleActionReduction_v1.md), `SS_SingleActionReduction_v1.tex` (not included), `SS_SingleActionReduction_check_v1.py` (not included)  
**Decision:** A definite classical common-parent-to-localizer/material interaction is derivable from one *explicitly added* common-metric action, with an exact, nonzero odd-mode overlap and no independently selected cross-level coupling. However, the same action introduces a nonmetric gauge-kinetic scale dependence; its equivalence to the accepted universal-Jordan matter coupling and the independent-leaf parent remains **HOLD**.

## 1. Source ownership and the distinction that matters

The live canonical `SS-DYN_leafwise_dynamical_closure_v8.tex` (LaTeX source of SS-DYN v8; not included) specifies a **restricted** common-metric family, with one universal Jordan matter metric and protected background parent weights. It explicitly warns that replacing those fixed weights by dynamical `F(X)` changes the model and its scalar charge. The live WS1 [WN-26](WN-26_P24ScaleKinkWeight.md) proposes relating the weight `sech^4` to the kink's BPS flow; [WN-32](WN-32_P26ChargeExtentOnKink.md) and [WN-34](WN-34_P28ChargedDropletKinkSize.md) independently model a material weight on that kink, with stated electromagnetic-weight choices. [WN-11](WN-11_SS_ParentMatter_FiniteSpectrum_v1.md), [WN-09](WN-09_SS_ParentMatter_DiracMatching_v1.md), and `SS_CrossSourceParent_Gate_v1.md` (not included) (the latter is a prior *local* result) motivate the shared-source/metric requirements. Their respective proofs, statuses and limitations remain separate.

The present exercise deliberately proposes and analyzes a **different restricted common-metric model member** to discover what a single-action coupling does. It **does not** modify a canonical action, choose a ghost-free independent-metric parent, prove that the SS postulates select this action, establish light-mode fermion quantum matching, or assert that this coupling is an empirically distinctive SS prediction.

## 2. One specified action

Let `y` be a proper scale coordinate and `x^μ` four clock-reading coordinates. On the declared common-metric ansatz, take a Lorentzian metric `g_{μν}(x)`, a real scale localizer `X(x,y)`, a four-coordinate matter multiplet `ψ_A(x)` for each sector A, and a common four-coordinate U(1) gauge potential `A_μ(x)`. Matter fields and this gauge potential are **restricted to their uniform scale profiles by the definition of this model member**; this is not a proof they dynamically truncate an independent-leaf theory. The action is

\[
\begin{split}
S[g,X,\psi_A,A]=\int d^4x\sqrt{-g}\int_{-\infty}^{\infty}dy\,\Big\{&
\frac{M_5^3}{2}F(X)R[g]
-\frac{Z_X}{2}g^{\mu\nu}\partial_\mu X\partial_\nu X \\
&-\frac{Z_X}{2}\big[\partial_y X-\kappa v(1-X^2/v^2)\big]^2
+F(X)\,\mathcal L_4(g,\psi_A,A)\Big\},\qquad
F(X)&=(1-X^2/v^2)^2.
\end{split}\tag{1}
\]

Here `M_5^3,Z_X,κ,v>0`, and `ℒ_4` is one *specified* ordinary four-dimensional gauge-invariant matter Lagrangian, for example

\[
\mathcal L_4=-\frac{1}{4g_5^2}F_{\mu\nu}F^{\mu\nu}
+\sum_A\overline\psi_A(i\gamma_g^\mu(\nabla_\mu-i q_A A_\mu)-m_A)\psi_A
+\mathcal L_{\rm int}.
\tag{2}
\]

The symbol `g_5` is a bare gauge normalization, not an extra-dimensional experimental charge, and `q_A` are representation charges. The classical analysis below needs only that `ℒ_4` be smooth in its fields and independent of y before reduction. The use of **one dynamical `F(X)` on gravitational and every matter term** is a substantive extra assumption, not implied by the accepted SS-DYN action. The BPS square and factor `F` resemble WS1 P24, but the combined action (1) has not been certified by WS1. Boundary terms, finite localizer energy, regularity, a physical regulator and the usual four-dimensional constraints are assumed. The graviton has only a common metric here; its ghost freedom does not settle the independent-leaf parent.

### The background and its exact zero-sector normalization

At `R=0`, vacuum-normalized `ℒ_4=0`, and flat `g`, the kink

\[
X_0(y)=v\tanh(\kappa y),\quad F_0(y)=\operatorname{sech}^4(\kappa y),\quad
W_0=\int dy F_0=\frac4{3\kappa}
\tag{3}
\]

sets the BPS square to zero. Restricting `X=X_0` yields the exact classical zero-sector action

\[
S_0=\int d^4x\sqrt{-g}\,W_0
\left[\frac{M_5^3}{2}R[g]+\mathcal L_4(g,\psi_A,A)\right],
\quad M_4^2=M_5^3 W_0.
\tag{4}
\]

For a gauge term `-W_0 F²/(4g_5²)`, canonical normalization gives `g_4²=g_5²/W_0`. An overall matter factor `W_0` must also be canonically normalized (including fermions) before interpreting physical mass/charge. Equation (4) is a **consistent member of the explicitly restricted action (1)**, not a result proving that an independent-leaf nonlinear action has only this low-energy mode.

## 3. Exact localizer spectral reduction

Perturb `X=X_0+η` around the flat, source-free background. The BPS square yields the second variation

\[
\frac{Z_X}{2}\int dy\,\eta\,\mathcal H_X\eta,\qquad
\mathcal H_X=-\partial_y^2+\kappa^2[4-6\operatorname{sech}^2(\kappa y)],
\tag{5}
\]

with a normalizable even translational zero mode and a normalizable odd mode:

\[
\chi_0(y)=\sqrt{\frac{3\kappa}{4}}\operatorname{sech}^2(\kappa y),\quad
\mathcal H_X\chi_0=0,
\]
\[
\chi_1(y)=\sqrt{\frac{3\kappa}{2}}\operatorname{sech}(\kappa y)\tanh(\kappa y),\quad
\mathcal H_X\chi_1=3\kappa^2\chi_1,
\quad\int\chi_a\chi_bdy=\delta_{ab}.
\tag{6}
\]

The continuum starts at `4κ²`; truncating to `χ_1` is a **single-mode exchange calculation**, not an exact replacement of the full field for arbitrary sources. A centre-pinning prescription or collective-coordinate treatment is required for the translational zero mode; the odd source below has no linear projection on it.

The scalar source generated *by varying the same action* is

\[
\mathcal J(x,y)=F_X(X_0(y))\,\mathcal B(x),\qquad
\mathcal B(x)=\frac{M_5^3}{2}R[g](x)+\mathcal L_4(x),
\]
\[
F_X(X_0)=-\frac4v\tanh(\kappa y)\operatorname{sech}^2(\kappa y).
\tag{7}
\]

This is an **action derivative**, not a postulated independent interaction. For `η(x,y)=q_1(x)χ_1(y)/√Z_X`, the exact linear overlap is

\[
\mathcal I_0=\int F_X(X_0)\chi_0\,dy=0,
\]
\[
\boxed{\mathcal I_1=\int F_X(X_0)\chi_1\,dy
=-\frac{\pi}{2v}\sqrt{\frac{3}{2\kappa}}\ne0.}
\tag{8}
\]

The first vanishes by parity. The second follows directly by substituting `t=tanh(κy)` and evaluating `∫_{-1}^1 t²√(1-t²)dt=π/8`. Thus a uniform-in-y material sector generically excites an **odd internal scale localizer mode**, even when its *direct bare metric source* follows the background protected `F_0` weights. This does not imply a physical relative-metric force in the accepted constrained theory: the current model has a single metric, while any independent-leaf completion must determine the effect of localizer-to-metric mixing and Ward constraints separately.

The effective canonical coupling and localizer squared mass are

\[
g_1=\frac{\mathcal I_1}{\sqrt{Z_X}},\qquad m_1^2=3\kappa^2,
\qquad
\boxed{\frac{g_1^2}{m_1^2}=
\frac{\pi^2}{8Z_X\kappa^3v^2}.}
\tag{9}
\]

Here `m_1` is the localizer-mode mass *in the action's declared four-dimensional clock-reading normalization*, not a measured particle mass. In a fixed-background Euclidean low-momentum treatment of the quadratic localizer field, eliminating `q_1` yields

\[
\boxed{\Delta S_{E,1}=-\frac12\int\frac{d^4p}{(2\pi)^4}
\frac{g_1^2}{p_E^2+3\kappa^2}\,
\mathcal B(-p_E)\mathcal B(p_E).}
\tag{10}
\]

For `ℒ_4=Σ_A ℒ_A`, the cross term between A and B is fixed by the same `g_1²` and pole. It cannot be chosen independently at the molecular, biological or bulk level within this action. **But** (10) is a *bare fixed-metric Schur complement*: its `Rℒ`, `R²` and `ℒ²` pieces must be interpreted only after gravitational constraints, field redefinitions and full EFT matching. The continuous localizer modes also contribute; (10) is not a claim of the complete propagator or a new observed force.

## 4. The important counter-result: universal stress is not the same as a universal metric-only matter action

Because the same dynamical `F(X)` multiplies the Maxwell term, its four-dimensional effective gauge coefficient is `W(q_1)/g_5²`, where

\[
W(q_1)=W_0+g_1q_1+O(q_1^2),\qquad
\frac1{g_4^2(q_1)}=\frac{W(q_1)}{g_5^2}.
\]

Consequently

\[
\boxed{\left.\frac{\partial\ln g_4}{\partial q_1}\right|_0
=-\frac{g_1}{2W_0}
=\frac{3\sqrt6\pi\sqrt\kappa}{32\sqrt{Z_X}v}\ne0.}
\tag{11}
\]

An overall conformal change of a four-dimensional metric **does not** produce this coefficient: `√-g F_{μν}F^{μν}` is conformally invariant in four dimensions. Thus a change of gauge coupling from (11) cannot be represented merely by changing the universal conformal Jordan metric. The single-action construction has generated a physical-looking gauge-kinetic *dilaton-type operator*, not established purely metric universality. To make the action compatible with SS-DYN's accepted matter coupling, one must either (a) protect/fix the matter gauge normalization independently of dynamical `W` while deriving a different localizer–matter interaction, or (b) explicitly adopt and test a theory with varying gauge normalization and its associated constraints and radiative effects. Option (a) sacrifices the naive universality of one `F(X)` factor across all terms; option (b) requires additional physical authorization and cannot be silently relabelled SS-DYN.

**On-shell matter caution.** Terms proportional to a classical Dirac equation can be moved by field redefinitions and must not be counted as physical scattering couplings. The gauge-kinetic variation is a robust diagnostic at the action level, but converting it into a measurable amplitude still requires canonical normalization, conserved-current matrix elements, loop matching and the appropriate background. In particular `F²=0` for a single free plane electromagnetic wave; this does not remove the operator for all superpositions or scattering configurations.

### Scalar–gravity kinetic mixing also changes the naive exchange

The nonminimal scalar coefficient is `M_5³ W(q_1)R/2`. A conformal transformation to a fixed Einstein-frame Planck coefficient produces a positive kinetic correction

\[
\boxed{\Delta Z_E=\frac32 M_4^2\left(\frac{g_1}{W_0}\right)^2
=\frac{27\pi^2 M_5^3}{64 Z_Xv^2}.}
\tag{12}
\]

This is computed **at the zero background**, with `q_1` initially normalized by `Z_X`; it arises from the standard conformal transformation of the curvature term. Hence (10)'s `m_1²=3κ²` and its exchange coefficient are **not yet the physical Einstein-frame scalar pole/residue**. One must canonicalize the mixed scalar and metric system and include all other localizer modes before claiming such a pole. This explicit correction sharpens the earlier cross-source graph note: even the seemingly protected common metric can have nontrivial scalar mixing in an actual covariant parent.

## 5. What has and has not been unified

| Required link | Status under (1) | Reason |
|---|---|---|
| Kink geometry to protected weight | **Derived within chosen BPS/weight ansatz** | `F_0=sech⁴`, `W_0=4/(3κ)`; selecting `F(X)` itself remains an assumption |
| Weight and localizer dynamics to a matter source | **PASS (conditional)** | Exact variation (7) and nonzero overlap (8) |
| Same source to a fixed cross-sector mediator | **PASS (bare restricted model)** | One `g_1` and `m_1` give (10), no per-sector coupling fit |
| Protected four-dimensional gravitational zero mode | **PASS at fixed background in the restricted action** | Common metric imposed, `M_4²=M_5³W_0`; not a leafwise-parent theorem |
| Purely universal metric matter coupling after dynamics | **HOLD / obstruction for the naive full `F(X)` weighting** | Gauge-kinetic variation (11), scalar–metric mixing (12) |
| Nonlinear independent-leaf parent and full constraints | **OPEN** | Not constructed or validated here |
| Quantum QED/neutral composites from this parent | **OPEN** | P19 heavy thresholds, fermion/gauge mixing, loops and hard annihilation matching required |
| Ordinary object size ↔ intrinsic `y`/`u` | **OPEN** | A composite Born pushforward is not a physical extra coordinate |
| Biological response/pattern thresholds | **OPEN** | No common-source state preparation or calibrated measurement map derived |

The central physical result is a **tradeoff rather than a completed unification**: promoting the scale weight to a dynamical common factor is sufficient to generate a linked scale-mediated interaction, but it also generates nonmetric material effects. This is the exact kind of structural choice a parent theory must resolve before connecting independent disciplines.

## 6. Next decisive PC-2 gate

A proper upgrade should **not** fit more interaction coefficients. It should compare two complete, constraint-consistent actions against one common matching target:

1. **Candidate U (universal Jordan matter):** retain SS-DYN v8's `S_m[g_J,ψ]`, fixed background parent weights, and vary localizer/metric variables in its adopted finite multiplet. Derive the physical scalar-to-complete-stress matrix and eliminate the constrained modes. Record if any of the intrinsic odd channel in (8) survives through the *actual* Jordan map.
2. **Candidate W (dynamically weighted matter):** take the explicit extension (1), calculate its Einstein-frame canonical kinetic terms and independently normalized gauge/Dirac operators, then match physical on-shell source amplitudes in a regulated finite member. Determine whether its new gauge-kinetic source can satisfy existing constraints or requires new physics.
3. **Compare** the same invariant amplitude matrix, pole locations and residue signs for complete conserved sources. A cross-level interaction is a parent consequence only if the observed effective laws inherit a shared matched pole/residue and use one derived intrinsic-scale readout. Separate ordinary size labels do not qualify.

**Pass gate:** one model produces (i) an accepted protected physical metric, (ii) an independently justified physical scale mediator and its complete source functional, (iii) self-consistent gauge/Dirac matching, and (iv) a bound on discarded-mode and radiative errors in the energy domain relevant to the intended observables. **Hold:** any requirement is enforced by a new fitted coefficient, a change of matter normalization not accounted for, or an unverified identification of ordinary size with `u`.

**Scope:** The actual independent-leaf parent and its inhomogeneous constraints remain in WS1. This analysis is downstream, restricted, noncanonical and additive. It is not a basis for changes to WS1, SS-DYN, SS-MAT [v1, doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555), SS-MULTI [v2, doi:10.5281/zenodo.23873325](https://doi.org/10.5281/zenodo.23873325), BIO or MEAS.

## 7. Reproducibility and limitations

Run `python SS_SingleActionReduction_check_v1.py` (not included) with SymPy. It checks the kink integral, normalized localizer modes and eigenvalues, exact odd/even overlaps, single-mode Schur coefficient, gauge variation and Einstein-frame kinetic correction; it prints symbolic expressions. The independently verified result here is **symbolic algebra and direct variational reasoning**, not a rerun of independent-leaf numerical dynamics, a global field-theory constraint analysis or an external peer review. No new physical parameter values, experimental data, new reference-corpus works or measured SS effects are claimed.

---

## References and related notes (public edition)

Published works cited:

- **SS-BIO v4** (written "BIO" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-BIO: Scale-Extended Biological Dynamics in Scale Space: Configurational Structure, Transport, and Reaction–Diffusion Tests* (version 4). Zenodo. [doi:10.5281/zenodo.23874087](https://doi.org/10.5281/zenodo.23874087). Published; current version.
- **SS-DYN v8**: D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-MAT v1** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MAT: Scale-Extended Matter Sources: Protected Matching, Scale Transport and Completion Gates* (version 1). Zenodo. [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555). Published; current version.
- **SS-MEAS v2** (written "MEAS" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MEAS: Measurement Projection and Identifiability in Scale Space: Calibrated Observables, Null Spaces, and Withheld-Probe Tests* (version 2). Zenodo. [doi:10.5281/zenodo.23865651](https://doi.org/10.5281/zenodo.23865651). Published; current version.
- **SS-MULTI v2** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MULTI: Physical Scale as a Location Coordinate: A Multi-Scale Framework in Scale Space* (version 2). Zenodo. [doi:10.5281/zenodo.23873325](https://doi.org/10.5281/zenodo.23873325). Published; current version.

Other working notes referred to by label:

- P19: [WN-27](WN-27_P19DiracMaxwellParent.md)
- P24: [WN-26](WN-26_P24ScaleKinkWeight.md)

Material named in this note but not included in this release: `SS-DYN_leafwise_dynamical_closure_v8.tex`, `SS_CrossSourceParent_Gate_v1.md`, `SS_SingleActionReduction_check_v1.py`, `SS_SingleActionReduction_v1.tex`.
