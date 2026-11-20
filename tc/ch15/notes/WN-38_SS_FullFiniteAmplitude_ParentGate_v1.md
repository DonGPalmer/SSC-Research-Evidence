> **Public edition of evidence note WN-38.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `SS_FullFiniteAmplitude_ParentGate_v1.md`, a working note dated 9 November 2026. Not peer reviewed.
> - **Source content hash:** `2f142fa534badc8a6835ac83a3cf71d940d3f2f2dd2b6b0e0e590a1ae7da16a4` (14989 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** The scope of its √3κ gauge mode and 2κ threshold is limited to the specified action in [WN-41](WN-41_SS_Parent5D_Decision_v1.md) and [WN-42](WN-42_SS_5DParent_IntervalGate_v1r1.md), which find that they do not carry over to the covariant 5D parent. An editorial note marks the affected passage; the original wording is kept.

# Full finite SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) scalar eigenbasis and transverse gauge exchange

**Date:** 9 November 2026  
**Programme:** Donald G. Palmer, Scale Space (SS) / MAT–DYN  
**Status:** Noncanonical research and exact/finite-Galerkin tree calculation; author adoption NOT requested.  
**Scope:** Direct extension of [WN-37](WN-37_SS_KinkFermionGauge_ParentGate_v1.md), evaluated against the **canonical SS-DYN v8 finite odd basis** and the even heavy-photon spectrum of that specific coupled candidate. No change to canonical DYN or MAT.  
**Primary evidence:** `SS_FullFiniteAmplitude_check_v1.py` (not included), `SS_FullFiniteAmplitude_results_v1.json` (not included).

## Decision

> **Editorial note (public edition, 19 November 2026):** Later notes find that the heavy gauge spectrum used here, an odd bound mode at √3κ and a continuum from 2κ, comes from the weighted gauge operator of the specified 4+1 action and does not carry over to the covariant 5D parent: there the transverse graviton and gauge spectra start at zero on the full line, and on a finite interval the positive gap is not 2κ and becomes small as the interval grows. Those notes treat this as a limit on scope: the results below hold for the specified action, but their gap should not be assigned to the covariant 5D bulk. See [WN-41](WN-41_SS_Parent5D_Decision_v1.md) §5 and [WN-42](WN-42_SS_5DParent_IntervalGate_v1r1.md) §5. The text below is unchanged from the working note.

**PASS (specified quadratic/classical action, physical conserved external currents):** after full finite localizer/Einstein-metric diagonalization, the N=48 or N=96 scalar Galerkin problem reproduces canonical SS-DYN v8's reported Q pole and dimensionless coupling. The exact BPS light fermion current has zero direct coupling to every massive photon, so in the zero-field vacuum the connected **quadratic vector current–current** tree amplitude contains the massless photon only. A small admissible odd localizer shape deformation activates a positive, momentum-dependent even heavy-photon exchange that has been evaluated with 24, 48, 96 even photon modes. Its static coefficient is independently reproduced from the exact weighted 1D Gauss Green function. **Metric-mixed scalar poles contribute to the physical mass/stress scalar-density amplitude, not to a second vector-current pole at order J² in the vacuum.** They also couple to two photon field strengths, generating higher-current interactions.

**HOLD (full physical parent):** This is not the constrained independent-leaf tensor amplitude, not an independently established gauge-invariant quantum on-shell amplitude with fermion boxes/radiative thresholds, and not a complete five-dimensional parent. The gauge tower is the declared 4+1 candidate, while the scalar pencil is the same *finite odd common-metric DYN family*. Neither model proves that the assumed fermion/gauge/localizer couplings follow from SS geometry alone.

## 1. Same source action and physical comparison domain

Use the action already specified in [WN-37](WN-37_SS_KinkFermionGauge_ParentGate_v1.md): one four-dimensional Jordan metric independent of the transverse coordinate y, kink scalar X, two opposite-transverse-Yukawa fermions with one vectorlike 4D light species, and gauge kinetic weight F(X). Its reference kink is
\[
X_0=v\tanh(\kappa y),\quad F_0=\operatorname{sech}^4(\kappa y),\quad
H_0=\int F_0dy=\frac4{3\kappa},\quad
\rho_0=F_0/H_0.
\]
The gauge zero mode is constant and exactly massless from the unbroken diagonal U(1). Its physical, canonically normalized coupling is \(e_4=e_5/\sqrt{H_0}\). The fermion 4D mass m is a matched *input*, not derived.

For the scalar comparison set \(\kappa=1\) in eigenproblem units, retain the live canonical values \(r=10^{-6},\zeta_X=181150,L=12\), and vary N=24,48,96. This is the exact **type** of finite sine family defined in SS-DYN v8:
\[
x(y)=\tanh y+\sum_{j=1}^{N}a_j e_j(y),\quad
e_j=L^{-1/2}\sin(j\pi y/L)\ \ (|y|<L),\quad e_j=0\ \ (|y|\ge L).
\]
Full-line kink tails are retained in H0. The scalar finite family is distinct from the full continuous-scale spectral theory; the gauge continuum is approximated on a finite box.

Conserved external currents are separately specified classical or on-shell physical light fermion currents with p·J=0; the calculation evaluates a **transverse Euclidean exchange kernel**. It is not a completed QED scattering cross-section. Momentum p is Euclidean, measured in units κ.

## 2. Full finite scalar metric mixing, no one-mode substitution

Let \(f(y)=-4\tanh y\operatorname{sech}^2y\),
\[
f_i=\langle e_i,f\rangle,\quad
K_{ij}=\langle e_i,[-\partial_y^2+4-6\operatorname{sech}^2y]e_j\rangle,
\quad
G_{ij}=r\delta_{ij}+\frac9{8\zeta_X}f_if_j.
\]
The second term of G comes from \(\frac{3M_4^2}{2\Phi^2}\Phi_i\Phi_j\) after Einstein-frame conversion. It must not be omitted as in a bare localizer-spectrum calculation. Solve
\[
K v_a=\mu_a G v_a,\qquad v_a^TGv_b=\delta_{ab},\qquad m_a/\kappa=\sqrt{\mu_a}.
\]
The universal scalar coupling relative to unit Newton tensor strength in the DYN normalization is
\[
\alpha_a=\frac{3}{8\zeta_X}(f^T v_a)^2,
\qquad \alpha_a\ge0.
\]
These are the *physical common-metric scalar* eigenmodes of the specified finite family at linear order, not the bare \(3\kappa^2\) kink shape eigenmode. For the W-type gauge completion, the logarithmic electric-coupling derivative along the canonical scalar direction equals its logarithmic Einstein-frame fermion mass derivative:
\[
\frac{\partial\ln e_4}{\partial\varphi_a}
=\frac{\partial\ln m_E}{\partial\varphi_a}
=\frac{\partial\ln\Phi^{-1/2}}{\partial\varphi_a},
\quad
2M_4^2\left(\frac{\partial\ln e_4}{\partial\varphi_a}\right)^2=\alpha_a.
\]
This equality holds at the reference kink for zero-mode-matched fermion and photon fields **in the chosen candidate**. It does not imply a universal Jordan electromagnetic coupling.

| Finite N | first \(m_Q/\kappa\) | \(\alpha_Q\) | total \(\sum_a\alpha_a\) |
|---|---:|---:|---:|
| 24 | 340.9398181301 | 0.3208244628 | 0.3212108064 |
| 48 | 340.9360090365 | 0.3208246397 | 0.3212109653 |
| 96 | 340.9360090363 | 0.3208246397 | 0.3212109653 |

DYN v8 explicitly reports 340.936009 and 0.320824640 from its independent continuum/D1-D2 calculations. The re-evaluated finite basis agrees to the displayed precision at N>=48; the total strength minus the Q pole is ~0.000386326, or ~0.1204% of the Q pole. The next finite eigenmass is ~2019.59277 κ at L=12. Higher poles in the finite box discretize the continuum.

The scalar-density/stress exchange kernel for conserved on-shell matter stress sources is, with the usual amplitude/trace conventions,
\[
\mathcal K_{TT}^{\rm scalar}(p)
=\frac1{2M_4^2}\sum_{a=1}^N\frac{\alpha_a}{p^2+m_a^2}.
\tag{1}
\]
It multiplies the two matter trace or scalar-density matrix elements; it is **not**, by itself, a two-vector-current quadratic polarization. The massless graviton contributes the usual tensor exchange separately. The full nonlinear independent-leaf spin-2 constraints are not tested by this common-metric family.

## 3. Actual heavy photon and current matrix elements

On the same kink, write the gauge Sturm-Liouville operator
\[
\mathcal L_\gamma=-F_0^{-1}\partial_y(F_0\partial_y).
\]
With \(u=\psi/\sqrt{F_0}\), its Schrödinger representative is
\[
\mathcal H_\gamma=-\partial_y^2+4-6\operatorname{sech}^2y.
\]
It has a normalizable even massless zero mode \(\psi_0=\sqrt{F_0/H_0}\), an odd bound state at \(m^2=3\kappa^2\), and an even/odd continuum beginning at \(m=2\kappa\). An even deformed light-current density couples only to even gauge modes. The odd bound photon is therefore absent from this specific current exchange, not from the theory.

Let \(\rho_q(y)\) be the exactly normalized light fermion density on a smooth admissible static shape background \(X_q\), and let \(F_q=F(X_q)\). For normalized gauge eigenmodes \(u_n(q)\) in \(L^2(F_q dy)\),
\[
g_n(q)=e_5\int \rho_q(y)u_n(q,y)dy,\quad
g_0(q)=e_5/\sqrt{H_q},\quad H_q=\int F_qdy.
\]
At the BPS background \(\rho_0=F_0/H_0\), so
\[
\boxed{g_{n>0}(0)=0\quad\text{exactly}.}
\tag{2}
\]
The finite truncation is not needed to prove (2).

For the odd shape tangent \(\partial_q X|_0=\sqrt{3\kappa/2}\tanh(\kappa y)\operatorname{sech}(\kappa y)\), the *correct variation of the gauge eigenbasis* is included by differentiating its weighted orthogonality. Thus the heavy-mode source derivative is the mismatch
\[
d(y)=\left.\partial_q\left[\rho_q-F_q/H_q\right]\right|_0
=\frac{4C}{v}\frac{F_0}{H_0}
\left[\cosh(\kappa y)-\frac{3\pi}{8}\right],\quad C=\sqrt{3\kappa/2}.
\]
The total summed heavy-mode strength obeys Parseval:
\[
\sum_{n>0}\frac{|g_n'(0)|^2}{e_4^2}
=H_0\int \frac{d(y)^2}{F_0(y)}dy
=\frac{24\kappa}{v^2}\left(\frac32-\frac{9\pi^2}{64}\right)
=\frac{2.6900851463234154\kappa}{v^2}.
\tag{3}
\]
The numerical spectral coefficients below are reported for \(\kappa=v=1\). For general \(\kappa,v\), the shape amplitude must be converted to the same normalized tangent convention.

## 4. Physical transverse current-current amplitude

For the BPS vacuum \(X=X_0\), with no background electromagnetic field and conserved external light currents, the order-J² tree-level *electromagnetic* amplitude is
\[
\boxed{\mathcal A_{JJ}(p;X_0)
= e_4^2\,\frac{J_{1T}\cdot J_{2T}}{p^2}}
\tag{4}
\]
(up to signature signs). The metric is still dynamical, but its tree exchange is in a stress-stress channel, not directly in the vector propagator. The scalar coupling to the photon kinetic function is a \(\varphi F_{\mu\nu}F^{\mu\nu}\) vertex: with a zero background field it has **two photon legs**, so integrating out \(\varphi\) does not add an order-J² scalar pole to (4). A scalar pole enters charged *fermion–fermion* scattering through their scalar mass/stress matrix elements; it cannot be inferred from vector currents without those on-shell matrix elements. Additional scalar contributions to order-J² can arise in a nonzero electromagnetic background or at loop level; neither is included here.

For a small but finite admissible static shape displacement \(q\), with \(g_n=qg_n'(0)+O(q²)\), the transverse photon kernel is
\[
\mathcal A_{JJ}(p;X_q)=
J_{1T}\cdot J_{2T}
\left[
\frac{e_5^2}{H_qp^2}
+q^2 e_4^2\mathcal S_\gamma(p)+O(q^3)_{\rm heavy}
\right],
\]
\[
\mathcal S_\gamma(p)=
H_0\sum_{\substack{n>0\\\mathrm{even}}}
\frac{\left|\langle d/\sqrt{F_0},\,\psi_n\rangle\right|^2}{p^2+m_{\gamma,n}^2}.
\tag{5}
\]
The exact \(e_5^2/H_q\) is deliberately retained rather than truncating its O(q²) massless-pole coefficient without computing \(H_q''\). The remainder describes only the heavy component at fixed p away from its poles. A deformed q field is an externally held background, not an established stationary solution of the complete dynamical theory.

To evaluate (5), use even orthonormal functions \(\cos[(j+\tfrac12)\pi y/L]/\sqrt L\) on \([-L,L]\), Galerkin diagonalize \(\mathcal H_\gamma\), discard the normalized near-zero state, and sum all remaining even modes. At \(L=12\):

| \(p/\kappa\) | N=24 | N=48 | N=96 |
|---|---:|---:|---:|
| 0 | 0.615260211 | 0.615268423 | 0.615268423 |
| 0.5 | 0.581559643 | 0.581567180 | 0.581567180 |
| 1 | 0.499618610 | 0.499624594 | 0.499624594 |
| 2 | 0.320021077 | 0.320024135 | 0.320024135 |
| 4 | 0.131643201 | 0.131644039 | 0.131644039 |
| 10 | 0.025753412 | 0.025753514 | 0.025753514 |

The first positive even finite-box eigenvalues approach \(m_\gamma^2/\kappa^2=4.0223448094, 4.1988593885,\ldots\). These are **continuum-box levels**, not physical isolated massive particle predictions. The odd \(m_\gamma=\sqrt3\kappa\) bound state is parity-forbidden here.

The N=96 total squared overlap is 2.69008514347 versus the exact 2.69008514632. The near-zero eigenvalue has numerical magnitude below \(2\times 10^{-12}\) and source overlap <\(2\times10^{-13}\), as expected from gauge protection. At \(p=100\kappa\), \(\mathcal S_\gamma=0.0002688885695\), in agreement with the large-momentum total-residue limit \(\lim_{p\to\infty}p^2\mathcal S_\gamma(p)=2.6900851463\).

## 5. Independent static Gauss-law check

The static projected Green function can be computed without gauge eigenvectors. The weighted gauge equation with source d is
\[
-\partial_y(F_0\partial_y u)=d,\qquad \int d\,dy=0.
\]
Writing \(t=\tanh y\) for \(\kappa=v=1\), define
\[
Q(t)=\tfrac12[t\sqrt{1-t^2}+\arcsin t]
-\frac{3\pi}{8}\left(t-\frac{t^3}{3}\right).
\]
The integrated source is \(D(y)=(4C/H_0)Q(\tanh y)\). Integration by parts and the finite-energy boundary conditions yield
\[
\boxed{\mathcal S_\gamma(0)
=18\int_{-1}^{1}\frac{Q(t)^2}{(1-t^2)^3}\,dt
=0.61526842194\ldots .}
\tag{6}
\]
A separate high-precision quadrature agrees with the N=96 spectral answer to ~\(1.3\times10^{-9}\), an independent static check. Equation (6) is a **convergent finite-energy continuum value**, not a claim that the full coupled dynamical electromagnetic background has been evolved.

## 6. What the combined amplitude says (and does not say)

For scattering of physical charged fermions, a schematic tree matching includes:
- transverse massless photon (and possible massive photon residues under a held non-BPS shape);
- scalar exchange between **mass/stress** matrix elements, governed by (1), including Einstein-metric mixing;
- ordinary massless graviton exchange between conserved stress tensors;
- no additional tree-level scalar *vector-current two-point pole* in the zero-field BPS vacuum.

In the nonrelativistic limit, scalar exchange adds a universally normalized Yukawa potential between masses, with weights \(\alpha_a\). The same localizer shape mode changes the effective electric coupling in W but not in universal-Jordan U. Thus the W and U candidate theories are distinguishable even though both have the same reference kink and canonically matched \(m,e\).

**No distinctive empirical SS prediction follows yet.** Absolute κ, the actual matter current/stress matrix elements, the physical background and electromagnetic calibration, the far-tail effective cutoff and loop matching are not fixed by this calculation. QED Ward identities protect the diagonal charge on a given background but do not alone establish radiative protection of \(F(X)\), fermion localization, or the full independent-leaf constraint system.

## 7. Scope and verification

This is a scientific calculation plus new additive research output for comparison with the WS1 notes. Parent action changes, regulators and loop matching lie outside its scope.

**Reproducibility:** The Python script `SS_FullFiniteAmplitude_check_v1.py` (not included in this release) builds the precise finite sine basis, metric-mixed generalized scalar eigenproblem, gauge Galerkin continuum, numerical overlaps and amplitude values. It checks scalar eigenvector G-orthonormality, reproduces the canonical SS-DYN pole/coupling, checks total heavy-photon strength against exact Parseval, and reports the gauge zero-mode overlap. The independent integrated-Gauss quadrature is recorded separately. The result is a reproducible **tree-level comparison**; a complete parent-model on-shell amplitude still needs constrained tensor, spinor vertex and loop matching.

**Sources consulted:** canonical `SS-DYN_leafwise_dynamical_closure_v8.tex` (LaTeX source of SS-DYN v8; not included), related integration working reports [WN-37](WN-37_SS_KinkFermionGauge_ParentGate_v1.md), [WN-36](WN-36_SS_TwoReductionComparison_v1.md), [WN-40](WN-40_SS_ProfileSelection_Decision_v1.md), `SS_WardAmplitudeMatching_v1.md` (not included) and WS1 [WN-27](WN-27_P19DiracMaxwellParent.md).

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN", "DYN v8" in this note): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-MAT v1** (written "MAT" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MAT: Scale-Extended Matter Sources: Protected Matching, Scale Transport and Completion Gates* (version 1). Zenodo. [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555). Published; current version.

Material named in this note but not included in this release: `SS-DYN_leafwise_dynamical_closure_v8.tex`, `SS_FullFiniteAmplitude_check_v1.py`, `SS_FullFiniteAmplitude_results_v1.json`, `SS_WardAmplitudeMatching_v1.md`.
