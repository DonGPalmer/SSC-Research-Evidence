> **Public edition of evidence note WN-22.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P8CutoffBox.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `b25ea2242cbcf23c23503d73cb22f08633f330f0f46444c6e68e45fd409e15ca` (5397 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** Its box limit on the TeV window is lifted in [WN-23](WN-23_P9FarRegion.md). An editorial note marks the affected passage; the original wording is kept.

# P8. The parent cutoff under the fold, and its dependence on the scale box

WS1 working note, 8 November 2026. Draft for the author. Working material only: not reviewed, nothing published.
Follows [WN-17](WN-17_P7FoldRule.md) (§5, check 1). Script: `c17_cutoff_fold_box.py`; output: `c17_out.txt` (not included in this release).

## 1. Question
P7 asked whether the parent-cutoff coefficient Ĉ3 was computed with fold-allowed (P-even) modes only. Ĉ3 matters because it sets the top of the TeV window in P5 (κ ≲ 11.35 TeV).

## 2. Result
1. **The fold does not change Ĉ3.**
   - Ĉ3 = 40469.6 comes from the null-sector gate (P20_NS_gate_v1, 18 August). That gate uses an odd-function localizer profile on a reflection-symmetric chain, which is P-even and kept by the fold.
   - Rebuilt here: the gate's table is reproduced to within 1×10⁻⁴.
   - A P-odd direction alone has zero cubic coupling. The mixed coupling (one P-even and two P-odd legs) is about 1, against 4×10⁴. The fold removes it.
   - So the fold leaves Ĉ3, the 8.10 keV cutoff and the 11.35 TeV top as they were.
2. **New: Ĉ3 is set by the size of the scale box, not by the theory.**
   - The gate fixed the box at |y| ≤ Y = 8 kink widths.
   - At Y = 8, 98.7% of Ĉ3 comes from |y| > 4, 58% from |y| > 6 and 9% from |y| > 7.
   - Ĉ3 grows like e^(2Y)/Y^4.5. The reason is the Fierz–Pauli edge weight, which is proportional to F ~ e^(−4y) and divides the constrained metric response. The same far-region weakness appeared for matter in P6.
> **Editorial note (public edition, 19 November 2026):** A later note finds that couplings driven from the localized level below about 0.94 M⊥ do not depend on the box, so the TeV window is no longer limited by the box size. Rescaled with that box-independent coefficient, the window top moves to about 1.5×10³ TeV, a figure the later note calls indicative only. See [WN-23](WN-23_P9FarRegion.md) §3. The text below is unchanged from the working note.

3. **Consequence for the TeV window.** κ_max is proportional to 1/Ĉ3, so the 11.35 TeV top is the Y = 8 value.
   - At Y = 10 the top falls to 0.55 TeV, which is the lower edge.
   - With the 8.10 keV form, the window closes at Y ≈ 9.8–10.0. D3b showed this is the algebraically correct form.
   - With the 5.62 keV form, it closes at Y ≈ 9.1–9.3.
4. **Consequence for DYN's millimetre benchmark.** The r window survives up to Y ≈ 32 (extrapolated with the far-region law). But the quoted 8.10 keV is also the Y = 8 value: it is 2.96 keV at Y = 10, 1.02 keV at Y = 12 and 0.11 keV at Y = 16.
5. **In the continuum limit** (Y → ∞, DYN's infinite scale line), Λ⊥ → 0 for the softest orthogonal direction. The cutoff is a statement about where the regulator box ends.

## 3. Method
- c17 rebuilds the gate's regulator from its own description:
  - odd D†D localizer stiffness;
  - midpoint weights μ_e = sech⁴(y_e)/Δy and d_e = f(y_e)v_e/Δy, with f = −4 tanh sech²;
  - softest direction with Σ s = 0;
  - normalization ∫v² = 1, Dirichlet at |y| = Y.
- It computes Ĉ3 = Σ d_e ρ_e², with ρ_e taken from exact flux sums along the chain. A pseudo-inverse loses accuracy where μ_e ~ 10⁻¹³; that was found and fixed during this check.
- Reproduction at Y = 8: the null stiffness matches to 10 digits. Ĉ3 matches to 5×10⁻⁷ at J = 20 and 7×10⁻⁵ at J = 320.
- The box scan uses Δy = 0.05 and 0.025 with Richardson extrapolation. The two resolutions agree to about 0.2%.

| Y | Ĉ3 | Ĉ3/Ĉ3(8) | κ_max (8.10 keV form) |
|---|---|---|---|
| 4 | 1.91e2 | 4.7e-3 | 2400 TeV |
| 6 | 2.47e3 | 6.1e-2 | 186 TeV |
| 8 | 4.05e4 | 1 | 11.3 TeV |
| 10 | 8.32e5 | 20.5 | 0.55 TeV |
| 12 | 2.01e7 | 497 | 23 GeV |
| 16 | 1.64e10 | 4.0e5 | 28 MeV |

d ln Ĉ3/dY = 1.28, 1.40, 1.51, 1.59, 1.65, 1.70, against the far-region estimate 2 − 4.5/Y.

## 4. What it means
- **The fold is neutral for the cutoff.** It neither lowers nor raises Λ⊥; it only removes small mixed couplings.
- **The decisive open item is now the far region of the scale axis.** Far from the localized level, both the matter couplings (P6) and the localizer Galileon (here) grow without bound. There are three ways the theory could handle this, none established:
  1. Scale space physically ends, or is cut off, within about 10 kink widths of the localized level for the TeV option, or about 30 for the millimetre benchmark. This needs a stated boundary and a reason for it.
  2. F stops falling and has a floor far from the centre. This changes the action and the tensor continuum, and needs its own check.
  3. The far region is strongly coupled but decouples from physics at the localized level, so only a local cutoff matters. This is not shown. It would need an argument that far-region strong coupling does not feed back into the Q sector or the matter zero modes.
- **The box dependence may be understated.** Ĉ3 is computed for the softest direction, as in the gate. Directions concentrated near the box end couple more strongly.

## 5. Limits
- AI computation, not reviewed.
- g3 and the R3 normalization were taken as printed; only the box was varied.
- The regulator was rebuilt from the gate's description and reproduces its table, but it is not the gate's own code.
- Probe level: no back-reaction, tree level only.
- The physical meaning of Y (how far scale space extends, in kink widths) is not established. Turning Y into a ratio of physical scales needs the λ ↔ ln ℓ normalization, which is not fixed here.

## 6. Proposal only
If confirmed, SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)'s "8.10 keV" and its r window should be stated with the box they assume (Y = 8), and P5's TeV window should be stated as conditional on Y ≲ 10.

## 7. Files
- This note. Script `c17_cutoff_fold_box.py` and output `c17_out.txt` (not included in this release).

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.

Other working notes referred to by label:

- P5: [WN-24](WN-24_P5CommonScale.md)
- P6: [WN-16](WN-16_P6ReflectionFold.md)
- P7: [WN-17](WN-17_P7FoldRule.md)
