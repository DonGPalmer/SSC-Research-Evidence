> **Public edition of evidence note WN-34.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P28ChargedDropletKinkSize.md`. Not peer reviewed.
> - **Source content hash:** `aecfc753aa0af902c5c326c72fcde421192d1539fa6ca5789a9d96e593f11b43` (5268 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# P28 — Charged droplet at the kink's own size: closure holds (9 Nov 2026)

Status: unreviewed AI calculation, noncanonical. Done at the author's request (9 Nov 18:04Z, "Solve it", on the P27 follow-up). Builds on [WN-32](WN-32_P26ChargeExtentOnKink.md) and [WN-33](WN-33_P27PhotonWarpWeight.md). No canonical file changed. Scripts (not included in this release): c41_charged_droplet.py, c41b_threshold.py, c41c_checks.py, c41d_checks2.py, c41e_near.py; output: c41_out.txt.

## Question

P27 showed closure survives the photon-weight mismatch (matter sech⁴, photon sech²) in the long-wavelength limit, where the droplet is much wider than the kink. Does it still hold when the droplet is about as small as the kink width 1/κ, where that split fails?

## Setup

Full self-consistent solve in both directions: 3D radius r (spherical droplet) and scale s = κy, on a grid, with no long-wavelength split.
- Matter: gauged cubic–quintic NLS, kinetic weight F = sech⁴, bare β = W₀, γ = W₀² so the lowest level has β_eff = γ_eff = 1 (ξ = 1, μ_sat = −1/4). N = 100 (droplet rms about 3.5 ξ).
- Photon: Gauss's law −∇·(g∇A₀) = q n F with g = sech² (DYN warp) or g = sech⁴ (matched control). The photon zero mode carries the 1/r tail (u = rA₀ with u′(R) = 0); the massive photon modes are Dirichlet. Solved exactly each step by separable eigen-decomposition.
- Charge strength Q_eff = q²/(ε₄G₀): level densities repel as Q_eff/(4πr). Q_eff = 0.003, 0.01, 0.03. A rough match of Coulomb-to-binding energy per particle puts ChargeExtent's own parameters near Q_eff ≈ 0.015 (the geometries differ, so this is only indicative).
- Kink width swept κ = 1, 0.5, 0.3, 0.25, so κ·rms runs from 3.5 (droplet wider than the kink) to 0.88 (droplet narrower than 1/κ).
- Measured: off-level fraction T = ‖ψ − P₀ψ‖²/N (P₀ = lowest scale level), mean scale position ⟨s⟩, residual.

## Results

1. **Matched control is exact at every size.** With g = F the off-level fraction is 3×10⁻²⁰ (machine zero) for all κ and charges. The solver reproduces P26's exact closure. (c41 main)

2. **With the DYN photon, closure holds at kink size.** Off-level fraction T:

| κ | κ·rms | Q_eff 0.003 | Q_eff 0.01 | Q_eff 0.03 |
|---|---|---|---|---|
| 1.0 | 3.5 | 7.8×10⁻¹⁰ | 8.6×10⁻⁹ | 7.5×10⁻⁸ |
| 0.5 | 1.75 | 9.9×10⁻⁸ | 1.1×10⁻⁶ | 1.0×10⁻⁵ |
| 0.3 | 1.05 | 4.8×10⁻⁶ | 5.5×10⁻⁵ | 5.6×10⁻⁴ |
| 0.25 | 0.88 | 2.6×10⁻⁵ | 3.0×10⁻⁴ | 3.2×10⁻³ |

   T scales as Q_eff² and roughly as κ⁻⁸ (η ∝ κ⁻⁴), as P27 predicted. Neutral droplets have T = 0 exactly.

3. **P27's long-wavelength formula still works at kink size.** The density-weighted local prediction η²D(λ) agrees with the full solve to within a factor 1.6 everywhere (full/formula = 0.62–0.81 for κ ≥ 0.3, 1.0–1.2 at κ = 0.25). The y-structure does not need the droplet to be wide.

4. **Converged.** At κ = 0.3, Q_eff = 0.01: T = 5.518×10⁻⁵; doubling the box (R 16→24, M 160→240) gives 5.519×10⁻⁵, a finer y grid (J 97→129) 5.520×10⁻⁵, double the time step 5.518×10⁻⁵. Edge density 6×10⁻⁸ of peak. (c41c, c41d; c41c's last two checks hit the run time limit and were rerun as c41d.)

5. **No scale shift above the holding threshold.** For κ ≥ 0.22 every charged droplet stays centred, ⟨s⟩ ≤ 10⁻⁹. Only even leakage occurs, consistent with P27 (the mismatch field is even).

6. **Charge and the holding threshold (new, mixed).** P26's neutral threshold is κ_c ≈ 0.219 at this N.
   - At κ = 0.22 and 0.23, Q_eff = 0.03 stays centred, but the even leak grows near the threshold: T = 1.3×10⁻² at κ = 0.22, 7.9×10⁻³ at 0.23.
   - At κ = 0.21, the neutral droplet shifts to ⟨s⟩ = 0.62; with Q_eff = 0.03 it reaches only ⟨s⟩ = 0.05 after 200000 steps and is still moving (not converged). So charge slows or slightly lowers the threshold, the safe direction P27 found.
   - Below the threshold (κ = 0.20, 0.18), the converged off-centre states are pushed further off-centre by charge: ⟨s⟩ = 0.82 → 1.12 at κ = 0.20, 1.12 → 1.28 at κ = 0.18, with μ rising (less bound). Likely reason: off centre, the photon's wider weight gives the field more room, lowering Coulomb energy. This is a reading, not checked.
   - Net: charge does not destabilize a held droplet, but once scale-holding fails, charge makes the failure larger.

## Verdict

The closure holds at the kink's own size. With ChargeExtent-like charge (Q_eff about 0.01–0.03), the leak off the lowest scale level is 6×10⁻⁵ to 6×10⁻⁴ when the droplet is as wide as the kink, and 3×10⁻⁴ to 3×10⁻³ when it is narrower, rising to about 10⁻² right at the scale-holding threshold. P27's simple formula predicts it to within a factor 1.6. The real limit is still P26's scale-holding threshold, not the photon mismatch; charge moves that threshold slightly the safe way but deepens the shift below it.

## Open

- κ = 0.21 charged run not converged; threshold shift with charge not pinned down.
- One N (100) and ξ = 1 only; the mapping of Ñ to ChargeExtent's N = 1 is still open.
- Classical only; no loops. Far region and global energetics remain open, as in P24–P27.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.

Other working notes referred to by label:

- P24: [WN-26](WN-26_P24ScaleKinkWeight.md)
- P26: [WN-32](WN-32_P26ChargeExtentOnKink.md)
- P27: [WN-33](WN-33_P27PhotonWarpWeight.md)
