> **Public edition of evidence note WN-33.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P27PhotonWarpWeight.md`. Not peer reviewed.
> - **Source content hash:** `0febe637835d64b138a31c16a6604c19a7ec857a53cdaa62fddc0b51bace98b5` (3752 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# P27 — Photon on the DYN warp weight: closure survives to about 10⁻⁴ (9 Nov 2026)

Status: unreviewed AI calculation, noncanonical. Done at the author's request (9 Nov 17:53Z, "Test it", on the P26 follow-up). Builds on [WN-32](WN-32_P26ChargeExtentOnKink.md). No canonical file changed. Scripts (not included in this release): c40a_sym.py, c40b_response.py, c40c_odd_and_checks.py, c40d_Dcheck.py; output: c40_out.txt.

## Question

P26 found exact closure of the lowest scale level when the photon shares the matter weight (sech⁴). In the DYN parent the photon more naturally carries the warp e^A = sech² (P24). Does closure survive?

## Setup

Matter weight F = sech⁴κy, Maxwell weight g = sech²κy, everything else as P26. Work in the long-wavelength limit (droplet larger than 1/κ). Split A₀ into the photon zero mode (the long-range field) and a y-dependent remainder, which obeys

  −∂_y(g ∂_yφ₁) = (q n/ε₄)(F − g W₀/G₀),  W₀ = 4/(3κ), G₀ = 2/κ.

## Results

1. **Long-range Coulomb survives exactly.** The photon's zero mode is normalizable (∫g = 2/κ). Its Liouville potential is κ²(1 − 2sech²), Pöschl–Teller ℓ = 1, so there is only the zero mode, with a continuum from κ. The 3D law stays 1/r with ε₃ = ε₄G₀ (P26 had ε₄W₀). (c40a)

2. **The mismatch field has a closed form.** φ₁ = −(q n/3ε₄κ²) ln cosh κy, up to a constant (c40a, exact). It is even, so it does not force the odd matter level (sinh κy) at all. It forces only the even continuum, above 2κ.

3. **Off-level fraction is tiny.** Define η = (q²n/ε₄κ²)/(ħ²κ²/2m), the local Coulomb energy against the level unit, and λ = 2nU″(n)/(ħ²κ²/2m), the matter stiffness. Then the static off-level fraction is T = η² D(λ):

| λ | D(λ) |
|---|---|
| 0 | 1.9×10⁻⁴ |
| 1 | 1.3×10⁻⁴ |
| 8 | 2.6×10⁻⁵ |

   Grid and box converged to 10⁻⁴ relative (c40d). The full self-consistent nonlinear solution, with Coulomb feedback, agrees with the linear formula to 0.1% at η = 0.01 and is 20% below it at η = 3. T ≤ 10⁻³ for η ≤ 3 (c40b).

4. **Main physical effect is a contact term, not leakage.** The y-structure stores field energy (q²/2ε₄)(2/27κ³)n², a repulsive contact interaction of range about 1/κ. In the 3D theory it renormalizes the cubic coupling: β → β − q²/(36ε₄κ²) (c40a: ∫gΦ′² = 2/27, exact).

5. **The odd threshold moves the safe way.** To first order the odd level shifts by Δe₁ = (−1/6 + 4/9)η = +(5/18)η, in units ħ²κ²/2m. Here −1/6 comes from the mismatch potential and +4/9 from transverse Coulomb exchange. For comparison, the matched P26 case gives +(2/3)η. Charge still raises the holding margin, e₁ + Δe₁ > |λ_min| (c40c, box-converged).

## At ChargeExtent's own parameters

These are ħ = m = ε₄ = 1, q² = 1.6π², β = 16π², γ = 9π⁴, at saturation density.

| κ | η | Off-level fraction (self-consistent) | Δβ/β |
|---|---|---|---|
| 1.7 | 0.34 | ≈ 8×10⁻⁷ (linear) | 0.1% |
| 1.0 | 2.84 | 8.7×10⁻⁶ | 0.3% |
| 0.5 | 45.5 | 1.4×10⁻⁴ | 1.1% |

At κ = 0.5 the first-order odd shift (+4.2 e₁) is outside its validity.

## Verdict

P26's closure survives in the DYN parent. It is no longer exact, but it holds to about 10⁻⁴ or better across the held range. The mismatch's real content is a small repulsive contact term that shifts β by 1% or less. The 1/r Coulomb law and the odd-level protection are unchanged.

## Open

- Finite droplets (scale near 1/κ), where the long-wavelength split fails, were not solved.
- The odd-threshold shift is first order only (large η untested).
- Classical only.
- The far region and the global energetics remain open, as in P24 and P26.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.

Other working notes referred to by label:

- P24: [WN-26](WN-26_P24ScaleKinkWeight.md)
- P26: [WN-32](WN-32_P26ChargeExtentOnKink.md)
