> **Public edition of evidence note WN-21.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P13L5DScaleGeometry.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `75b7e1cfc7117392df2c03510c37e2f53a1e59f7d049550c843111ced6dc96e3` (4358 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# P13. Which geometry SS-L5D [v1, doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609) gives the scale dimension near λc

WS1 working note, 8 November 2026. Draft for the author. Working material only: not reviewed, nothing published.
Follows [WN-20](WN-20_P12FoldDilation.md) §3 and [WN-17](WN-17_P7FoldRule.md) §5 item 6. Script: `c21_l5d_centred_lapse.py` (symbolic, sympy; needs no other file). Output: `c21_out.txt`. Neither is included in this release.
Source read: `SS-L5D_Clock geometry_v1.tex` (LaTeX source of SS-L5D v1; not included; canonical, version 1, last touched 2 November 2026; depends on SS-GEO v6 [doi:10.5281/zenodo.23603029](https://doi.org/10.5281/zenodo.23603029), SS-PIVOT v8 [doi:10.5281/zenodo.23607414](https://doi.org/10.5281/zenodo.23607414), SS-DYN v8 [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)).

## 1. Question
P12 found that SS-GEO's H⁴ has no isometric mirror at a constant-scale level, while the SS-DYN parent's kink background (e^A = sech²) does. Which of the two does SS-L5D give its scale dimension near the localized level λc?

## 2. What SS-L5D says
1. **Scale geometry: SS-GEO's H⁴, everywhere.** L5D fixes the configuration metric h = e^(2u) dx² + a² du² with u over all reals ("This is the hyperbolic metric in horospherical coordinates") and varies only the clock factor (lapse) N in g = −c²N² dt² + h. Scale u is the fourth configuration coordinate; t is the fifth, a reference clock.
2. **No localized level.** L5D does not mention λc, the kink, a localizer centre, a mirror, a reflection, a fold or a half-line. The word "localizer" appears once, describing SS-DYN.
3. **No claimed link to SS-DYN.** "Its finite classical closure is not automatically the single five-coordinate metric studied here, and no reduction or dynamical equivalence is asserted." Comparison "must be made through an explicit reduction, embedding or matching map."
4. **The ends of the scale line, not a centre.** The scale-only clocks are monotone: N = e^u (AdS₅ Poincaré patch, conformal boundary as u → +∞) and N = e^(pu) (Lifshitz; for p > 1 a tidal singularity as u → −∞). A finite scale interval is allowed for p > 1, with no boundary data supplied. No scale-only clock singles out a scale level.

## 3. One new point (c21)
L5D's second vacuum clock, N_c = ½[e^u(1 + |x|²/a²) + e^(−u)] (L5D eq. centered), is the only one with a distinguished level (u = 0, at x = 0).
- N_c = cosh(d/a), with d the H⁴ distance from the point (x, u) = (0, 0). It satisfies L5D's vacuum criterion Hess N = N h/a².
- It is exactly invariant under GEO's scale reflection about that point (the hemisphere inversion of P12).
- It is not invariant under the pure scale fold u → −u at fixed x, except on the axis x = 0 or the level u = 0.
- So L5D already holds a clock geometry with a scale mirror, but the mirror is centred on one point of space, exactly as P12 found for GEO. It is not a fold of the whole scale axis.

## 4. What it means
- **L5D does not supply Rule F**, and does not contradict it either: it simply never describes the region near λc.
- **The choice P12 named is open in L5D.** If L5D is to treat scale as the fourth dimension near the localized level, it has to say whether that dimension carries GEO's H⁴ there (no constant-scale mirror) or the parent's warped kink geometry (mirror at λc).
- **A Rule F statement in L5D would be new content**, a property of the parent's warped scale geometry, with GEO's H⁴ as the far-from-λc reference. It could not be derived from L5D's current setup.
- **L5D's matching map is the place for it.** L5D already asks for "an explicit reduction, embedding or matching map" to SS-DYN; the kink background and its fold would be part of that map.

## 5. Proposal only
- Mark P7 §5 item 6 (state the fold in SS-L5D) as: not possible from L5D v1's content; would be an addition tied to the L5D–DYN matching map.
- Possible future L5D sentence (not proposed for any version now): "Near the localized level the scale direction carries the parent's warped geometry, e^A = sech²[κ(λ − λc)], whose reflection about λc is an isometry; the hyperbolic configuration metric is the reference geometry away from that level."

## 6. Limits
- AI reading and symbolic checks, not reviewed. One file read; L5D's audit notes and Zenodo variant were not compared.
- Whether a dynamical geometry should match GEO far from λc is not settled here (P12 §4).

## 7. Files
- This note. Script `c21_l5d_centred_lapse.py` and output `c21_out.txt` (not included in this release).

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-GEO v6** (written "GEO" in this note): D. G. Palmer (2026). *SS-GEO: Logarithmic Scale as a Geometric Coordinate: Exact-Distance Projection and Radial Scale Response* (version 6). Zenodo. [doi:10.5281/zenodo.23603029](https://doi.org/10.5281/zenodo.23603029). Published; current version.
- **SS-L5D v1** (written "L5D", "L5D v1" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-L5D: Clock Geometry and Consistent Five-Dimensional Extensions of Scale Space* (version 1). Zenodo. [doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609). Published; current version.
- **SS-PIVOT v8**: D. G. Palmer (2026). *SS-PIVOT: From Scale Geometry to Gravitational Dynamics: What the Configuration Manifold Determines—and What It Does Not* (version 8). Zenodo. [doi:10.5281/zenodo.23607414](https://doi.org/10.5281/zenodo.23607414). Published; superseded by version 9 ([doi:10.5281/zenodo.24044579](https://doi.org/10.5281/zenodo.24044579)).

Other working notes referred to by label:

- P7: [WN-17](WN-17_P7FoldRule.md)
- P12: [WN-20](WN-20_P12FoldDilation.md)
