> **Public edition of evidence note WN-19.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P11bDYNWording.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `8d6168a54041df24dc8bbf05db37a9549c39e90401418ec5d555a745f35876ec` (8738 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# P11b. Proposed SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) wording changes from P5 to P10, corrected

WS1 working note, 8 November 2026. For the author's decision. Proposals only: nothing published. Any change would go into a new SS-DYN version.
This replaces P11DYNWording.md (not included), which is kept unchanged. It applies findings F1 to F8 of [WN-18](WN-18_P11Rev.md), a review written in a separate Claude session (not an external review). On the author's decision of 8 November, Rule F is held out of SS-DYN.
Reference text: `SS-DYN_leafwise_dynamical_closure_v8.tex` (LaTeX source of SS-DYN v8; not included; canonical, version 8.0.0, last touched 31 October 2026). Quotes are from that file, with LaTeX simplified.

## 0. Summary

| # | Where in v8 | Change | Basis | Status label (P11Rev) | Readiness |
|---|---|---|---|---|---|
| 1 | Validity section, cutoff paragraph; claim row C09 | The 8.10 keV coefficient belongs to one mode in a regulator box of eight kink widths | P8 | Growth with the box: Established within current model (numerical, rebuilt regulator). 8.10 keV itself: Derived conditional | Ready |
| 2 | Same paragraph, directly after change 1 | Couplings driven from the localized level below about 0.94 m_s,gap do not depend on the box | P9, P10 | Derived conditional | Ready. P10's extension was checked and passed in P11Rev |
| 3 | "Why the full parent remains open" | Name the parent cubic Q term that D lacks | P10 | Derived conditional | Ready |
| 4 | none | Rule F held out of SS-DYN | P6, P7 | Postulated | Held pending the dilation-pairing check |
| 5 | "Implications for the books and remaining work" | Name the far region of the scale axis as an open item | P8, P9 | Open | Ready |

## 1. The cutoff coefficient is a one-mode, regulator-box value (P8; F3, F8)

Current, Validity section, one paragraph: "The scalar threshold is not a UV cutoff. Classical nonlinear control depends on amplitude, gradients, bandwidth and background. The original parent Galileon normalization contains a factor-three substitution error: (...). The headline 8.10 keV is unaffected by this substitution repair: conditional on the first operator formula, it remains 8.10 keV (...); the erroneous substituted formula instead gives 5.62 keV. The original cubic coefficient has not been independently rederived. This parent scale does not transfer to the two-derivative common-metric model."

Current, claim row C09: "Parent EFT interval and cutoff are conditional parent statements, not a validated domain for D."

Proposed addition, after "...has not been independently rederived.":
> The coefficient behind 8.10 keV (Ĉ3 = 40469.6, null-sector gate of 18 August) was computed for the softest Q-orthogonal odd mode in a regulator box |y| ≤ 8 kink widths, y = κ(λ − λc). Over 98% of it comes from |y| > 4, and its integrand peaks about 1.7 widths inside the box wall. A rebuilt regulator reproduces the gate's five-value regression to 7×10⁻⁵ or better. The coefficient grows roughly as e^(2Y)/Y^4.5 with the half-width Y (the power is fitted, not derived), so the quoted scale is about 3.0 keV at Y = 10 and 1.0 keV at Y = 12, and tends to zero for this mode as Y grows without limit. Modes concentrated nearer the wall couple more strongly. The figure describes this mode and this box, not the continuous-scale theory.

Proposed C09 row:
> Parent EFT interval and cutoff are conditional parent statements, computed for one mode in a regulator box of eight kink widths and dependent on that box; not a validated domain for D.

## 2. Localized-level couplings do not see the box (P9, P10; F1, F2, F3)

Placement: directly after the change 1 text, so that it follows the box statement it qualifies.

Proposed addition:
> In the parent regulator the cubic Galileon vertex is local along the scale axis. For fields driven from the localized level below about 0.94 m_s,gap, with m_s,gap = 2κ/√r, and for the Q–Q–Q, Q–Q–χ and Q–χ–χ couplings with χ so driven, the cubic couplings do not depend on the box (tested to Y = 20). The zero-mode couplings of protected matter with at most one continuum leg are also box-independent. Couplings among continuum states do depend on the box, and Q with two continuum states grows linearly with it. This is a tree-level, cubic-order, probe-limit statement about the parent. The common-metric results of this record (Q pole, α_Q, valley, material tests) are computed in D_{N,L}, which has no parent box.

v8's next sentence, "This parent scale does not transfer to the two-derivative common-metric model", stays as it is.

## 3. A parent term D omits (P10; F7)

Current, "Why the full parent remains open": "The complete sum of parent vertices and nonlinear reconstruction remains to be calculated. Neither the common-metric action nor its successful tests silently supply this missing theorem."

Proposed addition, before "Neither...":
> One such vertex is a parent cubic Galileon for the Q direction itself, absent from the common-metric action. In the null-sector gate's convention its coefficient is 0.033, independent of the regulator box, and its scale is about 107 times the Y = 8 value of the orthogonal cutoff (about 0.87 MeV at the millimetre benchmark). A cubic Galileon of this kind is normally suppressed on shell by m_Q²/Λ³; that has not been derived here. Vertices that include the massless common mode, to which Q is kinetically mixed, have not been examined. This is a derivative cubic, distinct from the potential cubic C_QQQ of Section 5.

## 4. Rule F: held out of SS-DYN (P6, P7; F4, F5, F6)

Not proposed for SS-DYN at this time. Reasons:
- v8 already declares the part that concerns D: the odd perturbation family, the fixed centre and the odd scalar pencil. A localizer-only Rule F would add a postulate without changing a result.
- The tensor exclusion that P6 and P7 cite ("excluded by reflection parity", "excluded from the even leaf-metric sector") is in SS-DYN v6 [doi:10.5281/zenodo.23604782](https://doi.org/10.5281/zenodo.23604782) and SS-PHEN v2 [doi:10.5281/zenodo.23868193](https://doi.org/10.5281/zenodo.23868193), not v8. The matter-partner part is outside v8's scope (v8: a unified microscopic matter account is not specified).
- The dilation-pairing check (P7 §5 item 5) could void the rule and has not been done.

Record of the checks, for later:
- P7 check 1 (cutoff computed with P-even modes only): done in P8. The gate direction is P-even; the fold leaves Ĉ3 unchanged.
- Half-line convention (F4): with M5³ and γ doubled the Q pole is exactly unchanged (340.936009); with γ unchanged it would be 473.35.
- Checks 2 to 6 of P7 §5 remain: folding the finite regulator, normalization, fermion signs, dilation pairing, SS-L5D [v1, doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609) statement.
- If the rule is later adopted, the affected text includes SS-PHEN v2 as well as v6-derived passages, and the matter part belongs with the matter documents (MAT or SS-L5D).
- The TeV argument for Rule F rests on P6's nucleosynthesis comparison, which was not confirmed against the figures of arXiv 1709.01211. The box limit P8 put on the TeV window was lifted by P9, but P9's new upper end is indicative only.

## 5. The far region as an open item (P8, P9)

Current, "Implications for the books and remaining work": "Remaining validation includes ... strict nonlinear scale-continuum analysis, and quantum matching."

Proposed addition:
> The parent's behaviour in the far region of the scale axis, where the protected weight F falls and both localizer and matter couplings grow, is unspecified. It matters for parent physics near and above m_s,gap and for continuum rescattering, not for the low-energy results of this record.

## 6. Not proposed for SS-DYN

- **TeV common-scale branch (P5).** It replaces the 9.9 mm calibration convention and removes every gravity test. That is a programme choice for strategy and PHEN.
- **The 3 : 4 partner ratio (P5).** Withdrawn in P6.

## 7. What stays as it is

The Q pole (340.936009), α_Q, the 0.0012 orthogonal-strength ratio, the valley formulas, the homogeneous, probe and material tests, the relative-lapse obstruction, and the excluded status of the fixed benchmark.

## 8. Limits

- The underlying computations are AI work. P11Rev re-ran c17, c18 and c19 and checked P10's extension from scratch; it is a check by a separate Claude session, not an external review.
- Ĉ3 and g3 are taken as printed; the regulator is a rebuild, not the gate's own code.
- P9 and P10 are tree level, cubic order, probe limit, one source shape.
- Each change needs the author's review and the programme's usual source and delta audit.

## 9. Files

- [WN-19](WN-19_P11bDYNWording.md) (this note)
- Replaces P11DYNWording.md (not included). Review: [WN-18](WN-18_P11Rev.md); its script `rev_p11.py` and output `rev_p11_out.txt` are not included in this release.
- Basis notes: [WN-24](WN-24_P5CommonScale.md), [WN-16](WN-16_P6ReflectionFold.md), [WN-17](WN-17_P7FoldRule.md), [WN-22](WN-22_P8CutoffBox.md), [WN-23](WN-23_P9FarRegion.md), P10QLeg.md (not included)

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v6**: D. G. Palmer (2026). *SS-DYN: A Scale-Localized Leafwise Dynamical Closure for Scale Space: Protected Tensor Gravity, a Repaired Scalar Continuum, and Constrained Collective Matter* (version 6). Zenodo. [doi:10.5281/zenodo.23604782](https://doi.org/10.5281/zenodo.23604782). Published; superseded by version 8 ([doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)).
- **SS-DYN v8** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-L5D v1** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-L5D: Clock Geometry and Consistent Five-Dimensional Extensions of Scale Space* (version 1). Zenodo. [doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609). Published; current version.
- **SS-MAT v1** (written "MAT" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MAT: Scale-Extended Matter Sources: Protected Matching, Scale Transport and Completion Gates* (version 1). Zenodo. [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555). Published; current version.
- **SS-PHEN v2**: D. G. Palmer (2026). *SS-PHEN: Experimental Phenomenology of Scale Space: Protected Short-Range Scalar Response, Radiative Null Tests, and Matched Source Corrections* (version 2). Zenodo. [doi:10.5281/zenodo.23868193](https://doi.org/10.5281/zenodo.23868193). Published; superseded by version 3 ([doi:10.5281/zenodo.24044658](https://doi.org/10.5281/zenodo.24044658)).
- **SS-PHEN v3** (written "PHEN" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-PHEN: Experimental Phenomenology of Scale Space: Protected Short-Range Scalar Response, Radiative Null Tests, and Matched Source Corrections* (version 3). Zenodo. [doi:10.5281/zenodo.24044658](https://doi.org/10.5281/zenodo.24044658). Published; current version.

Other working notes referred to by label:

- P5: [WN-24](WN-24_P5CommonScale.md)
- P6: [WN-16](WN-16_P6ReflectionFold.md)
- P7: [WN-17](WN-17_P7FoldRule.md)
- P8: [WN-22](WN-22_P8CutoffBox.md)
- P9: [WN-23](WN-23_P9FarRegion.md)
- P10: not included in this release.
- P11Rev: [WN-18](WN-18_P11Rev.md)
