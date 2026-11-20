> **Public edition of evidence note WN-37.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `SS_KinkFermionGauge_ParentGate_v1.md`, a working note dated 9 November 2026. Not peer reviewed.
> - **Source content hash:** `72719436b2d9d0cde501e4aa37a716463a696ffdff64cc8713ece0ba97c8b82a` (16494 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** The scope of its √3κ gauge mode and 2κ threshold is limited to the specified action in [WN-41](WN-41_SS_Parent5D_Decision_v1.md) and [WN-42](WN-42_SS_5DParent_IntervalGate_v1r1.md), which find that they do not carry over to the covariant 5D parent. An editorial note marks the affected passage; the original wording is kept.

# SS kink–fermion–gauge parent: profile alignment and electromagnetic response

**Date:** 9 November 2026  
**Status:** Noncanonical working calculation; exact classical/algebraic results and a reproducible finite-deformation check. **Not** a canonical SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) replacement, a ghost-free independent-leaf gravity completion, or a quantum/radiative protection theorem.  
**Scope:** Independent, additive integration calculation for WS1 review. The independent-leaf parent, its full constraints and loop matching are not addressed here.  
**Evidence:** `SS_CoupledKinkFermionGauge_check_v1.py` (not included), `SS_CoupledKinkFermionGauge_results_v1.json` (not included). All quantities are in a fixed classical action and explicitly stated mode domains.

## 0. Decision

> **Editorial note (public edition, 19 November 2026):** Later notes find that the heavy gauge spectrum used here, an odd bound mode at √3κ and a continuum from 2κ, comes from the weighted gauge operator of the specified 4+1 action and does not carry over to the covariant 5D parent: there the transverse graviton and gauge spectra start at zero on the full line, and on a finite interval the positive gap is not 2κ and becomes small as the interval grows. Those notes treat this as a limit on scope: the results below hold for the specified action, but their gap should not be assigned to the covariant 5D bulk. See [WN-41](WN-41_SS_Parent5D_Decision_v1.md) §5 and [WN-42](WN-42_SS_5DParent_IntervalGate_v1r1.md) §5. The text below is unchanged from the working note.

**PASS (within one specified 4+1 effective action).** The kink's first-order equation is necessary and sufficient, within the monotone kink sector, for the normalized 4D light-fermion source density to equal the normalized light-photon and gravitational weight. The single action also predicts that an *internal odd shape excitation* changes the four-dimensional electromagnetic coupling and excites the previously protected heavy gauge sector, with a calculable leading weighted source norm. A pure *translation* of the kink preserves the exact alignment and the light gauge coupling.

**HOLD (full parent).** The present action deliberately uses one **four-dimensional Jordan metric** common to all transverse positions; it is not an independent-leaf or fully 5D covariant gravity construction. Its chosen `F(X)` gauge kinetic function and superpotential-tied Yukawa are explicit assumptions of this candidate, not consequences of the SS postulates. Full scalar constraints, heavy photon/fermion and localizer dynamics, radiative stability, far-tail strong coupling, and the independent-leaf physical stress amplitudes remain to be established. All first-order perturbations below are around a static kink with controlled worldvolume gradients; they do not imply an exact light-sector truncation for time-dependent shape fields.

## 1. One fully specified classical 4+1 effective action

Use a transverse real scale coordinate `y` on the whole line, a four-coordinate Jordan metric `g_{μν}(x)` independent of `y`, signature `(-+++)`, and fixed positive constants `M5,Z_X,r,kappa,v,e5`; `m>=0` is a 5D vectorlike interspecies mixing mass. Define

\[
w(X)=\kappa v(1-X^2/v^2),\quad F(X)=[1-X^2/v^2]^2,\quad
B[X]=\partial_yX-w(X),\quad H[X](x)=\int_{\mathbb R}F(X(x,y))\,dy.
\]

Retain a U(1) connection `A_M=(A_μ,A_y)` with `D_M=∇_M-i A_M`, and two five-dimensional Dirac fields `Ψ_+`, `Ψ_-` of equal vector U(1) charge. Their transverse mass functions are *opposite*, `+2κX/v` and `−2κX/v`; the two resulting opposite-chirality light modes form one vectorlike four-dimensional Dirac species. The action is

