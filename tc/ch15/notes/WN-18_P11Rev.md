> **Public edition of evidence note WN-18.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P11Rev.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `8c4f411f2170a186df578174602f126b0aba87186bf4ee46470919d4ccb90a6e` (14550 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# P11Rev. Independent review of P11 and its basis notes P5 to P10

WS1 auditor note, 8 November 2026. Reviewer: Claude, in a session separate from the one that wrote P1 to P11. Requested by the author.
Review only; any correction to P11 should be a new file.
Files: `rev_p11.py` and `rev_p11_out.txt` (20 PASS, 0 FAIL). It needs `c17_cutoff_fold_box.py` in the same folder. These files are not included in this release.

## 0. Result in brief

The numbers reproduce. The wording in P11 needs corrections before any of the five changes is used. With them, changes 1, 2 and 3 can go forward and change 5 is ready as it stands; change 4 is the author's decision. The check that changes 2 and 3 were waiting for (P10's extension) is now done and passed.

| # | P11 change | P11 readiness | My verdict | Needed |
|---|---|---|---|---|
| 1 | Cutoff is a regulator-box value | Ready | Ready after wording fixes | F3 |
| 2 | Localized-level couplings do not see the box | Needs a check of P10's extension | Check done and passed. Not ready as worded | F1, F2, F3 |
| 3 | Name the parent cubic Q term | Needs the same check | Ready after a small wording fix | F7 |
| 4 | Rule F, the scale fold | The author's decision plus P7 checks | The author's decision. I recommend not putting it in SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) as drafted | F4, F5, F6, section 3 |
| 5 | Far region as an open item | Ready | Ready | none |

Suggested status labels, in the author's five-tier vocabulary (P11 gives none): change 1, the growth with the box is Established within current model (numerical, rebuilt regulator) while the 8.10 keV itself stays Derived conditional; change 2, Derived conditional (tree level, cubic order, probe limit, one source shape); change 3, Derived conditional; change 4, Postulated; change 5, Open.

## 1. What I checked

| Check | Result |
|---|---|
| Re-ran c17, c18, c19 from the filed copies | c17 and c19 outputs identical to the filed ones. c18 identical except the last digits of the matter-vertex table (continuum-continuum-continuum 4.211e-10 vs 4.223e-10 at Y = 8, 5.747e-6 vs 5.746e-6, -8.264e-3 vs -8.267e-3). Those states are near-degenerate, so their labels can shift |
| P11 "Current" quotes against SS-DYN v8 | All five found verbatim: l.109, l.353, l.360 (three passages), l.371, l.382. Version 8.0.0, last touched 2026-10-31. C_QQQ is in Section 5 |
| Q profile algebra, exact (sympy) | K(y sech^2) = -f exactly; K(sech^2) = 0; <f, y sech^2> = -4/3; norm^2 of y sech^2 = (pi^2-6)/9; so <f,q> = -2.0334 and the Q kinetic norm is 2.668e-5 |
| Q pole, my own code (not the original notes' code) | dy = 0.04, 0.02, 0.01 gives 340.8757, 340.9209, 340.9322; Richardson 340.936009, which is DYN's value. Half-line with gamma doubled: identical to 0.0. Half-line with gamma unchanged: 473.35 |
| P10's extension to sum s not 0 | Derived from the massive-propagator limit: (L + k^2 D) h = s with kinetic weights D = diag(wF), k^2 to 0. The common mode goes as 1/k^2; the relative sector obeys L g = s - (sum s / W) wF, which is P10's s_rel. A dense solve agrees with c19's response to 4.5e-10 (Q profile) and 1.4e-13 (a generic odd profile). An unweighted subtraction differs at order 1, so the test discriminates. T(QQQ), T(QQ,box), T(Q,box,box) and T(box,box,box) agree between the two routes. Conditional on the kinetic weights being wF, the same assumption P10 makes |
| Growth law of the 8.10 keV coefficient | d ln C3/dY against 2 - 4.5/Y: within 0.003 for every interval from Y = 10 to 20; +0.04 at Y = 6 to 8 ("roughly" is right) |
| Where the coefficient comes from | At Y = 8, 98.7% from |y| > 4. At Y = 12, 16, 20 effectively all. The integrand peaks 1.62, 1.72, 1.77, 1.77 kink widths inside the box wall for Y = 8, 12, 16, 20 |
| Q-box-box growth | T = -16.43 <|y|> + 8.93, fitted on Y = 12, 16, 20; it predicts Y = 8 to 1%. P10's reading (coupling to the position along the axis) holds numerically |
| D3b | Section 9.2 locates the factor 3. It says D as printed has only two-derivative interactions. The admixture 6.7e-4 is in its table. C3 = 40469.61313 is "taken as printed" |
| Hand arithmetic | Cutoff scales 2.957, 1.022, 0.110 keV at Y = 10, 12, 16. 32/9 gives 0.943. Q cubic 0.0332, scale ratio 106.8, 0.865 MeV |

## 2. Findings

**F1. P11 section 2: "The same holds for every coupling with a Q leg" is too strong.**
P10 section 3 gives Q-box-box growing linearly with the box: -63.6, -96.6, -129.2, -161.9 at Y = 8, 12, 16, 20. P10 section 4 itself lists it under "what still depends on the far region". The box-independent set is Q-Q-Q, Q-Q-chi and Q-chi-chi with chi driven from the localized level (constant to the printed digits from Y = 8 or 12 to 20; Q-chi-chi at 0.92 M_perp goes -24.29 to -24.37 and at 0.96 M_perp -29.80 to -30.56, converged). Fix: say that, and say Q with two continuum states grows linearly with the box.

**F2. P11 section 2: "the Q pole, alpha_Q, the valley results and the material tests ... hold for any box" does not follow.**
Those are results of D_{N,L}, which has no parent regulator box. Its own finite family is box dependent: v8 l.119, "N, L must accompany every prediction". v8 l.360 says the parent scale "does not transfer to the two-derivative common-metric model". P11 section 3 says the parent cubic Q term is distinct from D's C_QQQ. No note computes a link from the parent's Galileon couplings to D's results. The sentence is either empty (D has no parent box) or ambiguous (the family's own box L = 12). Fix: delete it, or say these results do not use the parent box.

