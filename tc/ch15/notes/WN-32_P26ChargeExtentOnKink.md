> **Public edition of evidence note WN-32.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P26ChargeExtentOnKink.md`. Not peer reviewed.
> - **Source content hash:** `f120196ede79e0063c1f19a1c1a760ac9f56eb4a8442972815f77ffbadb71453` (6485 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** Its statement that charge only helps is qualified in [WN-34](WN-34_P28ChargedDropletKinkSize.md). An editorial note marks the affected passage; the original wording is kept.

# P26 — ChargeExtent matter on the DYN kink: exact closure and a sharp scale-holding threshold (9 Nov 2026)

Status: unreviewed AI calculation, noncanonical. Done at the author's request (9 Nov 17:27Z, "Yes" to the P25 proposal). No canonical file was changed; the ChargeExtent note `SS_ChargeExtent_v1.md` (not included) was read only. Scripts (not included in this release): c39a_sym.py, c39b_droplets.py, c39c_flow2d.py, c39d_threshold.py; output: c39_out.txt.

## Setup

Take the ChargeExtent action unchanged in form (Schrödinger kinetic term, U(n) = −βn² + γn³, Maxwell with Z = 1 on the same volume form), but replace its scale direction (homogeneous H4, weight a e^{3u}) by the DYN/P24 kink: flat x ∈ R³, scale coordinate y, one common weight F(y) = sech⁴(κy) on the matter kinetic and potential terms and on the Maxwell term. This is the P24 reading (matter weight = localizer gradient energy density). The Maxwell weight is a modelling choice transplanted from ChargeExtent's Z = 1 convention.

Transverse operator: K = −(ħ²/2m) F⁻¹∂_y(F∂_y). Liouville form −χ″ + κ²(4 − 6 sech²κy)χ (c39a, exact). Levels: ψ₀ = const (energy 0, normalizable, ∫F = W₀ = 4/(3κ)); ψ₁ = sinh κy (odd, e₁ = 3ħ²κ²/2m); even continuum from 2ħ²κ²/m.

Contrast: on ChargeExtent's H4 the u-constant mode is not normalizable and the u-spectrum is pure continuum from E_c = 9ħ²/(8ma²). There is no lowest level to hold matter, which is why their leakage bounds are finite-time only.

## Result 1 — exact closure of the lowest level

Because the nonlinearity is pointwise and the weight is common, a y-independent ψ(x,t) stays y-independent under the full nonlinear evolution. With the common Maxwell weight, Gauss's law −∇·(F∇A₀) = qnF is solved exactly by a y-independent A₀ (c39a). So the lowest level is an exact invariant sector, neutral or charged. On it the model is ordinary 3D gauged cubic–quintic NLS:

- β_eff = β/W₀, γ_eff = γ/W₀², so β_eff²/γ_eff = β²/γ (W₀ drops out)
- 3D Maxwell with ε₃ = ε₄W₀: exact 1/r Coulomb for y-uniform sources

The zero-mode photon is normalizable on the kink. This removes the obstacle ChargeExtent states ("a constant photon profile is not normalizable on the noncompact scale line").

## Result 2 — sharp threshold for holding matter in scale

Linearise about a stationary 3D droplet ψ_D (chemical potential μ < 0). Transverse modes decouple level by level. Each sees the same 3D operators shifted by its level energy: L₊ + e_k (real part) and L₋ + e_k (imaginary part). L₋ ≥ 0, so the droplet stays on the lowest level iff

  e₁ = 3ħ²κ²/(2m) > |λ_min(L₊)|.

The even channel needs 2ħ²κ²/m > |λ_min| and is weaker. λ_min is the droplet's single negative L₊ eigenvalue, the 3D breathing direction.

- **Analytic sufficient bound, any localized droplet:** U′ + 2nU″ = −6βn + 15γn² ≥ −(3/5)β²/γ, and μ < 0. So κξ > √(2/5) ≈ 0.63 always suffices, with ξ = ħ/√(mβ²/γ) the matter healing length.
- **Sharp values (c39b; Newton-converged, residual 5×10⁻¹⁴, translation mode at 10⁻⁵):**

| Reduced content Ñ | 40 | 60 | 100 | 200 | 400 | 1000 |
|---|---|---|---|---|---|---|
| λ_min (units β²/γ) | −0.158 | −0.108 | −0.072 | −0.044 | −0.028 | −0.015 |
| κ_c ξ | 0.325 | 0.269 | 0.219 | 0.171 | 0.136 | 0.100 |

  Larger droplets are held more easily (λ_min → 0⁻ as μ → μ_sat = −β²/4γ). dN/dμ < 0 on this branch, so the 3D droplets are Vakhitov–Kolokolov stable.

**Full (r, y) check without the linear reduction (c39c, c39d; Ñ = 100, prediction κ_c ξ = 0.219 odd, 0.190 even):**

| κξ | Seed | Final off-level fraction T |
|---|---|---|
| 0.32 | odd or even | 3×10⁻²⁷ (exact return) |
| 0.23 | odd | 5×10⁻¹⁴, decaying |
| 0.21 | odd | 0.32; matter shifts to ⟨κy⟩ = +0.62 |
| 0.20 | even | 9×10⁻¹¹ |
| 0.18 | even | grows |
| 0.15 | odd / even | 0.87 / 0.85; ⟨κy⟩ ≈ ±1.3 |

Both thresholds are bracketed as predicted. Below threshold the scale offset grows continuously (a pitchfork): matter slides to one side of the kink centre rather than escaping. No runaway to the box edge (κ|y| = 5) was seen.

## Result 3 — time-uniform leakage bound

Above threshold, the second variation of E − μN splits into a lowest-level block and transverse blocks with no cross terms at quadratic order. The transverse block is coercive with gap g = e₁ − |λ_min|. Since E − μN is conserved,

  ‖P_⊥ψ(t)‖² ≤ [ (E − μN)(ψ(0)) − (E − μN)(ψ_D) ] / g  for all t,

to quadratic order and modulo the droplet's symmetries. This replaces ChargeExtent's finite-time projector bound, which was valid only to τ ≈ 0.01. It also gives doc 5's energy defect Δ a fixed physical scale: the kink gap.

> **Editorial note (public edition, 19 November 2026):** A later note, which solves charged droplets numerically with the SS-DYN photon weight, finds that charge does not destabilize a droplet held above the scale-holding threshold and moves the threshold slightly the safe way, but that below the threshold charge pushes the off-centre states further off-centre, and near the threshold the even leak grows to about 10⁻². See [WN-34](WN-34_P28ChargedDropletKinkSize.md) Result 6. The text below is unchanged from the working note.

Charge only helps. Transverse photon modes have the same spectrum: massive, √3κ odd and from 2κ even. In the transverse channel Coulomb is Yukawa-screened and adds a positive operator to the L₊ block. Charged droplets were not solved numerically.

## Reading (proposal, not established)

One dimensionless number, κξ (kink width against matter healing length), decides which mechanism sets matter's scale extent:

- **κξ above threshold:** the kink holds matter on its lowest level. The scale profile is the protected sech⁴ envelope, exactly, and the 3D physics closes with ordinary Coulomb.
- **Below threshold:** the matter's own binding wins and it sits off-centre in scale. This is the ChargeExtent self-localized regime.

This matches ChargeExtent's own numbers. Their β²/γ = 256/9 gives ξ = 3/16. Their flat-R⁴ and H4 (a = 10) energies differ by only 0.4%: geometry is irrelevant when nothing confines. On a kink, their matter would be held for κ ≳ 0.5–1.7 (their units, depending on the content Ñ, not mapped). This is the first concrete link between ChargeExtent and SS-MAT v1 [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555)'s sech⁴ envelope, which their note says was never matched.

## Open

- Maxwell weight ≠ matter weight, e.g. the P24 warp e^A = sech²: closure then breaks by a static even polarization (the odd level is protected by parity). Not computed.
- Global energetics and the far region (κ|y| ≫ 1) are not settled. This is the same open item as P24's far-region and leakage question.
- Charged droplets were not solved.
- The map from Ñ to ChargeExtent's N = 1 content is not done.
- All results are classical (no loops).

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-MAT v1**: D. G. Palmer (2026). *SS-MAT: Scale-Extended Matter Sources: Protected Matching, Scale Transport and Completion Gates* (version 1). Zenodo. [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555). Published; current version.

Other working notes referred to by label:

- P24: [WN-26](WN-26_P24ScaleKinkWeight.md)
- P25: not included in this release.
