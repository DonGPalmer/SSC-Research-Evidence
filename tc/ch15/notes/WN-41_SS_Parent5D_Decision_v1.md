> **Public edition of evidence note WN-41.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `SS_Parent5D_Decision_v1.md`, a working note dated 10 November 2026. Not peer reviewed.
> - **Source content hash:** `b5a5ad0084ac80e9aa3f39c51ed590624babe99c39c2530966e465b3c70124d6` (15422 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# SS parent identification: exact Einstein–localizer warp and coupled source-alignment gate

**Research date:** 10 November 2026  
**Status:** Noncanonical working result; no proposed change to accepted SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) or SS-MAT [v1, doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555).  
**Outcome:** PASS—explicit covariant 5D Einstein–scalar background generating the SS `sech^4` gravitational weight, with one conditional fermion/gauge alignment construction. FAIL—the exact same warp with a *constant-kinetic original tanh field* as the sole Einstein source. HOLD—the constructed 5D parent does **not** inherit SS-DYN's gapped reduced-mode spectra, and a constant fermion mixing mass and generic bulk gauge counterterm violate the desired protected reduction.

## Executive decision

A stronger parent **candidate** can be stated explicitly:
\[
S=\int d^5x\sqrt{-g_5}\left[\frac{M_5^3}{2}R_5
-\frac12(\partial\phi)^2-V(\phi)
-\frac{Z_A(\phi)}{4e_5^2}F_{MN}F^{MN}
+\sum_{s=\pm}\bar\Psi_s(i\Gamma^M D_M-sY(\phi))\Psi_s
\right]+S_{\rm optional\,mass}.
\tag{1}
\]
The scalar potential is fixed through one first-order superpotential:
\[
\mathcal W(\phi)=6M_5^3\kappa\sin\theta,\quad
\theta=\frac{\phi}{\sqrt{6M_5^3}},\quad
V=\tfrac12\mathcal W_\phi^2-\frac{2}{3M_5^3}\mathcal W^2
=3M_5^3\kappa^2(1-9\sin^2\theta).
\tag{2}
\]
The additional constitutive choices
\[
Z_A(\phi)=\cos^4\theta,\qquad Y(\phi)=\frac{\mathcal W(\phi)}{2M_5^3}=3\kappa\sin\theta
\tag{3}
\]
are **specified, not derived by gravity alone**. They align the photon and the massless chiral-fermion source density with the gravitational tensor zero-mode weight. The construction is a controlled background-level example, not a demonstrated unique parent, complete supersymmetric theory, or quantum-corrected completion.

The same calculation finds decisive limitations: the fully covariant 5D tensor/gauge continua reach zero invariant mass, and constant 5D left-right mixing produces a mass-term source mismatch quantified exactly by \(1/14\) (squared heavy-to-common normalized overlap). For a noncompact scale direction, an arbitrarily small strictly positive *uniform* gauge kinetic floor destroys the normalizable photon zero mode. The parent candidate is therefore **not yet suitable for promotion** as the origin of both the canonical SS-DYN scalar spectrum and ordinary stable massive quantum matter.

## 1. First theorem: original \(X=v\tanh(\kappa y)\) and exact warp do not solve constant-kinetic Einstein–scalar equations