**F3. P11 section 1 loses a qualifier, and sections 1 and 2 are placed in the wrong order.**
P8 section 2 item 5 says the cutoff tends to zero "for the softest orthogonal direction". P11 says it "tends to zero on the infinite scale line", which reads as a property of the parent. P8 section 4 adds that directions concentrated near the box end couple more strongly. Add "for the softest Q-orthogonal odd mode". Sharper and checked: the integrand peaks about 1.7 widths inside the wall at every Y, so the coefficient is a wall-neighbourhood quantity.
Order: in v8 l.360 everything is one paragraph. P11's section 2 insertion goes after the second sentence, before section 1's insertion (after "not independently rederived"). Section 2 then speaks of "the box dependence of the previous paragraph", which comes later. Put the section 1 text first, or merge them.

**F4. Rule F and the Q pole: "unchanged" is exact, but only with a stated convention.**
The Q mode is an odd function, so the half-line Dirichlet problem is the same problem. The 340.932 in P7 and 340.912 in P6 differ from 340.936009 by grid size only. But this holds only with the covering-line convention carried over (M5^3 and gamma doubled). With gamma unchanged the pole is 473.35, which c16 prints. P7 section 5 item 3 flags the convention; P11 section 4 does not. Add a clause to the "equivalently, the half-line" sentence.

**F5. P7 lists six checks before adoption; P11 lists five.**
The one dropped is P7's check 1 (was the parent cutoff computed with P-even modes only?). P8 closed it: the gate direction is odd to 0.0, a P-odd direction alone has zero cubic coupling, and the mixed coupling is 1.0 against 4.0e4. P11 should say it is done. P7 section 6 also proposes rewriting "C02's 'excluded by reflection parity'". P11 correctly leaves that out, because the text is not in v8 (F6).

