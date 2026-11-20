> **Public edition of evidence note WN-24.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P5CommonScale.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `661e2642d36567836f79901f9848238707c31054ce906664d0dd4fc3953d383d` (5790 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** Its 1.155 level spacing is withdrawn in [WN-16](WN-16_P6ReflectionFold.md), and the top of its window is superseded in [WN-23](WN-23_P9FarRegion.md). Editorial notes mark the affected passages; the original wording is kept.

# P5. One common scale for matter partners and gravity

WS1 working note, 8 November 2026. Working material only: not reviewed, nothing published.
Follows [WN-15](WN-15_P4CouplingWeight.md). Script: `c14_common_scale.py`; output: `c14_out.txt` (not included in this release).

## 1. Short answer

> **Editorial note (public edition, 19 November 2026):** A later note supersedes the upper end of this window, which §3 derives from the regulator-box value of the parent cutoff coefficient: with a box-independent coefficient for fields driven from the localized level, the top moves from 11.35 TeV to about 1.5×10³ TeV, a figure that note calls indicative only, and the lower edge is unchanged. See [WN-23](WN-23_P9FarRegion.md) §3. The text below is unchanged from the working note.

- Yes, a window exists. With one common scale κ for all sectors (common scale weight and equal speeds, c_i = c_u = 1), the matter partners are out of current reach and the parent stays self-consistent for roughly
  **0.6 to 0.9 TeV ≲ κ ≲ 4 to 11 TeV**,
  with the repair parameter r moved up from 1e-6 towards its ceiling 2.57e-6.
- This removes the 1e15 to 1e17 stiffness hierarchy of the Paper-20 [retired series; see References] post-R3 note. It does so by moving κ itself about 1e17 times above the legacy 9.9 mm benchmark; it does not explain why κ sits near a TeV.
- The price: every gravity-side prediction moves out of laboratory reach. The Q pole range becomes about 1e-21 m. SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)'s gravity sector then has no tabletop test.
> **Editorial note (public edition, 19 November 2026):** A later note withdraws the 1.155 level spacing and drops the √3 κ partner from the TeV branch: under the scale fold it recommends, these partners do not exist, and the alternative symmetry reading, in which they decay during big-bang nucleosynthesis, is likely excluded, though not confirmed against the published figures. Under the fold, the matter-side signal of the TeV option is a single continuum threshold at 2κ. See [WN-16](WN-16_P6ReflectionFold.md) §1. The text below is unchanged from the working note.

- What becomes testable is a collider spectrum: one partner level per Standard Model field at √3 κ, then a continuum from 2 κ, with the gravity tensor continuum starting at the same 2 κ. The level ratio 2/√3 = 1.155 differs from universal extra dimensions (second level at twice the first). This is where the 3 : 4 spectral ratio becomes an observable.

