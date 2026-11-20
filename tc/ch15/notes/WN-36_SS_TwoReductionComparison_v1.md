> **Public edition of evidence note WN-36.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `SS_TwoReductionComparison_v1.md`, a working note dated 9 November 2026. Not peer reviewed.
> - **Source content hash:** `4490be8d53923cf27075ee61d7680438facbb9560189627acbef9df2be5d72bc` (13155 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# SS two-reduction comparison: one kink, matched material inputs, different gauge response

**Programme:** Scale Space / SSC; **Date:** 9 November 2026  
**Status:** Noncanonical, unregistered conditional research candidate. No canonical adoption or physical data fit.  
**Source authority:** The *U* Jordan matter term and gravitational/localizer functional are those printed in canonical SS-DYN v8 [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). The full-line one-odd-mode projection is a controlled **quadratic Galerkin diagnostic**, not a claim to reproduce its finite `D_{N,L}` pole spectrum. The *W* matter term is a separate proposed extension, not an adopted canonical change.  
**Files:** [WN-36](WN-36_SS_TwoReductionComparison_v1.md), `SS_TwoReductionComparison_v1.tex` (not included), `SS_TwoReductionComparison_check_v1.py` (not included).

## 1. Decision

**PASS (exact conditional effective-action comparison):** Starting from the same scalar–tensor/localizer gravitational functional and the same four-dimensional Dirac–Maxwell material parameters at the kink, a universal Jordan matter term and a uniformly dynamically weighted matter term have identical canonically normalized Einstein-frame fermion *mass dependence* but different electromagnetic gauge-kinetic functions. The difference survives scalar–metric canonicalization and produces unequal logarithmic responses of the *dimensionless* fine-structure parameter and of dimensionless Coulomb observables. In particular, `d ln(B/m)/d ln Phi = 0` for U and `-2` for W at the leading matched Coulomb level, without an added independently fitted coupling.

**HOLD (complete SS parent):** This comparison does not establish that the W action is dynamically selected, that the odd Galerkin mode equals the full DYN physical scalar pole, that an independent-leaf multigravity completion is ghost-free, or that either model has passed experimental bounds. Quantum Coulomb and annihilation formulas are the conventional controlled weak-coupling *conditional* light Dirac–Maxwell completion of the P19 branch, not a derivation of the Standard Model or ordinary chemical matter. The two actions are **different**; matching their reference input does not assert they are the same microscopic theory.

## 2. The same physical input and two complete four-dimensional action prescriptions

Let `g_J` be one Jordan metric in four clock-reading directions, `y` proper scale, `X(x,y)` the localizer, and `psi_A(x), A_mu(x)` declared y-uniform matter/gauge fields. Take

\[
 F(X)=(1-X^2/v^2)^2,\quad
 B[X]=\partial_yX-\kappa v(1-X^2/v^2),\quad
 W(X)=\int_{\mathbb R} F(X)\,dy,\quad \Phi=W/W_0,
\]
\[
 X_0=v\tanh(\kappa y),\quad W_0=4/(3\kappa),\quad M_4^2=M_5^3W_0.
\]
Use **the same gravitational/localizer action** on both sides:
\[
 S_G=\int d^4x\sqrt{-g_J}\left[
   \frac{M_4^2}{2}\Phi R_J
 - \frac{rZ_X}{2}\int dy\,g_J^{\mu\nu}\partial_\mu X\partial_\nu X
 - \frac{Z_X}{2}\int dy\,B[X]^2\right],\qquad r>0.
\tag{1}
\]
This is the declared classical functional of SS-DYN v8 before finite regularization. For a strict canonical model member, its finite-dimensional profile/domain restriction must be used; here the full-line continuum functions provide analytic **comparison** formulas. We hold `M_5, Z_X, r, kappa, v` and the background centre fixed in both actions.

Define the same four-dimensional Jordan Dirac–Maxwell functional, with equal physical reference masses `m_A`, representation charges `q_A`, and gauge normalization `g_0`:
\[
S_m=\int\sqrt{-g_J}\left[-\frac{1}{4g_0^2}F_{\mu\nu}F^{\mu\nu}
+\sum_A\bar\psi_A(i\gamma_J^\mu D_\mu-m_A)\psi_A+\mathcal L_{\rm int}\right].\tag{2}
\]
All fields, boundary conditions, stress-tensor prescriptions and effective momentum ranges must match. The two **distinct** complete actions being compared are
\[
\boxed{S_U=S_G+S_m[g_J,\psi,A]},\qquad
\boxed{S_W=S_G+\Phi(X)\,S_m[g_J,\psi,A]}.\tag{3}
\]
Here `Phi S_m` means the multiplier is inserted **inside the local four-dimensional integral**. `S_U` follows the universal Jordan choice of canonical DYN; `S_W` is the scale-uniform reduction of the locally `F(X)`-weighted action in [WN-35](WN-35_SS_SingleActionReduction_v1.md). The bare parameter of that parent must be chosen `g_5^2=W_0g_0^2` to make its reference photon kinetic term identical; similarly normalize its fermions so the reference pole mass and charge agree. No additional free phenomenological parameter is introduced for the comparison.

## 3. Exact Einstein-frame Dirac and Maxwell reduction

For positive Phi set `g_E=Phi g_J`. In four dimensions the Maxwell density is conformally invariant, while a Jordan Dirac kinetic density carries `Phi^{-3/2}` and a Dirac mass density `Phi^{-2}`. If `C(Phi)=1` for U and `C(Phi)=Phi` for W, then in the Einstein metric
\[
\mathcal L_{\rm ferm,E}=C\Phi^{-3/2}\bar\psi i\slash D_E\psi
 - C\Phi^{-2}m\bar\psi\psi
\quad\text{(spin-connection terms handled by the conformal spinor map)}.\tag{4}
\]
Using the symmetric Hermitian Dirac kinetic term and a local rescaling to unit kinetic coefficient, the reference scalar mass becomes
\[
\boxed{m_E(\Phi)=m\Phi^{-1/2}\quad\text{in BOTH actions}.}\tag{5}
\]
A local scalar-spinor rescaling does not authorize ignoring the quantum functional Jacobian or derivative operators at loop order. Equation (5) is tree-level.

The Maxwell coefficient instead reads
\[
-\frac{C(\Phi)}{4g_0^2}F_E^2,\qquad
\boxed{g_U^2(\Phi)=g_0^2,\quad g_W^2(\Phi)=g_0^2/\Phi}.\tag{6}
\]
Thus the physical dimensionless low-energy Coulomb coupling, conditional on compatible matching and no additional charged threshold effects, is
\[
\boxed{\alpha_U(\Phi)=\alpha_0,\qquad \alpha_W(\Phi)=\alpha_0/\Phi}.\tag{7}
\]
The precise operational alpha requires a photon/charge renormalization prescription. (6) is a tree-level gauge-kinetic fact, not a one-loop prediction.

## 4. Exact odd Galerkin mode, scalar--metric canonicalization, and response matrix

Use the source-free background `X_0` with fixed centre and the normalized odd fluctuation
\[
\chi_1(y)=\sqrt{3\kappa/2}\,\mathrm{sech}(\kappa y)\tanh(\kappa y),
\quad X=X_0+q(x)\chi_1(y)/\sqrt{Z_X}.
\]
The BPS Hessian eigenvalue is `3 kappa^2`, but the four-dimensional kinetic normalization is `r`, not unity unless `r=1`.

The exact weight overlap (previously derived; independently checked) is
\[
 W=W_0+hq+O(q^2),\quad
 h=\frac1{\sqrt{Z_X}}\int F_X(X_0)\chi_1dy
 =-\frac{\sqrt6\pi}{4\sqrt{Z_X\kappa}\,v}.\tag{8}
\]
The conformal change of metric produces the **positive** additional Einstein-frame kinetic coefficient
\[
\boxed{K=r+\frac32M_4^2(h/W_0)^2
=r+\frac{27\pi^2M_5^3}{64Z_Xv^2}>0.}\tag{9}
\]
The canonical odd coordinate at linear order is `varphi=sqrt(K) q`. Within this one-coordinate Galerkin truncation its squared scalar mass and logarithmic modulus are
\[
\boxed{m_{\varphi}^2=3\kappa^2/K},\qquad
\boxed{\sigma=\left.\frac{d\ln\Phi}{d\varphi}\right|_0=\frac{h}{W_0\sqrt K}}.\tag{10}
\]
The canonically normalized scalar charges of a massive free Dirac source and the gauge kinetic coupling are therefore
\[
\begin{array}{c|cc}
&\partial_\varphi\ln m_E&\partial_\varphi\ln g\\\hline
U&-\sigma/2&0\\
W&-\sigma/2&-\sigma/2
\end{array}.\tag{11}
\]
The *one-odd-mode* Euclidean scalar-coefficient response kernel for operators with these canonical charges is
\[
\mathscr R^{(s)}_{AB}(p_E^2)=\frac{c_A^{(s)}c_B^{(s)}}{p_E^2+m_\varphi^2},\tag{12}
\]
with `A,B` drawn from the **complete** matched rest-mass and gauge-kinetic operator basis, not arbitrary density source labels. Thus for U the mass--photon scalar cross entry vanishes, while for W it is `sigma^2/[4(p_E^2+m_varphi^2)]` and the photon--photon entry is the same. Both models share the same mass--mass entry in this one-coordinate comparison. Its static coefficient equals `9*pi^2/(512 Z_X kappa v^2)` (the K factors cancel). This is a site/operator coefficient before the photon stress, full graviton tensor exchange, quantum Ward and complete metric/scalar constraints are contracted; it is NOT a physical-force prediction or a full S-matrix.

**Critical finite-model qualification.** In DYN v8 the actual scalar eigenvalue problem is a rank-one generalized pencil: its physical odd Q is *not generically identical* to the bare odd BPS eigenfunction. The finite `D_{N,L}` physical pole reported in the canonical paper must not be overwritten by `3 kappa^2/K`. The present reduction is an explicit matched **one-mode projection** used on both actions; it preserves the correct action-level and photon-normalization comparison. A complete finite-member amplitude comparison must use the *same DYN physical eigenbasis and corresponding projection* in both U and W.

## 5. Different linked predictions for a matched conditional neutral composite

For the same weakly coupled Dirac--Maxwell particle/antiparticle pair, conditional on a controlled light sector and matching, the conventional leading Coulomb scale is `B=m_E alpha^2/4`, the equal-mass Bohr radius is `a=2/(m_E alpha)` (units `hbar=c=1`), and the spin-singlet annihilation width is `Gamma=m_E alpha^5/2`. The actions then require the exact **logarithmic response exponents** in this approximation:

| Observable | U exponent in Phi | W exponent in Phi |
|---|---:|---:|
| `m_E` | -1/2 | -1/2 |
| `alpha` | 0 | -1 |
| `B` | -1/2 | -5/2 |
| `a` | +1/2 | +3/2 |
| `Gamma` | -1/2 | -11/2 |
| **`B/m_E`** (dimensionless) | **0** | **-2** |
| **`Gamma/B`** (dimensionless) | **0** | **-3** |
| **`a/(1/m_E)`** (dimensionless) | **0** | **+1** |

These are **not** direct observations of a varying fine-structure constant. They are response predictions if the same physical localizer excitation can be prepared/read out and if the conditional P19 light QED EFT remains valid at the binding and hard-annihilation scales. Standard radiative corrections, scalar-induced shifts in matching masses and extra heavy operators could modify the simple exponents. A common scalar change in all dimensionful rest masses is not itself a clean observable, whereas a dimensionless ratio is.

## 6. A precise decision and remaining certificate

The accepted universal-Jordan prescription U passes the **tree-level metric-only coupling criterion**: the Maxwell coefficient is independent of the localizer, and the fermion's apparent scalar mass dependence follows the single Jordan metric. The proposed W branch **fails exact metric-only universality for nonzero h**, because conformal four-dimensional geometry cannot produce its `Phi F^2` gauge coefficient. This is a theorem about the declared two actions and operator basis; it is not a general no-go for dynamically weighted parents with extra gauge/compensator structure.

The positive shared-parent gain is that both prescriptions are now calculated from **one pinned gravitational/localizer sector with identical background matter inputs**, and their differences are expressed in a common physical operator basis. No independent molecular/bulk/biological scalar coupling was fitted. The result identifies the necessary next choices:

1. **Protect U:** derive the universal Jordan matter coupling from a regulator-fixed independent-leaf parent while retaining protected metric/source weights and controlling scalar threshold terms, or
2. **Complete W:** justify dynamical `Phi` matter weighting with a symmetry/compensator and compute gauge, Dirac and radiative matching. A bare `Phi` factor is new physical content, not a derivation of universal metric coupling.

In either case, calculate the **full constrained finite-member** tensor/scalar/gauge pole-and-residue matrix. The one-odd-mode value above is a transparent diagnostic rather than that final certificate. Derive an actual intrinsic-`u` material density and measurement map before claiming that QED molecular size distributions or BIO populations probe this coordinate. No model is approved for canonical adoption by this analysis.

## 7. Sources and reproducibility

Primary live source read: `SS-DYN_leafwise_dynamical_closure_v8.tex` (LaTeX source of SS-DYN v8; not included) (canonical), especially its Jordan functional, `r>0`, Einstein-frame kinetic metric, and rank-one spectral pencil. Other live sources: [WN-27](WN-27_P19DiracMaxwellParent.md), [WN-26](WN-26_P24ScaleKinkWeight.md), [WN-32](WN-32_P26ChargeExtentOnKink.md), [WN-34](WN-34_P28ChargedDropletKinkSize.md), and [WN-35](WN-35_SS_SingleActionReduction_v1.md) (predecessor note), [WN-09](WN-09_SS_ParentMatter_DiracMatching_v1.md), [WN-11](WN-11_SS_ParentMatter_FiniteSpectrum_v1.md), `SS_CompositeScaleProfile_v1.md` (not included). Existing WS1, canonical SS-DYN, MAT, MULTI, BIO and MEAS records remain unchanged.

Reproduction: `python SS_TwoReductionComparison_check_v1.py` (not included), standard SymPy, performs exact Einstein-frame fermion-mass and gauge reductions, `r`-dependent scalar canonicalization, tree-level source matrix and the eight logarithmic-response exponents. No third-party data downloaded or fitted; no external peer review. Avoid treating the arbitrary single-mode Galerkin scalar pole as the exact DYN pole or treating classical conditional results as validation of SS-specific physics.

---

## References and related notes (public edition)

Published works cited:

- **SS-BIO v4** (written "BIO" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-BIO: Scale-Extended Biological Dynamics in Scale Space: Configurational Structure, Transport, and Reaction–Diffusion Tests* (version 4). Zenodo. [doi:10.5281/zenodo.23874087](https://doi.org/10.5281/zenodo.23874087). Published; current version.
- **SS-DYN v8** (written "DYN", "DYN v8" in this note): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-MAT v1** (written "MAT" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MAT: Scale-Extended Matter Sources: Protected Matching, Scale Transport and Completion Gates* (version 1). Zenodo. [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555). Published; current version.
- **SS-MEAS v2** (written "MEAS" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MEAS: Measurement Projection and Identifiability in Scale Space: Calibrated Observables, Null Spaces, and Withheld-Probe Tests* (version 2). Zenodo. [doi:10.5281/zenodo.23865651](https://doi.org/10.5281/zenodo.23865651). Published; current version.
- **SS-MULTI v2** (written "MULTI" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MULTI: Physical Scale as a Location Coordinate: A Multi-Scale Framework in Scale Space* (version 2). Zenodo. [doi:10.5281/zenodo.23873325](https://doi.org/10.5281/zenodo.23873325). Published; current version.

Other working notes referred to by label:

- P19: [WN-27](WN-27_P19DiracMaxwellParent.md)

Material named in this note but not included in this release: `SS-DYN_leafwise_dynamical_closure_v8.tex`, `SS_CompositeScaleProfile_v1.md`, `SS_TwoReductionComparison_check_v1.py`, `SS_TwoReductionComparison_v1.tex`.
