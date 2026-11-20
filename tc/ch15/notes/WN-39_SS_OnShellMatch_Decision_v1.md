> **Public edition of evidence note WN-39.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `SS_OnShellMatch_Decision_v1.md`, a working note dated 9 November 2026. Not peer reviewed.
> - **Source content hash:** `1c055a996a104abed94237aad149c08f168354e55774cb3143bc503030bda07d` (15147 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** The scope of its √3κ gauge mode and 2κ threshold is limited to the specified action in [WN-41](WN-41_SS_Parent5D_Decision_v1.md) and [WN-42](WN-42_SS_5DParent_IntervalGate_v1r1.md), which find that they do not carry over to the covariant 5D parent. An editorial note marks the affected passage; the original wording is kept.

# MAT–DYN on-shell matched fermion amplitude and the protected-kink stopping gate

**Date:** 9 November 2026. **Status:** noncanonical research and conditional stopping decision; no canonical adoption. **Author:** Donald G. Palmer Scale Space programme, AI-assisted calculation. **Evidence:** `SS_OnShellMatch_check_v1.py` (not included), `SS_OnShellMatch_results_v1.json` (not included), `SS_OnShellMatch_output_v1.txt` (not included). These checks are independent numerical spinor tests and a new Galerkin matching calculation; they are not quantum-loop calculations or an external physics review.

## Decision

> **Editorial note (public edition, 19 November 2026):** Later notes find that the heavy gauge spectrum used here, an odd bound mode at √3κ and a continuum from 2κ, comes from the weighted gauge operator of the specified 4+1 action and does not carry over to the covariant 5D parent: there the transverse graviton and gauge spectra start at zero on the full line, and on a finite interval the positive gap is not 2κ and becomes small as the interval grows. Those notes treat this as a limit on scope: the results below hold for the specified action, but their gap should not be assigned to the covariant 5D bulk. See [WN-41](WN-41_SS_Parent5D_Decision_v1.md) §5 and [WN-42](WN-42_SS_5DParent_IntervalGate_v1r1.md) §5. The text below is unchanged from the working note.

**PASS at a controlled tree-level gate:** using the *same external on-shell light Dirac states*, the electromagnetic current and symmetric energy–momentum tensor satisfy the Ward identities, and the scalar trace reduces exactly to the on-shell fermion mass bilinear. Combining these sources with the finite SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) metric-mixed scalar modes and the even heavy-photon modes yields a definite tree-level on-shell *two-fermion scattering kernel*. In the exact BPS, zero-field vacuum, direct heavy-photon exchange between two light fermion currents is identically absent. The standard photon, common graviton and SS-DYN scalar modes remain. The first new heavy-photon effect from a dynamically excited localizer requires two insertions of the localizer field; it is a positive semidefinite **two-current–two-scalar** response kernel rather than a new vacuum four-fermion force.

**HOLD, and stop the present unification branch at this precise boundary:** a regulator-matched one-loop on-shell four-fermion amplitude, complete constraint-solved independent-leaf tensor sector and physical SS scale-to-matter map are not supplied by the existing common-metric candidate. Their coefficients cannot be inferred from the source-overlap theorem, the diagonal Ward identity or the finite-mode Galerkin numbers. Further parameter scans of the same tree action will not resolve this. The parent action and loop matching are outside this note. The present result is useful as a rigorous reference point, not a completed physical parent.

## 1. Precisely specified source action, frame and state

Use the previously filed [WN-37](WN-37_SS_KinkFermionGauge_ParentGate_v1.md) action (one four-dimensional Jordan metric, localizer X, two opposite-chirality five-dimensional Dirac copies, same photon, Yukawa linked to the BPS function, gauge kinetic weight F(X)). On its reference solution,

\[
X_0=v\tanh(\kappa y),\quad F_0=\operatorname{sech}^4(\kappa y),\quad
H_0=\int F_0dy=4/(3\kappa),\quad e_4=e_5/\sqrt{H_0},\quad
\rho_0(y)=F_0/H_0.
\]

The paired chiral light modes give a four-dimensional vectorlike Dirac field with a **model-input** mass m. At a fixed static kink, the normalized fermion zero mode has unit integral, so after Einstein-frame normalization its mass is \(m_E=m\Phi^{-1/2}\), while the physical low-energy vector coupling is \(e_4=e_5/\sqrt{H[X]}\). These are matching statements conditional on the model's spectrum and unbroken diagonal U(1); fermion wavefunction dressing and quantum thresholds are uncomputed. The accepted canonical SS-DYN v8 restricted action instead has its own universal Jordan-metric matter term and is not modified.

