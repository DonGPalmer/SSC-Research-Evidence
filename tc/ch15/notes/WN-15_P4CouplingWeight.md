> **Public edition of evidence note WN-15.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P4CouplingWeight.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `6e45847bf61348be90f32f518807db758ec4d6328cb5d70801741f4f5cc59ca5` (8053 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# P4. What fixes the coupling weight between scale levels

WS1 working note, 8 November 2026. Working material only: not reviewed, nothing published.
Follows [WN-14](WN-14_P3ScaleSpectra.md) (scale spectroscopy). Scripts: `c12_coupling_weight.py`, `c13_weighted_hopping_rank.py` and their outputs (not included in this release).

## 1. Short answer

- The weight cannot be derived from symmetry alone. For every field i the ratio Z_i(X) = G_i/F_i (gradient weight over leaf weight, as a function of the localizer X) is left free by everything checked: protection of the zero mode, gauge invariance, leaf diffeomorphisms, and the ghost-rank test.
- One principle fixes it: every field's scale-derivative term carries the same localizer dependence as its leaf term ("common scale weight", Z_i = constant). SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) already obeys this for gravity: one F(X) multiplies both the leaf curvature and the inter-leaf strain in its action (DYN v6 eq. Sspec).
- Under that principle all sectors get the graviton's operator -F^-1 d(F d), so the spectrum 0 : 3 : 4 (in units c_i^2 kappa^2) is universal across spins. Only the speeds c_i are free, and they drop out of the ratio.
- Correction to P3 §2: this matter result is not new. The Paper-20 [retired series; see References] post-R3 note (26 Aug 2026, §8, §11) already wrote the gauge, Higgs and fermion scale operators with this weight, found 0, 3, 4, and identified the tower at sqrt3 c_i kappa and 2 c_i kappa as the main matter obstruction (too light at the millimetre benchmark unless c_i ~ 1e15 to 1e17). The programme then removed the tower by constraint (P20_CM gate v1; DYN v6 "constrained collective matter").
- Consequence for P2's per-leaf parent: finite hopping mu brings that tower back (c_i^2 grows with mu). The parent is safe only in the mu -> infinity limit (DYN's constrained bundle) or if the common kappa is not at the millimetre benchmark.

## 2. Gravity: why G = F there

DYN v6 continuum action (eq. Sspec):
S = (M5^3/2) ∫ dλ d^4x sqrt(-g) F(X) [ R[g] - c_u^2 (K_{μν}K^{μν} - K^2) ] + localizer terms + S_m.
For the transverse-traceless mode h, R gives (1/4)(∂_x h)^2 and the strain gives (c_u^2/4)(∂_λ h)^2, both multiplied by the same F. Hence G = F for the graviton, and the operator is the l = 2 Pöschl-Teller problem that DYN states (Λ = 0, 3κ², continuum from 4κ²). Note this is fixed by how DYN writes the action (one F in front of the whole bracket); the finite-regulator dRGT links are given X-dependent β coefficients chosen to match it, so it is a definition, not a consequence of the links.

## 3. Matter

### 3.1 The free function
For a field with leaf weight F_i and scale-gradient weight G_i, change of scale coordinate dλ -> J dλ' sends F_i -> F_i J and G_i -> G_i / J. The coordinate-free content is the ratio Z_i = G_i/F_i, i.e. the scale-line metric that field sees. Nothing in the protected construction fixes Z_i:
- protection: the zero mode χ = const solves -F^-1 d(F Z dχ) = 0 for any Z;
- gauge invariance allows any Z(X) F_{λμ}F_λ^μ term;
- ghost test (c13): hopping carried inside each leaf's F-weighted action is rank 2 (ghost-free) at both sample points; the control (hopping across the non-link pair 1-3) is rank 4. Localizer values held at background (not dynamical) here.

### 3.2 Power-law family G = F^a (c12 part A)
Liouville variable z = ∫ sqrt(F/G) dλ = ∫ sech^{2(1-a)} y dy.
- a < 1: z has finite range, so the tower is discrete and trapped. a = 1/2 gives exactly n(n+3) = 0, 4, 10, 18, 28 (box-independent).
- a = 1: z = y, exponential weight: zero mode, one bound state at 3, continuum from 4. The only exponent with both a gap and a continuum.
- a > 1: power-law weight in z, no gap (a = 1.1: eigenvalues fall from 1.49 to 0.67 as the box grows; a = 1.5, 2: all ~0).
So a = 1 is the critical point between a trapped tower and a gapless one.

### 3.3 Interior shape (c12 part C)
G = F(1 + ε sech² y), i.e. Z = 1 + ε sqrt(F) (a function of X): zero mode stays flat, threshold stays 4, but E1 moves:
ε = -0.5, -0.2, 0, +0.2, +0.5, +1.0 gives E1/4 = 0.462, 0.644, 0.750, 0.844, 0.957, >1 (bound state gone).
So the ratio E1/threshold measures Z's shape. 3/4 means Z is constant.

