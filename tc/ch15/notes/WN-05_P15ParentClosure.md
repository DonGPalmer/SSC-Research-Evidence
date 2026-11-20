> **Public edition of evidence note WN-05.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P15ParentClosure.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `7d01a89a09c930b3d58e80a097a5a5f782c6bc72b9d4fc5a4aeb964eb9a431ad` (8752 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** Its conclusion that the parent "fails as a natural theory" is withdrawn in [WN-08](WN-08_P18RegulatedLoop.md). An editorial note marks the affected passage; the original wording is kept.

# SS WS1 P15: Priority 1 test of the per-leaf matter parent (P2)

Date: 8 November 2026. Status: **draft for the author's review. AI calculation, not independently reviewed.**
Done on the author's instruction "Please proceed with Priority 1" (8 Nov 2026), Priority 1 being from a review of WS1 P1–P13 made the same day (another Claude session's read-only review, not an external review). No canonical file is changed; this note proposes nothing for SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296).
Labels: [Derived], [Computed], [Assumed], [Conjecture], [Literature, not re-derived].

## 1. Verdict
> **Editorial note (public edition, 19 November 2026):** A later working note withdraws the verdict below that the per-leaf parent "fails as a natural theory", and the one-loop leaf-weight figures behind it, because they came from counting every matter copy equally in the loop; with a regulated loop it finds the parent radiatively stable while the cutoff stays within a few copy masses, an EFT condition. The same note also limits the tree rule and the "to all orders" tree-level truncation to the cases tested, and marks the Y = 8 rows as numerically unstable. See [WN-08](WN-08_P18RegulatedLoop.md), section "Corrections to P15 and P17". The text below is unchanged from the working note.

**P2's per-leaf parent fails Priority 1 as a natural theory.** The constraint structure holds where tested and the protected source survives integrating out the heavy matter copies at tree level, exactly and to all orders. But one-loop corrections regenerate leaf weights that are not proportional to F, so protection survives only with a separate fine-tuning on every leaf, and the matter copies are strongly coupled on most of the scale box.

| Test | Result |
|---|---|
| Constraint closure, homogeneous sector, fully nonlinear, variable F(X_n) | Pass: secondaries close, no tertiaries, 6 dof = the leaf scalars only [Computed C23] |
| Same with hopping that closes a loop (1–3) | Fail: 7 dof, one extra (Boulware–Deser-type) mode [Computed C23] |
| Inhomogeneous closure with shifts | Not shown. Only C7's primary (Hessian-rank) test exists |
| Protection after removing heavy copies, tree level | Pass, exact to all orders, any static localizer background [Derived; Computed C24 §2] |
| Protection at one loop | Fail: generated leaf weights vary by up to 10^13 (quadratic) and 10^16–10^29 (log) relative to F on the Y = 8 box [Computed C24 §3] |
| Matter boundary condition at the box ends | Must be Neumann (free ends) for plain hopping; Dirichlet leaks [Computed C24 §1] |
| Copies' coupling | Strongly coupled for \|y\| ≳ 1.1–1.7; grows as cosh⁴y, 5 × 10^12 at Y = 8 [Computed C24 §4] |

## 2. The action tested
Leaf n (n = 1…N on a chain), M₅³ = 1:
- gravity F(X_n)√−g_n R[g_n]/2 (variable localizer weight, non-minimal);
- localizer Z(∂X_n)²/2 + U(X_n), gradient κ(X_n − X_m)²/2 on linked pairs with split leaf measure;
- matter F(X_n)√−g_n[−(∂φ_n)²/2 − V(φ_n)], V = m²φ²/2 + gφ⁴ (P2 case 1);
- hopping (μ/2)W_e(φ_n − φ_m)² with measure (√−g_n + √−g_m)/2 on linked pairs only (P2 measure (a));
- links: minimal square-root (dRGT-type) terms m²Σβ_k c_k[e_n, e_m], β chosen tadpole-free at e_n = e_m with positive Fierz–Pauli sign (β₃ = 0, β₂ = 1, β₄ = 1/5).
The Hamiltonian is Σ_n N_n C_n, linear in every lapse [Computed check]. Numbers (Z = 3/2, λ = 1/2, κ = 9/10, m² = 7/10, μ = 13/10, matter mass² 1/3, g = 1/10) are generic test values.

