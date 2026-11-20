> **Public edition of evidence note WN-40.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `SS_ProfileSelection_Decision_v1.md`, a working note dated 9 November 2026. Not peer reviewed.
> - **Source content hash:** `9e6bbd9f6a1ff8e60de89f17526605f46376a13d19c4862dc3f52abe4d8ee7be` (15671 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# SS physical-scale profile selection from a common kink parent

**Date:** 9 November 2026  
**Status:** Noncanonical analytical development, independent numerical checks. No changes to the canonical papers.  
**Decision:** PASS for the parent localizer's **translational collective-mode profile**; PASS for a necessary-and-sufficient **linear protected-source alignment criterion**; HOLD for universal identification of these modes with every material species or every object's physical SS extent.

## Scope and prior work

The live SS-DYN v8 [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) kink has localizer profile `X_0(y)=v tanh(kappa y)` and the protected gravitational weight `F(y)=sech^4(kappa y)`. WS1 [WN-26](WN-26_P24ScaleKinkWeight.md) noticed that `F` is the localizer BPS-gradient energy density and proposed equating matter weighting to this density; [WN-32](WN-32_P26ChargeExtentOnKink.md) derives an exact lowest profile sector if the same weight is imposed on the coherent matter action; `P27`/`P28` assess differing photon weights and charged droplets. [WN-04](WN-04_P2Parent.md) uses per-leaf copies of matter with matching weights; the noncanonical [WN-06](WN-06_SS_ParentMatter_Final_Decision_v1.md) finds that universal protected source weighting remains an extra premise and loop protection is open. The new contribution here is a precise **defect collective-mode** source for `F`, its intrinsic width and the **complete heavy-mode coupling identity** which states the selection condition without fitting a profile. These are conventional soliton/weighted-mode tools applied to this particular SS candidate, not a unique discovery of these techniques.

## 1. The localizer selects its own extended collective excitation

Take an ordinary Lorentz-invariant scalar kink model in a prescribed flat auxiliary product geometry, with an independent transverse real coordinate `y` and one time/three-space worldvolume:

\[
S_X=\int d^4x\,dy\left[-\frac12\partial_A X\partial^A X-\frac12\left(W'(X)\right)^2\right],\qquad
W'(X)=\kappa v\left(1-\frac{X^2}{v^2}\right).
\]

The static BPS equation `X_0'=W'(X_0)` has solution

\[
X_0(y)=v\tanh(\kappa y),\quad X_0'(y)=\kappa v\operatorname{sech}^2(\kappa y).
\]

The translational Goldstone fluctuation is obtained **by differentiating a family of exact translated backgrounds**, not by guessing a matter profile:

\[
X(x,y)=X_0(y-Y(x)),\qquad \delta X=-X_0'(y)Y(x)+O(Y^2).
\]

To quadratic order in worldvolume derivatives, its inherited action is

\[
S_{\rm coll}= -T_{\rm wall}\int d^4x-\frac{T_{\rm wall}}2\int d^4x\,\partial_\mu Y\partial^\mu Y+\cdots,
\quad T_{\rm wall}=\int dy\,(X_0')^2=\frac{4\kappa v^2}{3}.
\]

The displayed kinetic sign uses signature (-+++). The normalized transverse wavefunction and physical energy-density profile are

\[
f_0(y)=\frac{X_0'}{\sqrt{T_{\rm wall}}},\qquad
P_0(y)=|f_0(y)|^2=\frac{3\kappa}{4}\operatorname{sech}^4(\kappa y).
\]

Thus the *same localizer action* fixes a finite distribution in the transverse coordinate, its normalization, and the collective inertia/tension. Its exact mean is zero and variance is

\[
\boxed{\operatorname{Var}_{P_0}(y)=\frac{\pi^2-6}{12\kappa^2},\qquad \sigma_y=0.5678618084/\kappa.}
\]

This is a genuinely extended **field excitation** across the transverse coordinate; it is not an ensemble of different macroscopic objects, nor a proof that the position collective coordinate `Y` is itself sharply localized quantum mechanically. The translational mode is massless in the exact translation-symmetric parent; pinning, gravity, boundaries and nonlinear backreaction can change it. If `y` is to be the physical logarithmic scale `u`, a metric-and-dynamics identification must be shown, rather than presumed. The SS-DYN localizer also need not literally have this flat-worldvolume Lorentz-invariant action, so this is a conditional parent realization aligned with its BPS profile.

## 2. An exact uniqueness and leakage theorem for protected matter weights

Consider the linearized tensor-mode Hilbert space `H=L^2(F dy)` with the protected normalized light mode `v_0=1/sqrt(W_0)`, `W_0=int F dy=4/(3kappa)`. Let `{v_0,v_a}` denote a complete generalized mode expansion, including discrete and continuum modes (or the corresponding spectral projector). Let a matter source couple to the metric modes with a real/nonnegative source weight `Z(y)` via `int dy Z(y) v(y) T(x)` and suppose `Z/sqrt(F)` is square-integrable. Its mode couplings are

\[
g_a=\int Z(y)v_a(y)\,dy
=\langle Z/F,v_a\rangle_F,\qquad
g_0=\frac{\int Z\,dy}{\sqrt{W_0}}.
\]

Parseval's identity (with the complete heavy spectral subspace) gives exactly

\[
\boxed{\sum_{a\ne0}|g_a|^2
=\int\frac{Z^2}{F}\,dy-\frac{(\int Z\,dy)^2}{W_0}
=W_0\operatorname{Var}_{F/W_0}(Z/F)\ge0.}
\]

**Necessary and sufficient selection criterion:** all direct overlaps with the complete heavy subspace vanish if and only if `Z/F` is constant almost everywhere; equivalently `Z=c F` with one overall normalization. This is an exact statement in the declared complete-mode, aligned-source model. It does not prove the absence of nonlinear, loop-induced, derivative, electromagnetic or nonuniversal interactions, or by itself establish constraint closure of a gravitational parent. If `Z` is not in the Hilbert-space dual domain, the heavy norm may diverge and the formula cannot be treated as a finite physical coupling.

For a controlled illustrative one-parameter family `Z_p(y)=sech^(2p)(kappa y)`, `p>1`, define `I(q)=int_{-infty}^{infty} sech^q z dz=sqrt(pi) Gamma(q/2)/Gamma((q+1)/2)`. The normalized heavy-to-light squared-coupling ratio is

\[
\boxed{R(p)=\frac{W_0\int Z_p^2/F\,dy}{(\int Z_p\,dy)^2}-1
=\frac{I(4)I(4p-4)}{I(2p)^2}-1.}
\]

It vanishes only at `p=2`. This result both explains why the preferred profile is exceptional for **linear universal matter sourcing** and quantifies what a mismatch does. The scale of `g_0` and any physical Yukawa strength additionally require the actual parent normalization, tensor projectors, masses and measurement map; `R` is not an experimental gravity limit.

| p | Heavy/light coupling norm squared R(p) |
|---:|---:|
| 1.25 | 0.3708397431 |
| 1.50 | 0.0807592922 |
| 1.75 | 0.0131664885 |
| 2.00 | 0 (protected) |
| 2.25 | 0.0075672112 |
| 2.50 | 0.0247199215 |
| 3.00 | 0.0714285714 |

For small mismatch `Z=F(1+epsilon h)`, the exact heavy squared norm is `epsilon^2 W_0 Var_F(h)`; its ratio to the light coupling is `epsilon^2 Var_F(h)/(1+epsilon E_F h)^2`. Thus the heavy **amplitude** is first-order in mismatch while its squared coupling is second-order, unless further selection rules suppress it. Parity only removes odd modes for even `Z`; it does not force `R=0` because even heavy continuum modes remain.

## 3. A conditional coupled-parent mechanism also selects a fermion profile

A more demanding version of the question is whether `F` can be inherited by a **distinct matter field**, not merely by the localizer's own Goldstone mode. There is a constructive example within a lower-dimensional supersymmetric Wess–Zumino-type kink parent. Take one real scalar `X` and a spinor whose Yukawa mass is **not independent** but is the superpotential derivative `m_f(X)=W''(X)=-2 kappa X/v`. (The spinor action and its transformations must be those of the stated supersymmetric parent, not an arbitrarily selected Yukawa in a generic 5D theory.) The 1D transverse first-order operator for one chirality is

\[
Q=\partial_y-W''(X_0(y))=\partial_y+2\kappa\tanh(\kappa y).
\]

Differentiating the localizer BPS equation `X_0'=W'(X_0)` gives `X_0''=W''(X_0)X_0'`, hence

\[
\boxed{Q X_0'=0,\qquad f_{\rm fermion,0}(y)=\sqrt{3\kappa/4}\,\operatorname{sech}^{2}(\kappa y).}
\]

The localizer fluctuation Hessian is exactly its supersymmetric quantum-mechanics partner

\[
Q^\dagger Q=-\partial_y^2+4\kappa^2-6\kappa^2\operatorname{sech}^2(\kappa y).
\]

Thus, with the usual flat transverse fermionic norm, **both** the wall's translational collective mode and a protected chiral fermion have normalized density `3 kappa sech^4(kappa y)/4`, and both are pinned to the *same* `W`, rather than to separately fitted localization profiles. This gives a concrete conditional **common-parent mechanism for species-profile inheritance**. The relation is familiar from supersymmetric kink physics; its embedding in SS would be new programme work, not a novel theorem about solitons.

It matters that a bosonic localizer translation mode and a fermionic zero mode have different 4D spin and dynamics: matching their transverse probability/kinetic profiles does **not** make them the same particle. Further, the existence of a BPS factorization `Q^dagger Q` by itself does **not** establish a quantum supersymmetry of the whole action. A true 4+1-dimensional SS implementation would need consistent multiplets, transformations, gravity and gauge coupling, boundary data, and anomaly/loop checks. Without those, the superpotential-linked fermion Yukawa is an **extra coupled-parent assumption**—albeit more economical and mechanically motivated than setting `Z=F` separately for every species.

## 4. What complex matter contributes—and what it cannot select

An object can have a nonzero profile across real `u` while its matter amplitude is complex. For a coherent matter field `Psi=R e^(i theta)` with transverse kinetic density `F |d_y Psi|^2`,

\[
F|\partial_y\Psi|^2=F[(\partial_yR)^2+R^2(\partial_y\theta)^2],\quad
j_y\propto F R^2\partial_y\theta.
\]

On a connected transverse line and with no background gauge connection, the zero-cost transverse state has constant modulus and constant phase, so its **normalized physical density** inherits `F/W_0`. A phase twist has positive energy and can have scale current without changing its instantaneous density profile. Complex values are therefore indispensable when describing phase, interference, quantum currents, charged fields and their reductions, but merely changing from real to complex amplitudes does not determine the profile `F` or create another real dimension. `SS_ComplexConnection_v1.md` (not included) correctly distinguishes this from complexifying `u`, which would alter the metric and its signature.

Complex internal channels can make the situation more interesting: coupled matrices, index-protected zero modes, relative phases, and Berry connections may select a particular *mode vector*. But without a specified coupling to `X` and a protected normalization, they do not force every matter species to have `Z=F`. The previously considered chiral wall zero mode has `f_0~sech^2` for a tuned Yukawa/operator relation; its squared norm matches `F`, while its exponent depends on the Yukawa coupling. This is another **conditional mechanism**, not universal protection.

## 5. Constructive limitation: why one matter weight is not yet selected for all objects

The localizer action fixes `X_0` and its own zero-mode density, but a separate conventional matter scalar `phi` can be coupled through `-Z(X)|partial_mu phi|^2/2` with any smooth, positive, normalizable `Z_p(X)=(1-X^2/v^2)^p` in the allowed domain (`p>1` for a finite complete-source norm). These actions have the *same* localizer kink in the test-field limit, positive local kinetic energy, and different physical profiles. Nothing in the kink BPS equation forbids them. A common source-alignment requirement **singles out** `p=2` but is an additional physical principle imposed on matter couplings; it is not obtained solely by extremizing the localizer's action. The requirement's status is logically different from the genuinely derived translational collective mode.

Likewise, `P26` obtains exact scale-flat coherent-field closure once all its kinetic/potential weights are made common, but that assumption cannot be exported unchanged to generic Dirac, gauge, polymer, thermal or biological constituents. Gauge-field and fermion localization can have different kinetic normalization; effective interactions and loop thresholds may spoil alignment. A blanket statement that *every object* is the wall's translational zero mode would confuse distinct dynamical objects. An object may possess a finite scale profile with material-dependent shape while being governed by a common parent law; universal shape is not implied by the programme's finite-extent postulate.

## 6. Decision and bounded next gate

**PASS A**: One BPS localizer action gives its own normalizable extended collective-mode probability/energy profile `3 kappa sech^4(kappa y)/4`, unique within its translational zero-mode sector; the normalized width and tension follow without empirical fitting.

**PASS B**: A superpotential-linked fermion in a restricted supersymmetric kink parent shares the translational mode’s exact `sech^4` transverse probability weight; this is conditional on the full shared interaction rather than solely on the BPS solution. With a full common-weight tensor eigenbasis, vanishing direct massive-mode source leakage forces and is forced by `Z proportional to F`; the complete heavy coupling norm is exactly `W_0 Var_F(Z/F)`.

**HOLD C**: The localizer mode is not demonstrated to be every matter species' intrinsic scale extent; no derivation yet equates the kink coordinate and homogeneous SS-GEO [v6, doi:10.5281/zenodo.23603029](https://doi.org/10.5281/zenodo.23603029) `u`; protected linear matter weights are not proven stable under radiative corrections and nonlinear parent constraints.

**HOLD D**: Complex internal amplitudes can encode a finite extended profile, dynamic scale phase/current and non-Abelian mixing, but do not alone yield a new matter-weight-selection principle. Do not identify imaginary components of the complex amplitudes with extra physical scale coordinates without a separately specified metric and observables.

**Next strict development gate**: Select one already-identified species (the WS1 chiral fermion or a localizer-bound scalar), derive its exact `Z(X)`/wavefunction from a single *specified* coupled parent under the same gauge and gravity normalizations, and evaluate the spectral overlap/threshold after integrating heavy modes. Require independent proof of quantum/radiative protection or label it classical only. Prefer the smallest field content and one hard selected regulator. If alignment is restored by tuning a free Yukawa coupling, classify this as *conditional matching*, not an explanation for universal weighting. A second alternative is to derive a symmetry (e.g., genuine supersymmetry with complete transformations and Ward identities) that forces the desired relation. Do not assume it merely because the kink admits BPS equations.

## Verification and scope

Accompanying `verify.py` (not included) and `results.json` (not included) evaluate the BPS zero-mode and factorized transverse Hessian symbolically, Gamma-function integrals, a finite-domain quadrature cross-check (including non-negligible tails for broad `Z`), the wall tension, the heavy-source norm, and the positive phase-gradient energy. The maximum absolute numerical mismatch in the tested heavy-coupling ratio is below `5e-10`; the wall-tension quadrature residual is below `1e-15`. These verify the derived mathematical formulas, not the full nonlinear coupled parent, external observations, or the gravitational tensor-sector constraints.

**Provenance:** `SS-DYN_leafwise_dynamical_closure_v8.tex` (LaTeX source of SS-DYN v8; not included); the P2, P24, P26, P27 and P28 working notes; `SS_ComplexConnection_v1.md` (not included), [WN-06](WN-06_SS_ParentMatter_Final_Decision_v1.md), `SS_ChargeExtent_v1.md` (not included), `SS_ProfileTransportBridge_v1.md` (not included). No author adoption is implied.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8**: D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-GEO v6** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-GEO: Logarithmic Scale as a Geometric Coordinate: Exact-Distance Projection and Radial Scale Response* (version 6). Zenodo. [doi:10.5281/zenodo.23603029](https://doi.org/10.5281/zenodo.23603029). Published; current version.

Other working notes referred to by label:

- P2: [WN-04](WN-04_P2Parent.md)
- P24: [WN-26](WN-26_P24ScaleKinkWeight.md)
- P26: [WN-32](WN-32_P26ChargeExtentOnKink.md)
- P27: [WN-33](WN-33_P27PhotonWarpWeight.md)
- P28: [WN-34](WN-34_P28ChargedDropletKinkSize.md)

Material named in this note but not included in this release: `SS-DYN_leafwise_dynamical_closure_v8.tex`, `SS_ChargeExtent_v1.md`, `SS_ComplexConnection_v1.md`, `SS_ProfileTransportBridge_v1.md`, `results.json`, `verify.py`.