\[
\boxed{\begin{aligned}
S={}&\int d^4x\sqrt{-g}\,\bigg\{\frac{M_5^3}{2}H[X]R[g]
-\frac{Z_X}{2}\int dy\,[r\,g^{\mu\nu}\partial_\mu X\partial_\nu X+B[X]^2]\\
&\quad+\int dy\,\sum_{s=\pm}\bar\Psi_s\big(i\slashed D_4+\gamma^5D_y-s\,2\kappa X/v\big)\Psi_s
-m\int dy\,(\bar\Psi_+\Psi_-+\bar\Psi_-\Psi_+)\\
&\quad-\frac{1}{4e_5^2}\int dy\,F(X)\big[\mathcal F_{\mu\nu}\mathcal F^{\mu\nu}+2g^{\mu\nu}\mathcal F_{\mu y}\mathcal F_{\nu y}\big]\bigg\}.
\end{aligned}}
\tag{1}
\]

Hermitian symmetrization of the first-order fermion derivatives is understood; choose consistent gamma-matrix and normalizability conventions so the retained chiral transverse equation is `f' +2κX f/v=0`. The 4D spin connection is the one of `g`. The transverse metric in the matter terms is a fixed unit metric; no independent 5D lapse or spin-two tower is included. The BPS-square localizer part is anisotropic in the 4+1 split (its 4D coefficient is `r`), exactly as in the DYN-style common-metric localizer choice; no 5D Lorentz or supersymmetry claim is made.

The source-normalization comparison is performed on smooth, monotone kinks approaching `−v,+v`, with `H>0`, normalizable fermion zero modes and a positive gauge kinetic weight on finite `y`. The mass `m` is the same bare parameter for the two opposite transverse chiralities; it is a **model input**, not an SS prediction. All unlisted higher operators are set to zero at this tree matching order. This is an explicit model choice, not a uniqueness argument.

The vacuum `g=η`, `A=0`, `Ψ=0`, `X=X_0=v tanh(κy)` solves this action with `B=0`, `R=0`. The scalar localizer Hessian is

\[
\mathcal K=-\partial_y^2+4\kappa^2-6\kappa^2\operatorname{sech}^2(\kappa y).
\tag{2}
\]

Its normalized translation and odd shape eigenfunctions are

\[
\eta_0=\sqrt{3\kappa/4}\,\operatorname{sech}^2(\kappa y),\qquad
\eta_1=\sqrt{3\kappa/2}\,\tanh(\kappa y)\operatorname{sech}(\kappa y),
\]
\[
\mathcal K\eta_0=0,\quad \mathcal K\eta_1=3\kappa^2\eta_1,\quad
H_0=\int F(X_0)dy=4/(3\kappa).
\tag{3}
\]

The **bare transverse** eigenvalue `3κ²` is not the complete physical pole after mixing with the Jordan metric, nor is it the exact DYN v8 Q pole. In DYN's source parameters the localizer 4D kinetic term carries `r`; that distinction is retained below.

## 2. Exactly aligned light species, gauge source and metric source

The two 5D fermions have normalizable opposite-chirality zero modes with the **same** transverse amplitude

\[
f_0(y)=\sqrt{3\kappa/4}\,\operatorname{sech}^2(\kappa y),\quad
\rho_0(y)=|f_0|^2=F(X_0)/H_0.
\tag{4}
\]

The constant transverse Maxwell mode `v_0=H_0^{-1/2}` is normalizable under the weighted gauge norm `∫F v²dy`; its canonically normalized four-dimensional charge is `e_4=e_5/sqrt(H_0)`. The gauge Sturm–Liouville operator is `−F^(−1)∂_y(F∂_y)`, unitary to (2) on the kink, with the normalizable constant mode, the odd bound mode and a continuum threshold at `2κ`. The fermion transverse chiral operator factors into the same supersymmetric-QM pair; this algebraic factorization is *not* evidence of a fully supersymmetric gravitational/gauge theory.