## 3. Constraint closure (C23)
Homogeneous, isotropic sector (lapses N_n, scale factors a_n, X_n, φ_n), fully nonlinear, 3 leaves; Dirac algorithm on random points of the constraint surface (residual < 10⁻³⁰).
- On a chain, {C₁, C₃} = 0 identically. Consistency gives two secondaries {C₁,C₂}, {C₂,C₃}; their consistency fixes the lapse ratios (rank 2), so there are no tertiaries. The 5 × 5 bracket matrix has rank 4, leaving one first-class constraint (time reparametrisation). Count: (18 − 2 − 4)/2 = 6, one X_n and one φ_n per leaf; gravity carries no homogeneous mode [Computed, 3 points each].
- F-weighting does not matter here: unweighted matter on the chain also gives 6.
- Hopping 1–3 (not a gravitational link) makes {C₁, C₃} ≠ 0, the bracket matrix has rank 2 of 3, and the count is 7: an extra scale-factor mode, the homogeneous face of C7's control ghost [Computed, 4 points].
- **Rule [Derived]:** the union of gravitational links and matter hopping must be a tree (here: the chain itself). Every hopping term is shift-free and linear in a single lapse, so it changes C_n but not the lapse–shift structure; that is why the chain survives and a loop does not.
- Not shown: the inhomogeneous field theory (shifts, secondary constraint's spatial propagation). For chains of square-root vielbein links this closure is the standard expectation [Literature, not re-derived]; P2's matter terms do not touch shifts, but a proof for this system is still owed.

## 4. Does the protected source survive removing the heavy copies? (C24)
Scale box |y| ≤ Y, Δy = 0.05, leaf weights F_n Δy (Σ = 4/3), gravity links μ_e = sech⁴(y_e)/Δy (NS gate conventions). Graviton modes F-orthonormal; leakage and α = (4/3)ΣJ_a²/J₀² as in C8.

**Tree level: pass [Derived; Computed].** With kinetic and potential both weighted by F_n and hopping vanishing on the flat configuration, φ_n = φ for all n is a consistent truncation: every vertex with light legs and a single heavy leg is ∝ Σ_n F_nΔy u_k(n) = 0 (computed 10⁻¹³ at Y = 4, 10⁻⁹ at Y = 6; Y = 8 is beyond double precision). It stays exact for a deformed localizer background F(X₀ + 0.3ξ) (10⁻¹²). So integrating out the heavy copies at tree level adds nothing to the light sector: the effective theory is (ΣF_n)S[g, φ], DYN v8's printed coupling, to all orders in the fields, for any static localizer. This also needs the gravity weight per leaf to be F_n with no extra w_n; DYN v6's w_n, a_n³ weights (not read) would have to match the matter weight exactly.

What breaks it at tree level is only the localizer moving: then φ's equation on leaf n picks up ∂ln F(X_n)·∂φ, leaf-dependent, so the light mode mixes with heavy copies through the gapped localizer (M⊥) channel. Its leaf factor f/F = −4 tanh y cosh²y grows like e^{2|y|}, the same regulator-box growth as P8 [Derived].

**One loop: fail [Computed].** A gφ⁴ term on each leaf generates per-leaf counterterms for φ²:
- quadratic divergence c_n ∝ F_nΔy Σ_k u_k(n)² = 1 on every leaf (uniform, not ∝ F);
- log divergence (scheme-independent) c_n ∝ F_nΔy Σ_k m_k² u_k(n)² = H_nn/(F_nΔy).

| Generated term (Y = 8) | c_n/(F_nΔy), centre .. edge | α of that term |
|---|---|---|
| quadratic, either hopping | 20 .. 9.9 × 10^13 | 1.9 × 10^10 (same as unweighted matter) |
| log, hopping W_e = 1 | 1.6 × 10^4 .. 2.6 × 10^29 | 5 × 10^12 |
| log, hopping W_e = F(y_e) | 1.6 × 10^4 .. 6.5 × 10^16 | 1.7 × 10^10 |
(Y = 4: α 8.4 × 10^3 to 5.8 × 10^5; Y = 6: 1.1 × 10^7 to 1.7 × 10^9. The α values are box-dependent and edge-dominated, like P8; their size only says the violation is not small.)

Nothing in the parent forces counterterms to be proportional to F(X_n): X_n is a field, and any G(X_n)√−g_n φ_n² is allowed. So keeping the source protected requires one fine-tuning per leaf, and the parent does not explain why matter couples with weight F; it imposes it.

**Matter boundary condition [Computed].** Free (Neumann) ends keep the flat mode exact. Dirichlet ends with plain hopping leak strongly (α = 208 at Y = 4, 1.2 × 10^5 at Y = 6). With F-weighted hopping the ends barely matter (α ≈ 10⁻⁵ at Y = 4, 10⁻¹² at Y = 8).

**Copies' coupling [Computed].** Canonically normalised, the quartic on leaf n is λ_light·W/(F_nΔy). With Δy = 0.05 copies are strongly coupled (λ_n > 16π²) for |y| ≥ 1.70 (λ_light = 0.1) or 1.05 (λ_light = 1). The grid-free part is cosh⁴y: 5.6 × 10^5 at Y = 4, 4.9 × 10^12 at Y = 8. F-weighted gauge copies would scale the same way [Derived; untested]. The one-loop numbers above are therefore only indicative outside the core.

## 5. What this means
- P2's construction explains DYN v8's printed matter coupling as a tree-level, low-energy statement, and its constraint structure is sound on a chain. It does not supply a reason for the weighting that survives quantum corrections.
- A parent that passes would need a symmetry, or a 5D origin, that makes "matter weight = gravity weight = F" exact. P2 §4 already showed a plain 5D bulk scalar fails at the mass term (α ≈ 0.07); this note shows the discrete per-leaf version fails radiatively.
- Neither result changes the established restricted common-metric theory (DYN v8 as restricted reference model).
- Suggested next step, not started: test whether a box confined to the weakly coupled core (|y| ≲ 1.5) changes the one-loop verdict, or look for a symmetry that ties matter and gravity weights.

## 6. Files
- Scripts and outputs (not included in this release): `c23_dirac_minisuperspace.py` (not included) / `c23_out.txt` (not included) (Python 3, sympy, mpmath; ~15 min); `c24_protection_box.py` (not included) / `c24_out.txt` (not included) (numpy).

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v6** (written "DYN v6" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: A Scale-Localized Leafwise Dynamical Closure for Scale Space: Protected Tensor Gravity, a Repaired Scalar Continuum, and Constrained Collective Matter* (version 6). Zenodo. [doi:10.5281/zenodo.23604782](https://doi.org/10.5281/zenodo.23604782). Published; superseded by version 8 ([doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)).
- **SS-DYN v8** (written "DYN v8" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.

Other working notes referred to by label:

- P1: [WN-01](WN-01_P1Gate.md)
- P2: [WN-04](WN-04_P2Parent.md)
- P8: [WN-22](WN-22_P8CutoffBox.md)
- P13: [WN-21](WN-21_P13L5DScaleGeometry.md)

Material named in this note but not included in this release: `c23_dirac_minisuperspace.py`, `c23_out.txt`, `c24_out.txt`, `c24_protection_box.py`.
