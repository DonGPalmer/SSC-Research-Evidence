> **Public edition of evidence note WN-17.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P7FoldRule.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `689f5646c3420416447f442bf5a6022371882ed0c1f2e40023fda49801dc044c` (5819 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** Its attribution of the tensor exclusion to SS-DYN v8 is corrected in [WN-18](WN-18_P11Rev.md) and [WN-19](WN-19_P11bDYNWording.md), its geometric reading in §4 is found to hold in SS-GEO only on one axis in [WN-20](WN-20_P12FoldDilation.md), and its §5 SS-L5D step is found not possible from SS-L5D v1 in [WN-21](WN-21_P13L5DScaleGeometry.md). Editorial notes mark the affected passages; the original wording is kept.

# P7. Rule F, the scale fold: draft architecture rule

WS1 working note, 8 November 2026. Draft for the author's decision. Working material only: not reviewed, nothing published.
Follows [WN-16](WN-16_P6ReflectionFold.md). Script: `c16_fold_halfline.py`; output: `c16_out.txt` (not included in this release).

## 1. Draft wording

> **Rule F (scale fold).** The scale axis is folded at the localization centre λc. Two field configurations related by the reflection P are the same physical configuration, and only P-even states are physical. P acts as (λ − λc) → −(λ − λc), X → −X, g_μν → g_μν, A_μ → A_μ, A_λ → −A_λ, H → H, and ψ → η_ψ γ5 ψ, with η_ψ = −1 for a fermion whose zero mode is left-handed and η_ψ = +1 for one whose zero mode is right-handed.

Equivalent form: scale space is the half-line λ ≥ λc, with these conditions at λc:

| Field | Condition at λc |
|---|---|
| leaf metric g_μν (lapse, shift) | Neumann |
| localizer X | Dirichlet, X(λc) = 0 |
| gauge A_μ / A_λ | Neumann / Dirichlet |
| Higgs H | Neumann |
| fermion with L zero mode | ψ_L Neumann, ψ_R Dirichlet |
| fermion with R zero mode | ψ_R Neumann, ψ_L Dirichlet |

The action (eq. Sspec) with protected matter is P-invariant term by term:
- F(X) is even.
- In the localizer square, ∂λX and κv(1 − X²/v²) are both even.
- The strain is odd, so its square is even.
- The kink mass m(X)ψ̄ψ and the Yukawa terms are invariant with the η choice above.

The kink itself is P-even.

## 2. What it keeps (c16)
- Tensor: the zero mode, and the continuum from 4κ² (Neumann l = 2). This is DYN C02 as stated.
- Matter zero modes:
  - gauge, Higgs and chiral fermions;
  - the protection theorem, g4 = g5√(3κ/4), and zero-mode universality are unchanged.
- Q pole:
  - on the half-line (Dirichlet, integrals over the half-line), m_Q/κ = 340.932, against DYN's 340.936 on the full line;
  - the scalar edge 2κ/√r is unchanged.
- Protected-source results: the protected source is P-even, so all its overlaps lie in the kept sector. The 1.2 × 10⁻³ continuum fraction, α_Q and the Eöt-Wash screen are unchanged.

## 3. What it removes
- The odd tensor state at 3κ². DYN already drops it; under Rule F it is dropped by rule rather than by remark.
- The matter partners at √3 c_i κ for gauge, Higgs and fermions. In c16 the E = 3 level appears only for the excluded conditions (l = 2 Dirichlet, l = 1 Neumann).
- The scale-shift (translation) mode, the massless Planck-coupled scalar of P6 (the Neumann zero mode of δX).
- The P-odd half of every continuum. This has no effect on protected sources.
- With these, the nucleosynthesis problem of P6's symmetry reading goes away.

## 4. Justification

> **Editorial note (public edition, 19 November 2026):** Later notes find that SS-DYN v8 contains no exclusion of the 3κ² tensor state (item 1 below): the exclusion sentences cited here and in P6 ("excluded by reflection parity", "excluded from the even leaf-metric sector") are in SS-DYN v6 and SS-PHEN v2, not v8. They confirm that v8 declares the odd perturbation family, the fixed centre and the odd scalar pencil. See [WN-18](WN-18_P11Rev.md) F6 and [WN-19](WN-19_P11bDYNWording.md) §4. The text below is unchanged from the working note.

1. **DYN already uses it.**
   - It drops the 3κ² tensor state.
   - It analyses the localizer only in its odd-function (P-even) sector.
   - Its scalar spectrum lists no massless mode.
   - It calls λc a fixed datum.
   - Without the fold, DYN would owe one more tensor state and one more massless scalar in its degree count.
2. **It pins the centre.** On the half-line, λc is a fixed point of the geometry, not a vacuum choice with a massless mode. That matches DYN's treatment of λc. Its value is still not selected.
3. **Precedent.** Z2 quotients with fixed points are standard in extra-dimension model building, where they remove modes and produce chiral zero modes (orbifolds in Randall–Sundrum and universal-extra-dimension models). Here the axis is non-compact, with one fixed point.

> **Editorial note (public edition, 19 November 2026):** A later note finds that the reading in item 4 below (a self-dual scale ℓc, with scale inversion about it identifying levels) holds in SS-GEO only on one spatial axis: SS-GEO's H⁴ has no mirror at a constant-scale level, so the fold's justification cannot come from SS-GEO and rests instead on the mirror-symmetric kink background of the dynamical parent. See [WN-20](WN-20_P12FoldDilation.md) §3. The text below is unchanged from the working note.

4. **Geometric reading (interpretation, for the author to judge).**
   - If λ is proportional to the log-scale coordinate u, then P is scale inversion ℓ → ℓc²/ℓ about a self-dual scale ℓc.
   - The fold then says ℓ and ℓc²/ℓ label the same level, so scale space runs one way from the localized level. This echoes the self-dual radius of T-duality, but only as motivation.
   - Tension: SSF treats scale as a full coordinate across many levels. Under the fold, the localized level sits on the edge of scale space.
5. **Phenomenology.**
   - Only the fold keeps the TeV common-scale option open (P6).
   - It removes the √3 c_i κ half of the Paper-20 [retired series; see References] matter obstruction. The matter continuum at 2 c_i κ remains.

## 5. To check before adoption
1. **Parent cutoff.** Confirm that the cubic coefficient Ĉ3 behind Λ⊥ was computed with P-even modes only. If P-odd modes entered, recompute it. This sets the upper end of the TeV window.
2. **Finite regulator.** Map the reflection-compatible dRGT tree to sites n ≥ 0, with the centre site as the fixed point. Check that the three-site shared-root gate folds to two sites without new constraints.
3. **Normalization.** State which convention the M4 relation uses.
   - Covering line: DYN's current M4² = 4M5³/(3κ) and γ = 9/(8ζ_X).
   - Half-line: M5³ and γ doubled.
   - c16 confirms the spectrum is the same either way, but the numbers quoted for M5 depend on the choice.
4. **Fermion content.** Fix η per Standard-Model field. The chiral zero-mode content is unchanged, so anomaly cancellation carries over.
5. **Dilations.** Check compatibility with the Scale Space pairing of scale shifts and spatial dilations (the T_c map).

> **Editorial note (public edition, 19 November 2026):** A later note finds that the step in item 6 below is not possible from the content of SS-L5D v1, which gives scale the SS-GEO H⁴ geometry everywhere and never describes the region near λc; a statement of the fold there would be an addition tied to the L5D–DYN matching map. See [WN-21](WN-21_P13L5DScaleGeometry.md) §5. The text below is unchanged from the working note.

6. **SS-L5D [v1, doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609).** State the fold in the scale-as-fourth-dimension geometry as well.

## 6. Placement (proposal only)
If adopted, the changes would be:
- add one paragraph to SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)'s architecture section;
- add one claims-table row ("The scale axis is folded at λc; only P-even states are physical");
- rewrite C02's "excluded by reflection parity" to cite the rule.

These would be made in a new version of SS-DYN.

## 7. Files
- This note. Script `c16_fold_halfline.py` and output `c16_out.txt` (not included in this release).

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-L5D v1** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-L5D: Clock Geometry and Consistent Five-Dimensional Extensions of Scale Space* (version 1). Zenodo. [doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609). Published; current version.
- **Paper 20**: D. G. Palmer (2026). *Paper 20: Dynamical Closure of the Scale-Space Framework: Complex Scale Potential, Newtonian Recovery, and the Hidden Configurational Sector*. Zenodo. Retired series (historical record), replaced by SS-DYN; published versions v2 to v10, the last being version 10, [doi:10.5281/zenodo.21684395](https://doi.org/10.5281/zenodo.21684395). The Paper 20 gate documents this note refers to (for example P20_NS_gate_v1) are unpublished working documents and are not included.

Other working notes referred to by label:

- P6: [WN-16](WN-16_P6ReflectionFold.md)