For **zero-mode 4D stress** `T_{μν}` (on shell), the fermion contribution has transverse weight `ρ_0`, the photon contribution has `F/H_0`, and the gravitational Einstein weight is `F`. Therefore, at the reference kink, both the charged light current and the transverse distribution of the light stress align with the protected metric/gauge weight. In a complete heavy weighted mode basis `u_a`,

\[
g_a=e_5\int\rho_0u_a\,dy=e_5 H_0^{-1}\int F u_a\,dy=0\quad(a>0).
\tag{5}
\]

This is the *direct* linear heavy-photon current overlap, not a proof that all heavy-mediated loop/box effects vanish. The common 4D metric of (1) has no relative metric modes; for an independent-leaf extension the same `ρ_0=F/H_0` would provide the required tree source alignment, subject to full tensor constraints.

## 3. Necessary-and-sufficient BPS alignment theorem

For a fixed smooth static monotone background `X(y)` in the stated kink sector, the exact fermion zero mode obeys

\[
\partial_y\ln\rho_f=-4\kappa X/v,
\qquad \rho_f=|f_X|^2/\int|f_X|^2dy.
\]

Its normalized gauge/gravity weight is `h_X=F(X)/H[X]`. Direct differentiation gives the **exact local identity**

\[
\boxed{\partial_y\ln\frac{\rho_f}{h_X}
=\frac{4X}{v^2(1-X^2/v^2)}\,B[X].}
\tag{6}
\]

If `B[X]=0`, then `ρ_f/h_X` is constant; because both integrate to one, `ρ_f=h_X`. Conversely, if the normalized profiles agree and `X` is a nonconstant smooth monotone kink crossing zero only at isolated points, (6) forces `B[X]=0` wherever `X≠0` and thus everywhere by continuity. Hence