**F6. "v8 already behaves as if folded" is true in part.**
Confirmed in v8: the perturbation family is odd (l.117), the centre is fixed (l.109), the pencil is called "the odd scalar pencil" (l.170), and v8 contains none of the words reflection, translation, massless, zero mode. Not in v8: any exclusion of the 3 kappa^2 tensor state. The sentences that P6 and P7 quote ("excluded from the even leaf-metric sector", "excluded by reflection parity") are in SS-DYN v6 [doi:10.5281/zenodo.23604782](https://doi.org/10.5281/zenodo.23604782) (Zenodo variant, l.66 and l.218) and SS-PHEN v2 [doi:10.5281/zenodo.23868193](https://doi.org/10.5281/zenodo.23868193) (l.205). P11 repaired this ("no massive tensor tower"); P6 and P7 did not. Two consequences:
- The matter-partner and tensor parts of Rule F are outside v8's scope. v8 l.362: a unified microscopic matter account is not specified.
- The sentences that adopting Rule F would rewrite are in SS-PHEN v2 and v6-derived text, not in v8. P11 does not list PHEN as affected.

**F7. P11 section 3: numbers verified; two wording points and one gap.**
The 0.033, the factor 107 and the 0.87 MeV all reproduce (0.0332, 106.8, 0.865 MeV). "Absent from D" agrees with D3b section 9.2.
- "107 times the box value of the orthogonal cutoff": say "the Y = 8 value". By F3 the orthogonal cutoff itself moves with Y. Against the Y = 12 value the ratio is about 850.
- P10 treats only the relative-sector cubic. Vertices that include the massless common mode, to which Q is kinetically mixed (Q's kinetic norm is 27 times r), are not examined. P10's list of limits does not say so.
- "On shell it is suppressed by m_Q^2/Lambda^3" is standard for a cubic Galileon but is stated without a derivation in P10.

**F8. P11 section 1 growth law.**
"Roughly e^(2Y)/Y^4.5" is supported numerically (section 1 above). The exponent 2 matches the tail exponent that P9 derives at the scalar threshold (2 - 3 sqrt(4 - lambda), which tends to 2). I did not derive the power 4.5; it fits.

## 3. Rule F: what the notes show and what they leave open

Shown: Rule F agrees with v8's declared odd family; it removes the translation mode, the 3 kappa^2 tensor state and the matter partners; the Q pole, alpha_Q and the cutoff coefficient are unchanged (F4, F5). Not shown: why scale space should be folded. Three points that P11 mentions only in passing or not at all:
1. In SSF, scale is a full coordinate and scale shifts are paired with spatial dilations (P6 section 3 caveat; P7 section 5 item 5). A fold makes scale space a half-line with one edge. This is the check I would do first: a negative result would void the rule, and a positive one is the real justification. P11 reduces it to one closing sentence about Book 1.
2. P7 section 4 item 5 says only the fold keeps the TeV option open. That rests on P6 section 5, where the exclusion of the symmetry reading is "likely but not confirmed against the figures" of arXiv 1709.01211. P8 also limits the TeV window to a box of about 10 kink widths or less. So the TeV argument for Rule F is weaker than P7 states.
3. Where it lives: the DYN-relevant content is the odd localizer parity that v8 already declares. The matter part belongs with the matter documents (MAT or SS-L5D [v1, doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609)), and the PHEN sentence changes at that time.

My recommendation, for the author to decide: do not add Rule F to SS-DYN as drafted. If the author wants it on record in DYN now, use the localizer and metric statement in section 4 below, marked Postulated, and put the rest in the document that holds the matter content once P7 checks 2 to 6 are done.

## 4. Replacement wording (for the author's decision)

Change 1, after "...has not been independently rederived.":
> The coefficient behind 8.10 keV (C3 = 40469.6, null-sector gate of 18 August) was computed for the softest Q-orthogonal odd mode in a regulator box |y| <= 8 kink widths, y = kappa(lambda - lambda_c). Over 98% of it comes from |y| > 4, and the integrand peaks about 1.7 widths inside the box wall. A rebuilt regulator reproduces the gate's five-value regression to 7e-5 or better. The coefficient grows roughly as e^(2Y)/Y^4.5 with the half-width Y, so the quoted scale is about 3.0 keV at Y = 10 and 1.0 keV at Y = 12, and tends to zero for this mode as Y goes to infinity. The figure describes this mode and this box, not the continuous-scale theory.

Change 2, placed after the change 1 text:
> In the parent regulator the cubic Galileon vertex is local along the scale axis. For fields driven from the localized level below about 0.94 m_s,gap, and for Q-Q-Q, Q-Q-chi and Q-chi-chi couplings with chi so driven, the cubic couplings do not depend on the box (tested to Y = 20). Couplings among continuum states do, and Q with two continuum states grows linearly with the box. This is a tree-level, cubic-order, probe-limit statement about the parent. The common-metric results of this record (Q pole, alpha_Q, valley, material tests) are computed in D_{N,L}, which has no parent box.

Change 4, localizer and metric part only:
> Rule F (scale fold, postulated). The declared odd localizer parity is the localizer case of a reflection P, (lambda - lambda_c) to -(lambda - lambda_c) with X to -X, under which the kink is invariant. On the half-line lambda >= lambda_c the same problem is obtained with M5^3 and gamma doubled; with gamma unchanged the Q pole would move from 340.936 to 473.35. The geometric justification is open.

Changes 3 and 5: as in P11, with the F7 wording points for change 3.

## 5. Not checked

- g3 and C3 from the parent action: taken as printed (P8 section 5; D3b section 9.2). So the 8.10 keV stays Derived conditional.
- The regulator is a rebuild. It reproduces the 18 August five-value regression (5e-7 at J = 20 to 7e-5 at J = 320). I did not see the gate's own code.
- P10's extension holds given kinetic weights wF; vertices with the common mode are open (F7).
- P9 and P10: tree level, cubic order, probe limit, one source shape. The 0.943 threshold comes from the tail exponent and does not depend on the shape; the amplitudes were tested for one shape.
- P6 nucleosynthesis comparison: figures of arXiv 1709.01211 not read.
- P1 to P4: read, not re-derived. P5: arithmetic only. P7 section 5 checks 2 to 6: not done.
- The physical meaning of Y in kink widths (P8 section 5).

## 6. Decisions for the author

- **D-1.** P11 needs a corrected version with F1 to F8 applied. It should be a new file, not an edit in place. Who issues it is the author's call.
- **D-2.** Rule F: hold it out of SS-DYN as drafted (section 3), or use the section 4 localizer-only wording as Postulated.
- **D-3.** Whether the dilation-pairing check (P7 section 5 item 5) should come next, since it decides whether Rule F survives.

## 7. Files and inputs

- This note. Script `rev_p11.py` and output `rev_p11_out.txt` (not included in this release).
- Scripts re-run from the reviewed notes: `c17_cutoff_fold_box.py`, `c18_far_region.py`, `c19_q_leg.py` (not included in this release).
- Sources compared: SS-DYN v8.0.0 (canonical), SS-DYN v6 Zenodo variant, SS-PHEN v2, WS1 note D3b (24 October).

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v6**: D. G. Palmer (2026). *SS-DYN: A Scale-Localized Leafwise Dynamical Closure for Scale Space: Protected Tensor Gravity, a Repaired Scalar Continuum, and Constrained Collective Matter* (version 6). Zenodo. [doi:10.5281/zenodo.23604782](https://doi.org/10.5281/zenodo.23604782). Published; superseded by version 8 ([doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)).
- **SS-DYN v8** (written "DYN" in this note): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-L5D v1** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-L5D: Clock Geometry and Consistent Five-Dimensional Extensions of Scale Space* (version 1). Zenodo. [doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609). Published; current version.
- **SS-MAT v1** (written "MAT" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MAT: Scale-Extended Matter Sources: Protected Matching, Scale Transport and Completion Gates* (version 1). Zenodo. [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555). Published; current version.
- **SS-PHEN v2**: D. G. Palmer (2026). *SS-PHEN: Experimental Phenomenology of Scale Space: Protected Short-Range Scalar Response, Radiative Null Tests, and Matched Source Corrections* (version 2). Zenodo. [doi:10.5281/zenodo.23868193](https://doi.org/10.5281/zenodo.23868193). Published; superseded by version 3 ([doi:10.5281/zenodo.24044658](https://doi.org/10.5281/zenodo.24044658)).
- **SS-PHEN v3** (written "PHEN" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-PHEN: Experimental Phenomenology of Scale Space: Protected Short-Range Scalar Response, Radiative Null Tests, and Matched Source Corrections* (version 3). Zenodo. [doi:10.5281/zenodo.24044658](https://doi.org/10.5281/zenodo.24044658). Published; current version.

Other working notes referred to by label:

- P1: [WN-01](WN-01_P1Gate.md)
- P4: [WN-15](WN-15_P4CouplingWeight.md)
- P5: [WN-24](WN-24_P5CommonScale.md)
- P6: [WN-16](WN-16_P6ReflectionFold.md)
- P7: [WN-17](WN-17_P7FoldRule.md)
- P8: [WN-22](WN-22_P8CutoffBox.md)
- P9: [WN-23](WN-23_P9FarRegion.md)
- P10: not included in this release.
- P11: original version not included; its revision is WN-18.
- P11Rev: [WN-18](WN-18_P11Rev.md)
