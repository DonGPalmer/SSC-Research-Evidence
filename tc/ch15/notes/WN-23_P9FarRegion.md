> **Public edition of evidence note WN-23.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P9FarRegion.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `aa66748c676e7bcb3753e810c4b5679c3e00efcf5a66b7412c772a77e920963b` (5823 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# P9. Does the far region reach the localized level?

WS1 working note, 8 November 2026. Draft for the author. Working material only: not reviewed, nothing published.
Follows [WN-22](WN-22_P8CutoffBox.md) (§4, reading 3). Script: `c18_far_region.py`, which needs `c17_cutoff_fold_box.py` in the same folder. Output: `c18_out.txt`. These files are not included in this release.

## 1. Question
P8 found that the parent's cubic Galileon coefficient Ĉ3 grows like e^(2Y) with the box size Y, and that the growth comes from the far region where F → 0. P8 left three readings open. This note tests the third: the far region is strongly coupled but does not reach physics at the localized level.

## 2. Result
1. **The cubic vertex is local along the scale axis.**
   - A centre mode (|y| < 3) and far modes (5 < |y| < 11) with separate supports have cubic couplings T(a,b,c), T(a,a,b), T(a,b,b) of 10⁻¹⁸ to 10⁻³⁷, i.e. zero.
   - The cubic couplings within each group are C3[a] = −0.54 and C3[b] = 3×10⁶.
   - Reason: the constrained response of a Q-orthogonal profile carries no flux past the edge of its own support.
2. **Fields driven from the centre see the far region only near the heavy threshold.**
   - A source at the centre, at energy E, drives a field whose tail falls like e^(−√(4−λ) y), with λ = rE²/κ².
   - Its cubic coefficient therefore converges in Y when 3√(4−λ) > 2, i.e. λ < 32/9. That is E < 0.943 M⊥, where M⊥ = 2κ/√r is the scalar heavy threshold.
   - Numerically, C3 for the driven field at Y = 8, 12, 16, 20:
     - λ = 0: 29.2 at every Y.
     - λ = 3.0 (E = 0.87 M⊥): 102 → 103.6, converged.
     - λ = 3.4 (0.92 M⊥): 223 → 301, converging.
     - λ = 3.7 (0.96 M⊥): 760 → 7×10⁴, diverging.
     - λ = 3.9: up to 7×10⁸.
   - Up to λ = 3.0, more than 80% of the coupling comes from |y| < 4. At λ = 3.4 the share beyond |y| = 4 is already 57%, though it still converges. Above the threshold, the far region dominates entirely.
3. **The matter zero modes are insulated.** These are gauge-type F-weighted modes, checked as the l = 2 Pöschl–Teller problem in boxes Y = 8, 12, 16.
   - The zero–continuum–continuum overlap is universal: 0.866 = (4/3)^(−1/2) at every Y. Off-diagonal it is zero.
   - The zero–zero–continuum overlap stays small and falls with box normalization.
   - Continuum–continuum–continuum grows with the box: 4×10⁻¹⁰, 6×10⁻⁶, 8×10⁻³. This is the same far-region growth.
4. **Not covered:** couplings with a Q leg. The gate's formula covers only Q-orthogonal directions. The Q profile is centre-localized (falling like e^(−2y)), so locality suggests it is insulated too, but this was not computed.

## 3. What it means
- **Reading 3 holds below the threshold.** In the localizer sector, physics at the localized level below about 0.94 M⊥ does not see the far region. There the effective Galileon coefficient is box-independent and small: 29 to 300, against the box value 4×10⁴ at Y = 8.
- **This removes P8's box sensitivity for low-energy statements:**
  - SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)'s long-range results (the Q pole, α_Q, the valley theory of D3b) are claims below M⊥, and they stand for any box.
  - DYN's window condition, "the cutoff stays above the first scalar continuum level", should be restated as: the theory at the localized level is weakly coupled up to about 0.94 M⊥. What happens at and above M⊥ depends on the far region.
- **TeV window, indicative only.** It uses P5's convention, rescaled with the driven-field coefficient instead of the box coefficient.
  - With the coefficient at 0.92 M⊥, the top moves from 11.35 TeV (box, Y = 8) to about 1.5×10³ TeV, independent of the box.
  - With the coefficient at zero energy, it moves to about 1.6×10⁴ TeV.
  - The lower edge (0.55–0.75 TeV under the fold) is unchanged.
  - So the TeV option is no longer squeezed by the box. Its top is set by physics near M⊥, which needs the far region.
- **What still needs the far region:**
  - localizer physics within about 6% of M⊥ and above it;
  - matter continuum states interacting with each other, i.e. any process with more than one continuum state in flight.
- For matter under the fold, the continuum starts at 2c_iκ. Single continuum production and exchange from zero modes are insulated. What produced continuum states do afterwards, once they move out along the scale axis, is not specified by the theory.

## 4. Status
- The far-region question is now narrower. The theory at the localized level is closed below about 0.94 M⊥ (localizer) and for zero-mode processes with at most one continuum leg per vertex (matter).
- A statement about the far region is needed only for high-energy and continuum-rescattering physics.
- Readings 1 (scale space ends) and 2 (F has a floor) remain options for that regime. They are no longer needed for the low-energy claims.

## 5. Limits
- AI computation, not reviewed.
- Tree level, probe limit, regulator rebuilt from the null-sector gate's description (c17).
- One source profile (tanh sech⁴, projected off Q). The threshold 32/9 follows from the tail law and does not depend on the source shape.
- The matter check uses only the lowest even continuum states in each box.
- Q-leg couplings not computed. Loops not considered.
- The P5 rescaling is a convention transfer, not a new cutoff derivation.

## 6. Proposal only
If confirmed:
- SS-DYN's EFT-window wording and the 8.10 keV figure could be restated as "weakly coupled at the localized level up to about 0.94 M⊥; box-dependent above".
- P5's window top should be marked as superseded by this note.

## 7. Files
- This note. Script `c18_far_region.py` (needs `c17_cutoff_fold_box.py`) and output `c18_out.txt` (not included in this release).

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.

Other working notes referred to by label:

- P5: [WN-24](WN-24_P5CommonScale.md)
- P8: [WN-22](WN-22_P8CutoffBox.md)