\[
\boxed{\rho_f(y)=F(X(y))/H[X]\ \text{for all }y
\quad\Longleftrightarrow\quad X'=\kappa v(1-X^2/v^2).}
\tag{7}
\]

This theorem requires the *specified* tied Yukawa `2κX/v` and gauge weight `F(X)`. It is not a theorem that all possible matter sources in nature share one scale profile. It provides a direct way to test whether an actual coupled parent retains protected alignment when its localizer is dynamical.

**Translation:** `X_Y(y)=v tanh[κ(y−Y)]` is another exact BPS solution, and both normalized profiles translate together. Its total gauge norm stays `H_Y=H_0`, so `e_4` is constant; all direct heavy overlaps vanish. This includes the translational zero-mode tangent. Fixed centre/fold conditions of canonical DYN may remove this collective degree of freedom, so its presence here must not be imported without checking those conditions.

## 4. Odd shape excitation: electromagnetic response and sourced heavy modes

At the undeformed kink take a small odd shape variation `X=X_0+q η_1+O(q²)`. Its first-order norm derivative is

\[
I_1=\left.\frac{dH}{dq}\right|_{0}
=\int F_X(X_0)\eta_1dy
=-\frac{\pi}{2v}\sqrt{\frac{3}{2\kappa}}\ne0.
\tag{8}
\]

Because the 4D charged zero modes remain normalized, the diagonal U(1) coupling is **exactly** `e_4(q)=e_5/sqrt[H(q)]` for a static shape background: its dependence on the zero-mode fermion profile cancels in the light-photon charge. Thus

\[
\boxed{\left.\frac{d\ln e_4}{dq}\right|_0
=-\frac{I_1}{2H_0}=\frac{3\pi}{16v}\sqrt{\frac{3\kappa}{2}},
\quad \left.\frac{d\ln\alpha_4}{dq}\right|_0=-\frac{I_1}{H_0}.}
\tag{9}
\]

This is a physical dimensionless gauge-strength change in the specified model, not removable by a 4D conformal frame transformation. By contrast the accepted DYN model has an *explicit* universal Jordan matter action with constant gauge coupling at the same classical order. The models agree at `q=0` but differ under the shape response.

The full Einstein-frame kinetic coefficient for **one retained odd profile** `q` is

\[
K_q=r Z_X+\frac{3M_5^3}{2H_0}I_1^2
=r Z_X+\frac{27\pi^2M_5^3}{64v^2},\qquad \varphi=\sqrt{K_q}\,q,
\tag{10}
\]

with bare one-mode quadratic mass `m_φ²=3κ² Z_X/K_q`. The physical finite-family scalar spectrum and pole residues require diagonalizing the *full* DYN scalar pencil; the single-profile mass is not substituted for those results. The normalized gauge response is `∂_φ ln e_4=−I_1/(2H_0 sqrt(K_q))`. For an explicit vectorlike interspecies mass `m` in (1), the 4D Einstein mass `m_E=m Φ^(−1/2)` responds as `∂_φ ln m_E=−I_1/(2H_0 sqrt(K_q))`. The ratio of scalar couplings is therefore `d ln e_4/d ln m_E=1` in the shape channel, versus zero for the gauge coupling in universal-Jordan DYN. These are ratios of tree response coefficients, not a physical equivalence-principle bound.

### Heavy gauge-mode leakage from the same deformation

For a static admissible shape background, the complete weighted photon eigenbasis gives an exact Parseval identity for the normalized light fermion source,

\[
\boxed{\mathcal R[X]\equiv\frac{\sum_{a>0}|g_a|^2}{|g_0|^2}
=H[X]\int\frac{\rho_f(y)^2}{F(X(y))}\,dy-1
=\int\frac{(\rho_f-F/H)^2}{F/H}\,dy\ge0.}
\tag{11}
\]

The integrals require `F>0` at finite `y` and `ρ_f²/F` integrable. At a BPS kink `R=0`. With `C=sqrt(3κ/2)` and `z=κy`, the linearized normalized profile mismatch is

\[
\left.\partial_q(\rho_f-F/H)\right|_0
=\frac{4C}{v}\frac{F_0}{H_0}
\left(\cosh z-\frac{3\pi}{8}\right).
\tag{12}
\]

The exact background moments are `E_0 cosh z=3π/8`, `E_0 cosh²z=3/2`, with `E_0` taken under `F_0/H_0`. Hence the **formal quadratic coefficient, validated along the admissible smooth completion below**, is

\[
\boxed{\mathcal R(q)=\frac{24\kappa}{v^2}
\left(\frac32-\frac{9\pi^2}{64}\right)q^2+o(q^2)
=2.6900851463234154\frac{\kappa}{v^2}q^2+o(q^2).}
\tag{13}
\]

The missing heavy-channel effect is thus second order in the squared source overlap, while the scalar dependence of the **diagonal light electromagnetic coupling is first order in `q`**. A Ward identity for diagonal U(1) charge does not cancel either the derivative of `e_4` with respect to a physical scalar or the higher-mode direct current for non-BPS profiles.

**Global-domain warning:** the naive finite ansatz `X=X_0+qη_1` for positive `q` crosses `|X|=v` in the tails. Its `F(X)` vanishes at a finite coordinate and its `ρ_f²/F` integral diverges; using (11) naively on that family is invalid. To verify the genuine linear response on a two-sided admissible family, choose the explicitly stated *nonlinear completion*

\[
X_q(y)=v\tanh\left[z+\frac{(q C/v)\sinh z}
{\sqrt{1+(q C/v)^2\sinh^2z}}\right],\qquad z=\kappa y,
\tag{14}
\]

which stays strictly inside `(-v,v)` at finite `y`, preserves both kink limits for either sign of `q`, and has tangent `∂_qX|_0=η_1`. It is a **test family**, not an exact excited nonlinear solution. Numerical integration of the exact zero-mode ODE and gauge norm for `κ=v=1`, on `y∈[−18,18]`, gives `R(q)/[2.690085 q²]` between `0.9887` and `1.0091` for `|q|≤0.012`, and the centered finite difference of `I_1` agrees within `1.5e−6` relative. Details and data are in the verifier outputs. This checks the perturbative coefficient and resolves the finite-branch singularity, but not a time-dependent 5D evolution or quantum amplitude.

## 5. Scientific compatibility with the programme

**Alignment vs responsiveness:** the *same* BPS relation explains why the fermion zero mode and light photon have the protected weight on the static parent, without assigning separate profile functions. It also shows why the dynamic odd mode does **not** stay within that aligned submanifold. Exact protection and nonzero shape-mediated response should not be conflated.

**U vs W:** This action is a physically specified W-like model with a derived chiral/vectorlike light mode rather than a merely imposed weight on an arbitrary four-dimensional material Lagrangian. Its fixed-background effective action reproduces the W conclusion `e_4∝Φ^(−1/2)`, while the *source alignment is derived from the BPS kink and tied Yukawa*. Universal-Jordan U retains the same gravitational `Φ` but **does not** have this additional gauge response. Thus source selection constrains the W completion but does not force it to become U.

**WS1 relation:** P24's observation that `F` is the kink gradient-energy profile is used, as is the idea of superpotential-tied fermions in Profile Selection. P19's independent-leaf fermion–Maxwell links and P21's loop thresholds are **different** parent candidates; no inheritance of their complete action, cutoff or gauge matching is claimed. P26/P28's coherent cubic–quintic matter and electrostatic droplets are also different matter actions. This document is an explicit **cross-branch comparator**, ready for WS1 review. The programme's related work is moving into MAT-DYN.

**Unresolved hard gates:** Determine the full physical metric–localizer poles and projectors, complete massive-photon currents and 4D stress matrix elements, one-loop gauge/fermion thresholds and any 5D boundary regulator; check far-tail strong gauge coupling where `F→0`; test whether the 4D metric's independent-of-y ansatz consistently emerges from a constraint-complete independent-leaf or 5D parent. The localizer is real; complex fermion/gauge fields give phase and charge but do not identify ordinary object size with intrinsic scale coordinate. The reference SS-GEO [v6, doi:10.5281/zenodo.23603029](https://doi.org/10.5281/zenodo.23603029) physical-coordinate map remains a separate identification problem.

## 6. Primary programme sources consulted

- `SS-DYN_leafwise_dynamical_closure_v8.tex` (LaTeX source of SS-DYN v8; not included) — live canonical common-Jordan action, restricted finite family, localizer pencil, and fixed protected-weight parent comparison.
- [WN-04](WN-04_P2Parent.md), [WN-08](WN-08_P18RegulatedLoop.md), [WN-27](WN-27_P19DiracMaxwellParent.md), [WN-26](WN-26_P24ScaleKinkWeight.md), [WN-32](WN-32_P26ChargeExtentOnKink.md), [WN-34](WN-34_P28ChargedDropletKinkSize.md), a coordination note (not included) — working, noncanonical results/coordination.
- [WN-40](WN-40_SS_ProfileSelection_Decision_v1.md), [WN-09](WN-09_SS_ParentMatter_DiracMatching_v1.md), [WN-11](WN-11_SS_ParentMatter_FiniteSpectrum_v1.md), [WN-35](WN-35_SS_SingleActionReduction_v1.md), [WN-36](WN-36_SS_TwoReductionComparison_v1.md) — recent working gates.

A November archive of related P29 parent-protection material (not included) could not be read when this note was written; it was therefore **not audited or treated as an authority**. The present result is independently stated with its own action and explicit assumptions.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN", "DYN v8" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-GEO v6** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-GEO: Logarithmic Scale as a Geometric Coordinate: Exact-Distance Projection and Radial Scale Response* (version 6). Zenodo. [doi:10.5281/zenodo.23603029](https://doi.org/10.5281/zenodo.23603029). Published; current version.

Other working notes referred to by label:

- P19: [WN-27](WN-27_P19DiracMaxwellParent.md)
- P21: [WN-25](WN-25_P21MatterIntoGravity.md)
- P24: [WN-26](WN-26_P24ScaleKinkWeight.md)
- P26: [WN-32](WN-32_P26ChargeExtentOnKink.md)

Material named in this note but not included in this release: `SS-DYN_leafwise_dynamical_closure_v8.tex`, `SS_CoupledKinkFermionGauge_check_v1.py`, `SS_CoupledKinkFermionGauge_results_v1.json`.
