> **Public edition of evidence note WN-20.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P12FoldDilation.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `807e4bd8a151440ecb5d9f3e0a7be5a821624193f40ecd0478072638c64b8f96` (5326 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# P12. Rule F against the Scale Space pairing of scale shifts and spatial dilations

WS1 working note, 8 November 2026. Draft for the author. Working material only: not reviewed, nothing published.
Follows [WN-17](WN-17_P7FoldRule.md) §5 item 5 and [WN-19](WN-19_P11bDYNWording.md) §4. Script: `c20_fold_dilation.py` (symbolic, sympy; needs no other file). Output: `c20_out.txt`. Neither is included in this release.

## 1. Question
SS-GEO v6 [doi:10.5281/zenodo.23603029](https://doi.org/10.5281/zenodo.23603029) gives the reference scale geometry dΣ² = e^(2u) dx² + a² du², four-dimensional hyperbolic space H⁴ of curvature radius a. Its exact symmetry pairs a scale shift with a spatial dilation: T_b: u → u + b, x → e^(−b) x (GEO eq. dilation_isometry, Killing vector ∂_u − x·∂_x). A pure scale shift is not a symmetry there.
Rule F folds the scale axis at λc: (λ − λc) → −(λ − λc). P6 flagged that this pairing might clash with the fold or give the scale-shift mode a mass. The review (P11Rev) named this as the check that could void the rule.

## 2. Result

1. **The pairing does not void the fold.** In GEO's geometry the reflection and T_b fit together the way a reflection and a translation of a line do:
   - I T_b I = T_(−b): the fold reverses the dilation.
   - T_b I T_b⁻¹ is the same fold about the level u_c + b. Every level is equivalent, and fixing one fold level breaks T_b.
   - The kink already breaks T_b (it fixes λc), so the fold adds no new breaking.
   - The broken generator is odd under the fold. Its mode (sech²y in DYN's localizer language) is removed, so the question of whether the pairing gives it a mass does not arise.
2. **GEO does not support the fold either.**
   - A pure scale reflection at fixed x is not an isometry of GEO's metric, nor is one at fixed physical position.
   - The fixed set of an isometric reflection must be totally geodesic. Constant-scale slices of H⁴ are horospheres, with second fundamental form K_ij = h_ij/a ≠ 0. So **no isometry of GEO's geometry can fold the scale axis about a constant-scale slice.**
   - GEO's scale reflections are inversions in a hemisphere |x|² + z² = ρ² (z = a e^(−u), ρ = a e^(−u_c)) centred on one spatial point. On the axis through that point it is exactly u → 2u_c − u.
   - Off the axis it keeps the physical distance R = e^u|x| from the centre but shifts the scale: u' = 2u_c − u + ln(1 + R²/a²). It is close to a pure scale fold only within R ≪ a of the centre.
   - It does not commute with spatial translations. A fold built from it would pick a preferred point in space, which no universal rule can do.
3. **The parent geometry does support it.** In SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)'s parent comparison metric the warp e^A = sech²[κ(λ − λc)] is even, so the pure fold is an exact isometry of that background.
   - Far from the centre, A' → ∓2κ. Each side is locally an exponential, GEO-like warp, and the two sides are mirror images glued at λc.
   - The parent background has no T_b-type symmetry (A is not linear); the kink replaces it.

## 3. What it means
- **Rule F survives this check.** The dilation pairing is broken by the localized level anyway, and the fold removes the mode that pairing would have governed.
- **Its justification cannot come from SS-GEO.** In GEO's H⁴, scale space has no mirror at a constant-scale level; the only scale mirrors are hemispheres centred on a point in space. P7 §4 item 4's reading (a self-dual scale ℓc, with ℓ and ℓc²/ℓ the same level) holds in GEO only on one spatial axis.
- **The support is the dynamical parent itself.** Its kink background is mirror-symmetric about λc, so the fold is a statement about the dynamical geometry, consistent with v8's "configuration geometry and dynamical geometry are distinct".
- **What this asks of SSF.**
  - If GEO's H⁴ is meant as the geometry of scale space at all scales, a constant-scale fold cannot be a symmetry quotient of it.
  - If the parent's warped geometry is the physical one, the fold is natural, and GEO is a reference far from the localized level.
  - The author's request that SS-L5D [v1, doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609) treat scale as the fourth dimension makes this choice concrete: L5D should say which geometry its scale dimension carries near λc.
- **For SS-DYN nothing changes.** Rule F stays out (P11b §4). If adopted later, it should be worded as a property of the dynamical parent geometry and say that SS-GEO does not supply it.

## 4. Limits
- AI computation, not reviewed. Symbolic checks of exact identities; no numerics.
- GEO's metric is taken as the reference configuration metric. Whether a dynamical geometry should inherit its isometries is a framework question, not settled here.
- The physical size of a is not fixed in SS-DYN or SS-GEO, so how far from a spatial centre GEO's inversion stays close to a pure fold cannot be stated in physical units.
- Matter, fermion signs and the finite regulator (P7 checks 2 to 4) are not touched. SS-L5D was not read for this note.

## 5. Proposal only
- Mark P7 §5 check 5 as done: no contradiction; no support from GEO; support from the parent background.
- Any future Rule F wording should say "an isometry of the parent's localized background, not of the SS-GEO reference geometry".

## 6. Files
- This note. Script `c20_fold_dilation.py` and output `c20_out.txt` (not included in this release).

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-GEO v6** (written "GEO" in this note): D. G. Palmer (2026). *SS-GEO: Logarithmic Scale as a Geometric Coordinate: Exact-Distance Projection and Radial Scale Response* (version 6). Zenodo. [doi:10.5281/zenodo.23603029](https://doi.org/10.5281/zenodo.23603029). Published; current version.
- **SS-L5D v1** (written "L5D" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-L5D: Clock Geometry and Consistent Five-Dimensional Extensions of Scale Space* (version 1). Zenodo. [doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609). Published; current version.

Other working notes referred to by label:

- P6: [WN-16](WN-16_P6ReflectionFold.md)
- P7: [WN-17](WN-17_P7FoldRule.md)
- P11Rev: [WN-18](WN-18_P11Rev.md)
- P11b: [WN-19](WN-19_P11bDYNWording.md)