## 2. The explicit on-shell gauge and gravitational source test

Take one incoming/outgoing pair of positive-energy on-shell Dirac spinors, \(p^2=p'^2=m^2\), \(q=p'-p\), \(P=p'+p\). With the mostly-minus Dirac convention define

\[
J^\mu=\bar u(p')\gamma^\mu u(p),\quad S=\bar u(p')u(p),\quad
T^{\mu\nu}=\tfrac14\left(J^\mu P^\nu+J^\nu P^\mu\right).
\]

The free Dirac equation and \(q\cdot P=0\) give the **exact identities**

\[
q_\mu J^\mu=0,\qquad q_\mu T^{\mu\nu}=0,\qquad
T^\mu{}_{\mu}=mS.
\tag{1}
\]

These use complete Belinfante *free/light-sector* stress matrix elements; gravity or gauge radiative form factors would require further matching. The supplied independent implementation uses explicit 4x4 gamma matrices, eight helicity/spin configurations, two nontrivial elastic kinematics, and verifies all three identities to floating precision. A Feynman-rule scalar Yukawa vertex \(m b_a S\) cannot in general be replaced by a universal multiple of \(J^\mu J_\mu\) at arbitrary spin and momentum; the on-shell trace identity provides the correct source dictionary.

A localizer-dependent gauge kinetic function yields the 2-photon vertex \(V^{\mu\nu}=(k\cdot k')\eta^{\mu\nu}-k'^\mu k^\nu\) (up to overall coupling/sign). It obeys \(k_\mu V^{\mu\nu}=V^{\mu\nu}k'_\nu=0\), checked explicitly. With no background photon field this vertex has two photon legs and **does not add a linear scalar pole to the vacuum quadratic vector-current propagator**.

## 3. Tree-level physical 2-to-2 amplitude in the protected vacuum

For two distinguishable external light fermions, with separately conserved current and stress, the physical tree-level **t-channel** amplitude contains the following independent source structures (overall signs, \(i\) factors and spinor exchange diagrams suppressed):

\[
\mathcal M^{(t)}_{\rm tree}(q_E)=
\underbrace{\frac{e_{4,1}e_{4,2}\,J_1\!\cdot J_2}{q_E^2}}_{\mathrm{massless\ photon}}+
\underbrace{\frac{m_1m_2}{2M_4^2}\sum_{a=1}^{N}\frac{\alpha_a S_1 S_2}{q_E^2+m_a^2}}_{\mathrm{metric\!\text{–}mixed\ scalar}}+
\underbrace{\mathcal M_{\rm graviton}[T_1,T_2;q_E]}_{\mathrm{massless\ tensor}}.
\tag{2}
\]

The massless tensor term is fixed by conserved on-shell stress and the usual projector, proportional to \((T_1^{\mu\nu}T_{2\mu\nu}-\tfrac12T_1T_2)/(M_4^2q_E^2)\); its exact overall convention depends on the graviton field normalization. For identical fermions the crossed u-channel term and antisymmetrization must also be included. For annihilating particle–antiparticle states there are additional physical s-channel diagrams. Equation (2) is the general source-factorized t-channel structure, not a full cross section.

The scalar couplings obey \(b_a=\partial_{\varphi_a}\ln m_E\), \(\alpha_a=2M_4^2b_a^2\) for this fixed universal matter mass. The \(\alpha_a\) values come from the physical generalized scalar eigenproblem in SS-DYN v8, including the rank-one metric kinetic term:

\[
Kv_a=\mu_a Gv_a,\quad G=rI+\frac9{8\zeta_X}ff^{\mathsf T},\quad
\alpha_a=\frac3{8\zeta_X}(f^{\mathsf T}v_a)^2.
\]

For the live benchmark \(r=10^{-6},\zeta_X=181150,L=12\), N=72 reproduces \(m_Q/\kappa=340.9360090\), \(\alpha_Q=0.320824640\). Other finite scalar couplings total approximately 0.000386326. The lowest pole is much heavier than the photon continuum threshold \(2\kappa\), which does **not** imply an observable long-range heavy-photon force, because the direct heavy-current overlap vanishes.

In the nonrelativistic spin-averaged/static limit, the form of the potential is the conventional Coulomb term plus the universal Newton term with scalar Yukawa correction,

\[
V_{\rm NR}(R)=\frac{Q_1Q_2\alpha_{\rm em}}R
-\frac{G_Nm_1m_2}{R}\left[1+\sum_a\alpha_a e^{-m_aR}\right],
\tag{3}
\]

within the indicated approximation and ignoring corrections to gravitational and electromagnetic source matching. This Yukawa structure was already part of SS-DYN; deriving it from the specified light Dirac on-shell states is a matching check, not a new empirical prediction.

**Exact absence result:** \(\rho_0=F_0/H_0\) and photon orthogonality \(\int F_0 u_nu_0=0\) imply \(g_{n>0}^{JJ}=e_5\int\rho_0u_n=0\), without any mode truncation. Thus the gauge tower supplies no additional vacuum t-channel pole at order \(J_1J_2\) in this action. A statement that a gauge continuum at \(2\kappa\) automatically modifies ordinary Coulomb exchange would be incorrect here.

## 4. The first new heavy-photon operator when the localizer fluctuates

For a small dynamically varying odd localizer fluctuation \(\delta x(y,z)=\sum_j a_j(z)e_j(y)\) (fixed-centre DYN sine modes), write \(e_j=L^{-1/2}\sin(j\pi y/L)\) inside the box. The log derivative of the normalized light fermion density follows from the same Yukawa equation:

\[
A_j(y)=\int_0^y e_j(s)ds=\frac{1-\cos(j\pi y/L)}{(j\pi/L)\sqrt L},\quad
f_j^{F}=\frac{F_X(X_0)}{F_0}v e_j=-4\frac{\tanh y}{\operatorname{sech}^2 y}e_j,
\]
\[
d_j(y)=\partial_{a_j}(\rho-F/H)|_0=\rho_0(y)
\left[-4(A_j-\langle A_j\rangle_0)
-(f_j^{F}-\langle f_j^{F}\rangle_0)\right].
\tag{4}
\]

Scale lengths are in \(\kappa=1\) units in (4). Let \(U_n(y)\) be canonically weighted even heavy photon eigenmodes and \(V_{ja}\) the **metric-mixed** scalar generalized eigenvectors (\(V^{\mathsf T}GV=I\)). Define

\[
C_{na}=\sqrt{H_0}\sum_j V_{ja}\int d_j(y)U_n(y)dy,
\quad n>0.
\]

The source-space heavy-photon exchange matrix is

\[
\boxed{\mathcal H_{ab}(p_E)=\sum_{n>0}\frac{C_{na}C_{nb}}{p_E^2+\mu_{\gamma,n}^2}\succeq0.}
\tag{5}
\]

It is positive semidefinite for Euclidean momentum. Crucially, it enters the effective action **quadratically in the localizer amplitudes**; the gauge-heavy/light-fermion vertex is \(\propto a_j J\), not a finite constant at the BPS vacuum. Once the localizer is canonically normalized, the operator at wavelengths longer than the heavy photon scales takes the schematic form

\[
\boxed{\Delta\mathcal L_{\rm EFT}\sim\frac{e_4^2}{2\mathcal S_c^2}
J_{T\mu}J_T^\mu\sum_{ab}\varphi_a\varphi_b\mathcal H_{ab}(0),\quad
\mathcal S_c^2=Z_Xv^2/\kappa,}
\tag{6}
\]

with momentum convolution and convention-dependent Lorentzian signs suppressed. Here \(a_j=\sum_aV_{ja}\varphi_a/\mathcal S_c\). For space-varying fluctuations (6) must be understood as a nonlocal bilinear before the low-gradient expansion, not as a universal constant scattering amplitude. Integrating out the dynamical localizer at tree level does not turn (6) into a pure four-fermion contact; vacuum four-fermion matching requires actual loop/threshold calculation.

The **standard bare odd shape** \(\eta_1\propto\tanh y\operatorname{sech}y\) has \(\mathcal H_{\eta_1\eta_1}(0)=0.61526842\) at unit spatial norm. The actual **physical lowest metric-mixed scalar profile**, rescaled to unit L2 norm, gives

\[
\boxed{\mathcal H_{QQ}^{\mathrm{L2norm}=1}(0)=0.30036044074.}
\tag{7}
\]

This new physical-profile result is stable under N=24, 48, 72 scalar truncations and 48, 80, 112 even gauge modes; N=72 and N=48 agree to 11 digits. In the particular dimensionless convention \(\kappa=v=M_5^3=1\) (hence \(Z_X=\zeta_X\)), using the **G-normalized** lowest scalar eigenvector gives \(\mathcal H_{QQ}(0)/\mathcal S_c^2=0.0622210885\), so the coefficient of \(e_4^2\varphi_Q^2J_T^2\) in (6) is \(0.0311105443\). This coefficient is **not** a dimensional physical prediction; \(M_5,\kappa,v\), the normalization of the actual current and the background all remain model inputs.

The two independent spatial-profile coefficients differ because Einstein-metric mixing changes the Q eigenfunction; the heavy gauge source mismatch functional is a different projection from the universal stress source. This is a real joint consequence of the chosen parent, not two fits to the same datum.

## 5. Residue and domain checks

The direct massive photon spectrum contains an odd bound mode at \(\sqrt3\kappa\), but the odd localizer deformation produces an **even** light-source mismatch; therefore this bound photon is excluded by parity from the reported current response. The relevant positive even spectrum is a finite-box discretization of the continuum from \(2\kappa\). Its lowest finite-box mass at L=12 is approximately \(2.00557842\kappa\), **not** a separate full-line bound particle.

The normalizable gauge zero-mode derivative overlaps with the scalar-source mismatch only at numerical levels (in the six leading generalized scalar directions the worst finite-box coefficient was \(6.5\times10^{-8}\), versus the exact vanishing expected by probability normalization). Static bare-shape amplitude reproduces the independently evaluated weighted Gauss integral of the earlier report; the updated full physical-mode shape amplitude converges to 0.30036044074.

The matrix (5) has been checked positive semidefinite on the six leading scalar modes. No assertion is made that positivity of this Euclidean transverse coefficient matrix guarantees positivity of the complete Lorentzian independent-leaf spin-two theory. The source family becomes singular if the gauge kinetic function crosses zero or if the localized source is not in the relevant weighted Hilbert-space domain. The BPS vacuum and small admissible shape excursions are the stated domain.

## 6. Decision for MAT–DYN and stopping rule

**PASS:** (i) complete on-shell free light-fermion current/stress Ward identities; (ii) all finite common-metric scalar modes and pole residues; (iii) exact BPS zero heavy-current projection; (iv) positive semidefinite full scalar/heavy-gauge response matrix and independent bare-shape control; (v) explicit low-gradient operator and selection of the first heavy-gauge interaction order.

**HOLD / scientific stopping point:** no unique **renormalized** vacuum on-shell four-fermion beyond (2) can be computed from this matched tree model without choosing a consistent gauge fixing, loop regulator and counterterm/matching scheme, specifying the physical external species and copy thresholds, and solving the independent-leaf nonlinear/gravity constraints. Earlier P19/P22 loop/off-shell Ward tests cannot be promoted to a physical amplitude coefficient. The full independent-leaf parent can also introduce relative metric/helicity exchange absent from the defined common-metric theory. This work should **not** be used to claim a new SS electromagnetic force, a certified all-science parent, or a completed empirical test.

**Next decision:** WS1 MAT–DYN should determine whether the retained common-metric coupled action can be admitted as a conditional low-energy **comparison branch** and specify a particular regulator/mass/charge matching transaction for on-shell 2-to-2 loops, not simply continue arbitrary parameter scans. Any canonical change needs the author's independent approval.

## 7. Inputs and evidence boundaries

Sources consulted: canonical `SS-DYN_leafwise_dynamical_closure_v8.tex` (LaTeX source of SS-DYN v8; not included), [WN-37](WN-37_SS_KinkFermionGauge_ParentGate_v1.md), [WN-38](WN-38_SS_FullFiniteAmplitude_ParentGate_v1.md), [WN-36](WN-36_SS_TwoReductionComparison_v1.md), `SS_WardAmplitudeMatching_v1.md` (not included), WS1 [WN-27](WN-27_P19DiracMaxwellParent.md), [WN-26](WN-26_P24ScaleKinkWeight.md), and [WN-34](WN-34_P28ChargedDropletKinkSize.md). The target branch remains noncanonical.

**Reproduction:** `SS_OnShellMatch_check_v1.py` (not included) (NumPy/SciPy; 1200-node Gauss integration) prints all checks; `SS_OnShellMatch_results_v1.json` (not included) retains the eight spinor cases and three converged finite-mode pairs. The numerical checks establish finite-mode consistency and first-order source residue convergence. They do not establish UV renormalization, physical S-matrix positivity, fully continuous spectral limits or exact detector responses.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-MAT v1** (written "MAT" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MAT: Scale-Extended Matter Sources: Protected Matching, Scale Transport and Completion Gates* (version 1). Zenodo. [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555). Published; current version.

Other working notes referred to by label:

- P19: [WN-27](WN-27_P19DiracMaxwellParent.md)

Material named in this note but not included in this release: `SS-DYN_leafwise_dynamical_closure_v8.tex`, `SS_OnShellMatch_check_v1.py`, `SS_OnShellMatch_output_v1.txt`, `SS_OnShellMatch_results_v1.json`, `SS_WardAmplitudeMatching_v1.md`.