Use signature (-++++), \(\mathrm ds_5^2=e^{2A(y)}\eta_{\mu\nu}dx^\mu dx^\nu+dy^2\), and
\[
S_{5,X}=\int\sqrt{-g_5}\big[\tfrac12 M_5^3R_5-\tfrac{Z_0}2(\partial X)^2-V(X)\big]
\]
with \(Z_0>0\) constant and no other background source. The independent Einstein equations are
\[
6M_5^3(A')^2=\tfrac{Z_0}2(X')^2-V,\qquad
3M_5^3A''=-Z_0(X')^2.
\tag{4}
\]
Demand \(X=v\tanh(\kappa y)\) and \(e^{A}=\operatorname{sech}^2(\kappa y)\).
Then \(X'=\kappa v\,\operatorname{sech}^2(\kappa y)\) whereas
\(A''=-2\kappa^2\operatorname{sech}^2(\kappa y)\). Equation (4) requires
\[
\boxed{Z_{\rm required}(X)=\frac{6M_5^3}{v^2(1-X^2/v^2)}}.
\tag{5}
\]
It cannot be a constant on the wall. **No choice of potential \(V(X)\)** can repair this contradiction in the difference Einstein equation. This is a theorem for *one minimally coupled scalar with constant kinetic coefficient and the stated ansatz*, not for all 5D parents or for the fixed common-metric SS-DYN theory.

## 2. Exact constructive repair by a canonical reparametrization

The \(Z_{\rm required}\) in (5) is positive on \(|X|<v\), although divergent in the original \(X\) coordinate at its vacua. Introduce the canonical field
\[
\phi=\sqrt{6M_5^3}\arcsin(X/v),\qquad
X=v\sin\theta,\quad\theta=\phi/\sqrt{6M_5^3}.
\]
The original background \(X=v\tanh(\kappa y)\) becomes
\[
\phi(y)=\sqrt{6M_5^3}\arcsin[\tanh(\kappa y)].
\]
The superpotential equations \(\phi'=\mathcal W_\phi\),
\(A'=-\mathcal W/(3M_5^3)\) and the choice (2) give
\[
A(y)=-2\ln\cosh(\kappa y),\quad e^{2A}=\operatorname{sech}^4(\kappa y).
\tag{6}
\]
The scalar Einstein equations AND the independently evaluated scalar EOM
\[
\phi''+4A'\phi'=V_\phi
\]
vanish exactly upon substitution. The scalar potential approaches
\(-24M_5^3\kappa^2\) in either asymptotic vacuum, giving an AdS-like bulk; the scalar mass squared about either vacuum is \(9\kappa^2>0\). The \(X\)-coordinate singularity is removable through the canonical \(\phi\) field, but \(X\) is not globally a canonical field at its endpoint vacua.

The geometry gives without a fitted gravitational source weight
\[
W_0=\int_{-\infty}^\infty e^{2A}dy=\frac4{3\kappa},\qquad
M_4^2=M_5^3W_0.
\tag{7}
\]
This realizes the *background* weight in canonical SS-DYN v8 and WS1 P24 through a bona fide dynamical 5D metric. It does **not** prove the same full scalar multiplet or reduce to the independent-leaf parent.

## 3. One coupled fermion–photon source construction

A minimally coupled 5D Maxwell field with constant bulk gauge kinetic factor has zero-mode norm \(\int_{\mathbb R}dy=\infty\), since the warp cancels from its 4D \(F_{\mu\nu}^2\) action. Therefore a dielectric/localization function is needed for a massless photon on the complete scale line. Specify the same superpotential-related function
\[
Z_A(\phi)=\left[\frac{\mathcal W_\phi}{\sqrt{6M_5^3}\kappa}\right]^4
=\cos^4\theta=e^{2A(y)}=\operatorname{sech}^4(\kappa y)
\quad\hbox{on the background}.
\tag{8}
\]
It gives a constant normalizable photon zero mode and \(e_4=e_5/\sqrt{W_0}\).

A warped 5D Dirac mode obeys, for a chosen chirality,
\[
f_L'+(2A'+Y)f_L=0,\qquad
Y(\phi)=\frac{\mathcal W}{2M_5^3}=3\kappa\sin\theta.
\tag{9}
\]
The exact profile is \(f_L\propto e^{-A/2}\) (the unrescaled 5D spinor function need not decay pointwise), and its **physical normalized 4D kinetic/current density** is
\[
\rho_f(y)=\frac{e^{3A}|f_L|^2}{\int e^{3A}|f_L|^2dy}
=\frac{e^{2A(y)}}{W_0}.
\tag{10}
\]
The sign-reversed \(Y\) for a second 5D spinor supplies an opposite-chirality mode with the same normalized density; together they form a vectorlike massless 4D light sector at this stage. This is a background-mode construction and does not establish an isolated massive Dirac fermion.

Thus the **tensor**, photon and massless light-fermion kinetic/current sources all have the same weight \(e^{2A}\). Every direct heavy-mode current overlap vanishes with respect to a complete \(L^2(e^{2A}dy)\) basis:
\[
g_n\propto \int e^{2A}u_n dy=0,\quad n>0.
\tag{11}
\]
Exact alignment results from the stated superpotential-related Yukawa **and** dielectric choices. This is not a proof that a symmetry enforces them, or that the 5D longitudinal scalar constraints and radiative thresholds close.

## 4. New obstruction: massive Dirac matter loses source alignment with constant 5D mixing

To obtain a 4D Dirac mass, one may add constant 5D left-right mixing \(m_5\bar\Psi_+\Psi_-+\mathrm{h.c.}\). The *projected* mass matrix element carries the 5D volume weight
\[
Z_{\rm mass}(y)\propto e^{4A}f_Lf_R=e^{3A}
=\operatorname{sech}^6(\kappa y),
\]
whereas the kinetic/current weight is \(Z_{\rm kin}=e^{2A}=\operatorname{sech}^4\). They are not proportional.

The exact relative-mode **squared overlap**, normalized by the common-mode squared overlap of the mass source, is
\[
R_{\rm mass}
=\frac{(\int e^{2A})(\int e^{4A})}{(\int e^{3A})^2}-1
=\frac{I_4I_8}{I_6^2}-1
=\boxed{\frac1{14}},
\tag{12}
\]
where \(I_n=\int_{-\infty}^\infty\operatorname{sech}^n z\,dz\).
The light-light mass matrix element obtained by projection is
\[
m_{\rm projected}=m_5\frac{\int e^{3A}}{\int e^{2A}}
=\boxed{\frac45\,m_5}.
\tag{13}
\]
Equation (13) is **not** a certified physical pole mass: an exact massive light eigenstate would require re-solving the full coupled fermion spectrum, including the gapless continuum below. Equation (12) precisely identifies the mass operator's mismatch in the *unmixed reference basis*, not a full massive fermion graviton amplitude.

In the same projected setting, pointwise mass-source alignment would require
\[
m_5(y)\propto e^{-A(y)}m_4
=m_4\sec^2\theta.
\tag{14}
\]
This diverges at the asymptotic scalar vacua; it is not accepted as a healthy repair merely because the weighted integral is finite. A symmetry-based mass-generation mechanism or different field content is needed. Constant mass mixing does not inherit the apparently protected massless current alignment.

## 5. Fully covariant tensor/gauge spectrum: no finite positive gap

The transverse traceless graviton and the transverse Maxwell mode with (8) obey **identical** 5D weighted Sturm–Liouville operators:
\[
-\partial_y[e^{4A(y)}\partial_y u_n]=m_n^2e^{2A(y)}u_n.
\tag{15}
\]
This equality is a positive nontrivial consequence of the aligned gauge dielectric, but it invalidates a naive import of the earlier *anisotropic* reduced gauge operator \(-F^{-1}(Fu')'\) and its threshold \(2\kappa\).

In the conformal coordinate \(dz=e^{-A}dy\), both reduce to
\[
\big[-\partial_z^2+V_T(z)\big]\psi_n=m_n^2\psi_n,\qquad
V_T=\frac32 A_{zz}+\frac94A_z^2
=e^{2A}\Big(\frac32A_{yy}+\frac{15}{4}A_y^2\Big).
\tag{16}
\]
For the exact wall,
\[
V_T(z(y))=\kappa^2\operatorname{sech}^4(\kappa y)
[18\tanh^2(\kappa y)-3].
\tag{17}
\]
This operator factorizes, with a normalizable zero mode \(\psi_0\propto e^{3A/2}\). Since \(z(y)\sim e^{2\kappa|y|}/(8\kappa)\) and \(e^{A}\sim1/(2\kappa|z|)\), 
\[
V_T(z)\sim\frac{15}{4z^2}\longrightarrow0
\qquad(|z|\to\infty).
\tag{18}
\]
Hence the essential spectrum of both the transverse graviton and the specified transverse gauge operator starts at **zero** mass squared. There is no positive KK mass gap on the complete line, notwithstanding the normalizable zero mode.

This is a **hard incompatibility** with identifying the physical 5D tensor/gauge spectrum with the \(m=\sqrt3\kappa\) bound mode and \(2\kappa\) continuum edge computed by the prior noncovariant weighted operator. The accepted common-metric SS-DYN scalar pencil has its own pole \(m_Q/\kappa\simeq340.936\); that pole has **not** been derived as a fluctuation of this new fully covariant Einstein–scalar wall.

A finite scale interval, different asymptotics, additional constraints or other localization mechanism may discretize/gap the sector. Each is added physical input and must be specified before declaring the parent complete.

## 6. Second structural obstruction: bulk gauge kinetic radiative protection

On \(\mathbb R_y\), the photon normalization is \(H_A=\int Z_A(y)dy=4/(3\kappa)\). A *uniform* local gauge-invariant counterterm \(\delta Z_A=\varepsilon>0\) produces
\[
H_A(\varepsilon)=\int[Z_A(y)+\varepsilon]dy=\infty.
\tag{19}
\]
Thus the normalizable 4D photon zero mode disappears for **any** strictly positive uniform bulk kinetic floor on the noncompact scale line. This is an exact functional-analytic sensitivity statement, **not** a proof that the specific quantum theory necessarily generates such a floor. Standard gauge symmetry permits an ordinary bulk \(F_{MN}^2\) term, so naturalness requires a symmetry, confinement, boundary mechanism or an independently established renormalization prescription that avoids this counterterm. A brane-localized correction is a different and potentially harmless profile; do not conflate it with (19).

## 7. Scientific verdict and programme alignment

| Gate | Finding | Status |
|---|---|---|
| Exact 5D Einstein + localizer background with SS weight | Explicit canonical scalar solution, all background equations checked | PASS, candidate |
| Same geometry with constant-kinetic original tanh field | Einstein difference equation forbids it for one scalar | FAIL (restricted no-go) |
| Massless photon, chiral fermion and graviton source alignment | Same \(\operatorname{sech}^4\) normalized weight with declared constitutive functions | PASS at tree/background |
| Massive Dirac stress-source alignment with constant mixing | Exact positive mismatch \(1/14\) | FAIL in projected sector |
| Canonical DYN/previous gauge \(2\kappa\) spectral gap inherited | 5D covariant tensor and gauge continuum begins at zero | FAIL |
| Protect localized photon under all permitted bulk operators | Uniform \(\varepsilon F^2\) destroys zero-mode normalizability | HOLD |
| Complete independent-leaf constraints, regulated on-shell QED, physical SS size map | Not supplied | HOLD |

**Recommendation:** Retain this as the first explicit fully 5D *Einstein–localizer background* candidate with related matter/gauge sources, but **do not promote it** to the universal SSC parent. The decisive next gate is not additional parameter fitting. Choose whether the parent is intended to be fully 5D covariant on a noncompact scale axis, or the restricted anisotropic/common-metric SS-DYN construction. If fully 5D covariant, its inherently gapless tensor/gauge spectra and gauge localization protection must be resolved. If restricted SS-DYN is retained, it must not be claimed to descend unchanged from the covariant model above.

The known five-dimensional domain-wall first-order formalism and localization mechanisms are well developed in prior literature. This result is an application and a compatibility test for the specific SSC weight, **not** a claim of a new supergravity theorem. No experimental data supplied by the author were used.

## Sources and provenance

- SSC source: `SS-DYN_leafwise_dynamical_closure_v8.tex` (LaTeX source of SS-DYN v8; not included); describes the canonical finite common-metric \(D_{N,L}\) model, scalar pole and protected profile, but does not claim a unique covariant five-dimensional parent.
- WS1 working calculations: [WN-26](WN-26_P24ScaleKinkWeight.md), [WN-27](WN-27_P19DiracMaxwellParent.md) and [WN-08](WN-08_P18RegulatedLoop.md).
- Related working results: [WN-40](WN-40_SS_ProfileSelection_Decision_v1.md), [WN-06](WN-06_SS_ParentMatter_Final_Decision_v1.md), [WN-39](WN-39_SS_OnShellMatch_Decision_v1.md), [WN-37](WN-37_SS_KinkFermionGauge_ParentGate_v1.md), [WN-38](WN-38_SS_FullFiniteAmplitude_ParentGate_v1.md); all remain noncanonical, and their earlier tree-level gap should not be assigned to the new covariant bulk.
- DeWolfe, O., Freedman, D. Z., Gubser, S. S., and Karch, A., “Modeling the fifth dimension with scalars and gravity,” *Phys. Rev. D* 62, 046008 (2000), DOI: https://doi.org/10.1103/PhysRevD.62.046008. Relevant established first-order wall method and tensor factorization; verified publisher abstract/metadata.
- Zhao, Z.-H. and Xie, Q.-Y., “Localization of U(1) gauge vector field on flat branes with five-dimension (asymptotic) AdS5 spacetime,” *JHEP* 05, 072 (2018), DOI: https://doi.org/10.1007/JHEP05(2018)072. Example established nonminimal gauge-localization mechanisms, not proof of our action's loop protection.
- Vaquera-Araujo, C. A. and Corradini, O., “Localization of abelian gauge fields on thick branes,” *Eur. Phys. J. C* 75, 48 (2015), DOI: https://doi.org/10.1140/epjc/s10052-014-3251-2. Independent comparator for nonminimal vector localization.

**Verification:** `SS_Parent5D_check_v1.py` (not included) reconstructs and checks the Einstein components, scalar EOM, first-order superpotential, canonical-X no-go, normalized fermion/gauge source identity, constant-mass mismatch, transverse common potential and uniform counterterm divergence using exact SymPy identities. No numerical fit or external solver is required.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-MAT v1** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MAT: Scale-Extended Matter Sources: Protected Matching, Scale Transport and Completion Gates* (version 1). Zenodo. [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555). Published; current version.

Other working notes referred to by label:

- P24: [WN-26](WN-26_P24ScaleKinkWeight.md)

Material named in this note but not included in this release: `SS-DYN_leafwise_dynamical_closure_v8.tex`, `SS_Parent5D_check_v1.py`.