## 2. Inputs (read, not rederived)
- Matter partners: odd bound state √3 c_i κ, continuum 2 c_i κ (P20 post-R3 §11; P4).
- Tensor gap 2 c_u κ (SS-DYN v6/v8 [doi:10.5281/zenodo.23604782](https://doi.org/10.5281/zenodo.23604782)); protected matter has no linear tensor-continuum charge.
- Q pole m_Q²(r) = (2/3) ζ_X κ² / (1 + δ_Q), δ_Q = r ζ_X (π² − 6)/18, ζ_X = 181150: m_Q/κ = 340.94 at r = 1e-6 (P20 R3 gate; DYN v8 gives 340.936009).
- Scalar continuum edge 2κ/√r (exact).
- Parent cutoff Λ⊥ = 8.10 keV (r/1e-6)^{1/2} at the benchmark, with Λ⊥³ ∝ κ² M4 (P20 R3 gate §2). SS-DYN v8 marks this as a conditional parent statement (C09): the cubic coefficient is not independently rederived, and the corrected substitution leaves 8.10 keV unchanged only "conditional on the first operator formula"; the erroneous form gives 5.62 keV.
- Q-shift ceiling r ≲ 2.57e-6 (10% shift), independent of κ.

## 3. Bounds on κ
Gravity (lower): at the benchmark the Q Yukawa range is 58.1 μm with α_Q ≈ 0.32. Using the Eöt-Wash |α| = 1 curve (38.6 μm) conservatively, κ ≳ 1.5 × benchmark. Weak.

Self-consistency (upper): the parent EFT needs Λ⊥ above the scalar continuum edge. Since Λ⊥ ∝ κ^{2/3} while the edge ∝ κ, the lower end of the r window rises as r_lo ≈ 2.46e-12 (κ/κ0)^{1/3}. It meets the Q ceiling at κ ≈ 11.4 TeV. With the 5.62 keV form the limit drops by 0.694³, to about 3.8 TeV. At κ ≈ 1 TeV, r = 1e-6 already fails (Λ⊥ 1.75 PeV < edge 2.0 PeV); r ≈ 2.57e-6 passes (2.80 PeV > 1.25 PeV).

Colliders (lower), by analogy with minimal universal extra dimensions (mUED), where the same orthogonality forbids single production and a reflection parity makes partners pair-produced:
- 13 TeV mUED bounds on the first level: about 1.1 TeV (Choudhury and Ghosh, arXiv:1606.04084, 13 TeV multijets) up to about 1.5 TeV (Deutschmann, Flacke and Kim, arXiv:1702.00410; this number was not read verbatim).
- Odd partners present: κ ≳ 0.64 to 0.87 TeV. Reflection treated as an identification (no odd partners, continuum only): κ ≳ 0.55 to 0.75 TeV.
- The analogy is rough: couplings come from profile overlaps, not mUED's. A real recast is not done here.
- The PDG 4.16 TeV bound applies to brane-localized fermions (single KK Z/γ production) and does not apply here, because orthogonality forbids single production of partners.

Cosmology (possible upper bound, flag only): if the reflection is exact, the lightest odd partner is stable. In mUED the stable partner gives the observed dark matter for 1.25 TeV ≲ 1/R ≲ 1.5 TeV and overcloses above (as quoted in 1702.00410, citing Belanger et al.). If that carried over, √3 κ ≲ 1.5 TeV, i.e. κ ≲ 0.87 TeV, squeezing the window to about 0.64 to 0.87 TeV. Annihilation rates here are not computed, so this is not a bound yet.

## 4. Spectrum inside the window (c_i = c_u = 1, κ = 1 TeV, r = 2.57e-6)
- Matter partners: 1.73 TeV (odd, pair-produced), continuum from 2 TeV.
- Tensor continuum: from 2 TeV; no linear coupling to protected matter.
- Q pole: about 331 TeV (m_Q/κ ≈ 331 after the 10% shift at the r ceiling); scalar edge 1.25 PeV; Λ⊥ ≈ 2.8 PeV.
- M5 ≈ 1.6e22 eV, so no TeV-scale quantum gravity.

## 5. What this changes
1. The per-leaf parent (P2) is phenomenologically allowed with finite hopping if κ sits in the window; it no longer needs μ → ∞ or a stiffness hierarchy.
2. The common-metric reference model (DYN v8, one matter metric) has no matter tower; for it, raising κ only removes the gravity signatures.
3. The fifth-force programme (Q pole, Eöt-Wash recasts) loses its target in this branch. The two branches are distinct choices: mm-scale κ (gravity tests, matter tower constrained away) or TeV-scale κ (collider tests, no gravity tests).
4. Spectroscopy prediction: E(partner)/E(threshold) = 3/4 in mass², 0.866 in mass, shared across spins, and equal to the tensor threshold. mUED predicts first-to-second level ratio 1/2.

## 6. Open points
- A real collider recast with SS overlaps, decay chains and the compressed (degenerate) spectrum.
- The relic abundance of the lightest odd partner, if reflection is exact.
- Rederiving the parent cutoff coefficient (sets the upper end: 4 or 11 TeV).
- Why κ is near a TeV (moved hierarchy, not solved).
- Whether the PHEN and Book 1 narrative can carry a branch with no gravity tests.

## 7. Files
- This note. Script `c14_common_scale.py` and output `c14_out.txt` (not included in this release).

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v6**: D. G. Palmer (2026). *SS-DYN: A Scale-Localized Leafwise Dynamical Closure for Scale Space: Protected Tensor Gravity, a Repaired Scalar Continuum, and Constrained Collective Matter* (version 6). Zenodo. [doi:10.5281/zenodo.23604782](https://doi.org/10.5281/zenodo.23604782). Published; superseded by version 8 ([doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)).
- **SS-DYN v8** (written "DYN v8" in this note): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **Paper 20**: D. G. Palmer (2026). *Paper 20: Dynamical Closure of the Scale-Space Framework: Complex Scale Potential, Newtonian Recovery, and the Hidden Configurational Sector*. Zenodo. Retired series (historical record), replaced by SS-DYN; published versions v2 to v10, the last being version 10, [doi:10.5281/zenodo.21684395](https://doi.org/10.5281/zenodo.21684395). The Paper 20 gate documents this note refers to (for example P20_NS_gate_v1) are unpublished working documents and are not included.
- **SS-PHEN v3** (written "PHEN" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-PHEN: Experimental Phenomenology of Scale Space: Protected Short-Range Scalar Response, Radiative Null Tests, and Matched Source Corrections* (version 3). Zenodo. [doi:10.5281/zenodo.24044658](https://doi.org/10.5281/zenodo.24044658). Published; current version.

Other working notes referred to by label:

- P2: [WN-04](WN-04_P2Parent.md)
- P4: [WN-15](WN-15_P4CouplingWeight.md)
- P20: the retired Paper 20 series and its unpublished gate documents (see References).