### 3.4 Fermions (c12 part B)
DYN's fermion operator Q = ∂_y + m tanh y has zero mode sech^m y, so |ψ0|² = sech^{2m}. Protection (common envelope F0 = sech⁴) forces m = 2, which gives Q†Q = -∂² + 4 - 6 sech² (the graviton operator exactly) and QQ† = -∂² + 4 - 2 sech² (l = 1: bound 3, continuum 4). Numerics: m = 1.5, 2, 2.5, 3 give E1/threshold 0.889, 0.750, 0.640, 0.556 = (2m-1)/m². With a constant coefficient on the scale derivative, a first-order operator is fixed by its kernel, so for fermions protection alone fixes the tower.
For bosons with G = F the Schrödinger form is the same Q†Q with Q = ∂ - (ln sqrt F)'. So "G = F for bosons" is the same statement as "bosons and fermions share one scale operator": a boson-fermion degeneracy along scale (supersymmetric quantum mechanics structure). This is the cleanest way to state the principle.

## 4. What this does to the scale-spectroscopy claims (P3)

Still stands:
- Spectral ratios as a cross-level test, including the SS-MULTI [v2, doi:10.5281/zenodo.23873325](https://doi.org/10.5281/zenodo.23873325) Example B slope ratios (P3 §5), which do not depend on this question.
- Under the common-scale-weight principle the matter ratio is parameter-free (3 : 4, masses sqrt3 : 2), with the speed c_i dropping out.
- New here: a = 1 is the unique gap-plus-continuum exponent; protection fixes the fermion operator; a non-constant Z shows up as E1/threshold ≠ 3/4.

Withdrawn or qualified:
- P3 §2 said no document applies the l = 2 operator to matter's own spectrum. Wrong: Paper-20 post-R3 note §8 did (gauge, Higgs, fermion), with the same 0, 3, 4.
- The odd state at 3 is reflection-odd. DYN excludes the odd tensor state from the even leaf-metric sector. If matter is treated the same way (reflection as an identification), the bound state is absent and only the threshold 2c_iκ and reflectionless scattering remain as tests. If reflection is only a symmetry, the odd partners exist but are not singly emitted (post-R3 §10 orthogonality rule); pair production is allowed.
- The tower's scale c_iκ is the real issue. At λ_T = 9.9 mm (legacy benchmark), κ ~ 1e-5 eV, so c_i ~ 1 gives meV matter partners; post-R3 §11 needs c_i ~ 1e15 to 1e17 to lift them. DYN v8 treats 9.9 mm as legacy, not a prediction, so a single common κ at a high scale with c_i ≈ c_u is not excluded by this argument. Then the cross-sector prediction would be: matter partners at sqrt3 c_iκ and continuum at 2c_iκ, with c_i = c_u giving the same threshold as the gravity tensor gap. Not checked against data here.

## 5. Open points
1. Whether the common-scale-weight principle follows from a deeper structure (e.g. a supersymmetric or 5D-covariant parent). Not derived here; it is the scale analogue of the equivalence principle.
2. The tower's scale: either constrained away (DYN), lifted by large c_i (unexplained hierarchy), or a single high κ for all sectors (needs a check of the gravity-sector consequences, e.g. the Q pole at about 341κ, and collider limits on pair-produced partners).
3. c13 holds localizer values at the background; a dynamical X_n in the hopping weight is not tested.

## 6. Sources read
- SS-DYN v6 [doi:10.5281/zenodo.23604782](https://doi.org/10.5281/zenodo.23604782) source extract (`foundation_DYN_v6_source_extract.tex`, not included): eq. Sspec, tensor spectrum, constrained collective matter, Q_ψ = D_λ + 2κ tanh y, "unwanted light matter Pöschl-Teller tower".
- P20_CM_gate_v1 (unpublished; not included): constrained matter; earlier gates found matter excitations of order c_iκ.
- P20_post_R3_matter_completion_progress_v1 (unpublished; not included): §6 protection theorem, §8 explicit matter operators (0, 3, 4), §10 orthogonality rule, §11 excitation-scale obstruction.

## 7. Files
- This note. Scripts `c12_coupling_weight.py` and `c13_weighted_hopping_rank.py` (imports `c7_hopping_chain.py`), outputs `c12_out.txt` and `c13_out.txt` (not included in this release).

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v6** (written "DYN v6" in this note): D. G. Palmer (2026). *SS-DYN: A Scale-Localized Leafwise Dynamical Closure for Scale Space: Protected Tensor Gravity, a Repaired Scalar Continuum, and Constrained Collective Matter* (version 6). Zenodo. [doi:10.5281/zenodo.23604782](https://doi.org/10.5281/zenodo.23604782). Published; superseded by version 8 ([doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)).
- **SS-DYN v8** (written "DYN", "DYN v8" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-MULTI v2** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MULTI: Physical Scale as a Location Coordinate: A Multi-Scale Framework in Scale Space* (version 2). Zenodo. [doi:10.5281/zenodo.23873325](https://doi.org/10.5281/zenodo.23873325). Published; current version.
- **Paper 20**: D. G. Palmer (2026). *Paper 20: Dynamical Closure of the Scale-Space Framework: Complex Scale Potential, Newtonian Recovery, and the Hidden Configurational Sector*. Zenodo. Retired series (historical record), replaced by SS-DYN; published versions v2 to v10, the last being version 10, [doi:10.5281/zenodo.21684395](https://doi.org/10.5281/zenodo.21684395). The Paper 20 gate documents this note refers to (for example P20_NS_gate_v1) are unpublished working documents and are not included.

Other working notes referred to by label:

- P2: [WN-04](WN-04_P2Parent.md)
- P3: [WN-14](WN-14_P3ScaleSpectra.md)
