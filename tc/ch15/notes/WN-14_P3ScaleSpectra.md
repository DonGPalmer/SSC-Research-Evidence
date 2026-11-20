> **Public edition of evidence note WN-14.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P3ScaleSpectra.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `3fc5105343e0dea54bc7a8d5731395fcbd14ab45b7e60da91a81022a771480c9` (11615 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** Its §2 novelty claim is withdrawn in [WN-15](WN-15_P4CouplingWeight.md), and its odd √3 partner and 3 : 4 test are found not observable under the scale fold in [WN-15](WN-15_P4CouplingWeight.md) and [WN-16](WN-16_P6ReflectionFold.md). Editorial notes mark the affected passages; the original wording is kept.

# SS WS1 P3: scale spectroscopy, a cross-level test from the spectrum along scale

Date: 8 November 2026. Status: **draft for the author's review. Not independently reviewed.**
Done on the author's instruction (8 Nov 2026): "Yes to writing up and run the same test. Then progress 'What's new is using the spectral ratios as the test across levels.'" Asked after "Can you find a conceptual tool that can cross levels of scale and be better than multi-scale modeling?" Follows [WN-04](WN-04_P2Parent.md) (WS1).
Labels as in [WN-01](WN-01_P1Gate.md): [Derived], [Computed], [Literature], [Assumed], [Conjecture]; [Read] = stated in the named document.

## 1. Short answer
- **The tool.** Treat everything that links levels as one operator along the scale coordinate u, and read predictions from its spectrum. Multi-scale modeling fits a handoff rule between each pair of levels; here the handoffs are the matrix elements of one operator, so the *ratios* between cross-level rates are fixed in advance. Each fixed ratio is a restriction that can fail on withheld data.
- **Per-leaf parent (P2), protected weight F = sech⁴.** The scale operator is the ℓ = 2 Pöschl–Teller (kink) operator: a shared mode at 0, one odd mode at 3, a continuum from 4, reflectionless [Derived; Computed C9, C10]. The ratio 3 : 4 holds for any coupling strength and measures the exponent of F directly.
- **SS-MULTI v2 [doi:10.5281/zenodo.23873325](https://doi.org/10.5281/zenodo.23873325) Example B.** At zero spatial wavenumber the scale rates are 0, γ, 2γ, … (set by the Gaussian carrier, not by the geometry). Their spatial slopes D_n are fixed by the single number b = |β|s, e.g. D₁/D₀ = 1 + b², D₂/D₀ = 1 + 2b² + b⁴/2 [Derived; Computed C11]. With s measured from the carrier's moments and β = 2, no slope ratio is free. This measures β without the reaction kinetics, which the threshold test of SS-MULTI §11.5 cannot do.

## 2. What the corpus already has (so the novelty claim is narrow)
- **Graviton spectrum.** The ℓ = 2 Pöschl–Teller operator with Λ = 0, 3κ², continuum ≥ 4κ², gap 2(c_u/c_T)κ is in the Paper 20 [retired series; see References] line: v13 internal audit eqs. 10–13; Dirac gate v1 §5; EFT/static-continuum gate v1 §2 (which calls it reflectionless). SS-DYN v8 [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) §4 uses K̂ = −∂y² + 4 − 6 sech²y in its odd scalar pencil [Read, via a helper's reading; not re-read line by line here].
- **Matter.** SS-MAT [v1, doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555) step 7 uses the K̂ continuum for matter-source overlaps. The 30 Oct SS-MAT audit finds that a 5D backreacted bulk scalar has no Pöschl–Teller well and a gapless continuum [Read, helper]. This matches C9(C) below.
- **SS-GEO v6 [doi:10.5281/zenodo.23603029](https://doi.org/10.5281/zenodo.23603029)** already compares holographic RG, cMERA, Fisher geometry and Kron/Dirichlet-to-Neumann reduction (§1.2, §6–8) [Read].
- **SS-MULTI v2** already expands along u in Hermite modes of a Gaussian carrier, with K_nm, the Mehler kernel and a Mori–Zwanzig reduction (§10.4–10.5), and states that without "an extra tested restriction" the description is "a useful representation without demonstrated additional physical content" (§11.7); feature (v) of §11.6 is "absent for every candidate" [Read, helper].
> **Editorial note (public edition, 19 November 2026):** A later note finds that the first item below is not new: the Paper 20 post-R3 note (26 August 2026, §8) had already applied the ℓ = 2 operator to gauge, Higgs and fermion matter, with the same levels 0, 3, 4, so that part of the novelty claim is withdrawn. The same note keeps the use of spectral ratios as a cross-level test. See [WN-15](WN-15_P4CouplingWeight.md) §4. The text below is unchanged from the working note.

- **Not in the corpus, as far as the searches went:** the same operator governing per-leaf *matter* in a ghost-free parent; spectral *ratios* used as an observable test; the observation that SS-MULTI's carrier and DYN's protected weight are the same construction.

## 3. One construction behind DYN and SS-MULTI [Derived]
For a profile weight F(u) (the protected weight in DYN, the carrier φ₀ in SS-MULTI) and a level-coupling weight G(u), the scale-mode operator is
  L χ = −(1/F) ∂_u (G ∂_u χ).
- With G = F the constant is always an exact zero mode (the "shared mode", the protected source of P2). Substituting χ = ψ/√F gives −ψ″ + V ψ with V = (√F)″/√F.
- **F = sech^{2q} u:** V = q² − q(q+1) sech² u, Pöschl–Teller ℓ = q. Bound E_n = q² − (q−n)², n < q; continuum from q²; reflectionless for integer q.
- **F Gaussian (u₀, s):** the operator is (1/s²) × the Ornstein–Uhlenbeck generator of SS-MULTI eq. 23 with the sign flipped; E_n = n/s².
- So the low spectrum identifies the profile shape: equal spacing for a Gaussian carrier; 0, 2q−1, …, threshold q² for sech^{2q}. The ratio of the first excited level to the threshold, (2q−1)/q², is 3/4 for sech⁴ and 5/9 for sech⁶; sech² has no excited level.

## 4. Test 1: the per-leaf parent, F = sech⁴ (C9, C10)
| Link (gradient) weight G | Spectrum on a refined lattice | Reading |
|---|---|---|
| G = F (sech⁴) | 0 (exact, flat), 3.0006, continuum from 4; box independent | Pöschl–Teller ℓ = 2; mode 1 = sinh u (rel. diff 4.5×10⁻⁴) |
| G = 1 (uniform hopping) | 4.62, 14.3, 29.0 … discrete, no continuum | every massive mode trapped near the central leaf |
| G = F² (5D bulk scalar) | gapless, many modes near 0 | outer leaves decouple; matches the 30 Oct SS-MAT audit |
| DYN's 3 leaves (u = −1, 0, 1), G = F | 0, 3.51, 4.74 | a coarse lattice of 0, 3, 4 |

- Family check (C10): q = 1, 2, 3 reproduce E_n = q² − (q−n)² and the continuum q²; E₁/threshold = 0.7500 (q = 2) and 0.5556 (q = 3), exact.
- Reflection (C10): |R|² ≈ 10⁻²⁶ for V = 4 − 6 sech² at E = 4.5, 6, 10; the control V = 4 − 5 sech² gives 1.8×10⁻² at E = 4.5.
- Units: E is mass² in units of (c_u κ)², c_u the propagation speed along scale of the hopping term. Only ratios are fixed; the absolute scale is not [Derived].

> **Editorial note (public edition, 19 November 2026):** Later notes find that the odd partner at 3 (items 2 and 3 below) is reflection-odd: if the scale reflection is a fold, which the second of those notes recommends, this state is absent and only the threshold and reflectionless scattering remain as tests; if the reflection is only a symmetry, the odd partners exist but are not singly emitted. See [WN-15](WN-15_P4CouplingWeight.md) §4 and [WN-16](WN-16_P6ReflectionFold.md) §7.3. The text below is unchanged from the working note.

**What this predicts for the parent [Derived, conditional on G = F]:**
1. Exactly one matter mode is shared identically by every level (ordinary matter, protected source).
2. The first heavy matter partner and the start of the heavy continuum are in mass ratio √3 : 2 (0.866), whatever the hopping strength.
3. The first partner is odd across the central leaf (χ ∝ sinh u), so a source symmetric about the central leaf cannot excite it at linear order.
4. Heavy-continuum disturbances cross the central leaf without reflection.
5. Same operator as the graviton (Paper 20). If matter and gravity hop along scale at the same speed (c_u equal), their spectra coincide level by level [Conjecture: whether c_u is shared is not fixed anywhere].

## 5. Test 2: SS-MULTI v2 Example B (C11)
Model: SS-MULTI eq. 23, ∂_t c̃ = D e^{−βu} ∂_x² c̃ + 𝓛⁺ c̃ + R, with the reaction switched off (a passive tracer). At spatial wavenumber k the decay rates are the eigenvalues of A(k) = γ diag(n) + D k² K, K_nm = ∫ φ₀ h_n e^{−βu} h_m du (SS-MULTI eq. 37), h_n = He_n/√n!.

| (β, s) | b = βs | k = 0 rates | D₁/D₀ | D₂/D₀ | D₃/D₀ |
|---|---|---|---|---|---|
| (2, 0.30) | 0.60 | 0, 1, 2, 3 (×γ) | 1.36000 | 1.78480 | 2.28217 |
| (2, 0.15) | 0.30 | 0, 1, 2, 3 | 1.09000 | 1.18405 | 1.28227 |
| (1, 0.60) | 0.60 | 0, 1, 2, 3 | 1.36000 | 1.78480 | 2.28217 |
| (0, 0.30) | 0 | 0, 1, 2, 3 | 1 | 1 | 1 |

- Closed form [Derived]: D_n/D₀ = (1/n!) Σ_j C(n,j)² j! b^{2(n−j)}; the numerics agree to 10⁻⁵ (24 modes, N_quad = 200).
- The k = 0 ratios 1 : 2 : 3 come from the Gaussian/OU carrier, an assumption of SS-MULTI. They test the carrier, not the geometry.
- The slope ratios carry the geometry through b = βs. With s from the carrier's moments (SS-MULTI §10.1: s² = m₂/m₀ − u₀²), |β| = √(D₁/D₀ − 1)/s, and D₂/D₀, D₃/D₀ are then pure predictions.
- Side result: the slow mode's k⁴ coefficient with all modes is −0.1144 at (β, s) = (2, 0.3) (u₀ = 0.4, D = γ = 1); SS-MULTI eq. 40's one-mode form gives −0.1042, 9% low. The paper's thresholds use N = 8 modes, so its Table 2 is unaffected [Computed].

## 6. The spectral-ratio test as a method
1. **Write the scale operator.** Profile weight F, level-coupling weight G, and the spatial term with its geometric exponent (β = 2 in SS).
2. **Separate what is assumed from what is geometric.** The k = 0 spectrum depends on the profile shape (F, G): its ratios test the carrier or the protected weight. The k-dependence (slope ratios D_n/D₀, mixing) depends on β: it tests the SS geometry.
3. **Fix everything before calibration.** Profile width from moments; shape class declared (Gaussian, sech^{2q}). Then only an overall rate (γ or c_uκ) and an overall diffusivity D remain free.
4. **Count restrictions.** With M measured rates or slopes and two free scales, there are M − 2 parameter-free predictions.
5. **Compare with the matched conventional model.** A hierarchical or latent-variable model with free relaxation rates per level has no ratio restriction. A latent-variable model with a measured D(ℓ) ∝ ℓ^{−β} law and an OU latent variable reproduces C11's slope ratios exactly with β free; SS adds the fixed value β = 2 [Derived]. Whether that alone meets SS-MULTI §11.6 feature (v) ("a stated Scale Space relation that the conventional model does not already contain") is a ruling for the author; §11.7 already notes that a free-exponent comparator imposes cross-scale relations [Read, helper].

> **Editorial note (public edition, 19 November 2026):** Later notes find that the 3 : 4 ratio in item 6 below is not observable if the scale reflection is a fold, which the second of those notes recommends: only P-even levels remain, so for the ℓ = 2 operator the cross-level test becomes the same threshold in every sector, and discrete ratio tests need operators with two or more even bound levels (ℓ ≥ 3). See [WN-15](WN-15_P4CouplingWeight.md) §4 and [WN-16](WN-16_P6ReflectionFold.md) §7.3. The text below is unchanged from the working note.

6. **Where the SS content is stronger.** In the DYN parent the ratio 3 : 4 follows from the exponent 4 of the protected weight, which the corpus derives from the warp e^{𝒜} = sech² (F₀ = e^{2𝒜}). A conventional multi-level model has no reason for that ratio [Derived; the warp itself is DYN's input].

**Advantage over the §11.5 threshold design [Derived]:** the threshold depends on the kinetics, needs (u₀, s, γ) calibrated and may not be injective (Prop. 2, 3). The passive slope ratio needs no kinetics, depends on |β|s alone, and is monotone in it, so it identifies |β| directly once s is measured.

## 7. Open points
- **G = F is a choice.** It is what makes the parent's matter operator equal the graviton's, and it gives a gap; uniform hopping (G = 1) and the 5D bulk scalar (G = F²) do not. Nothing yet derives G from an action. This is the main open link [Conjecture].
- **Absolute scale.** Only ratios are fixed; c_u and κ are not.
- **Measurability.** No system in the corpus has scale-resolved rate measurements. For Example B the design needs a passive tracer with resolved scale modes at two or more spatial wavenumbers.
- **Nonlinear and multi-field.** Linear, single scalar only; fermions and gauge fields untested (as in P2).
- **Prior art outside the corpus.** Pöschl–Teller and OU spectra are standard. The novelty claim is limited to their use as a cross-level test inside SS; no literature search for that was done.

## 8. Correction to [WN-04](WN-04_P2Parent.md) §2
[WN-04](WN-04_P2Parent.md) says of SS-L5D [v1, doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609): "the extra coordinate is clock time, not scale". That is wrong. In SS-L5D scale u is the fourth dimension (with the three space directions it forms the 4D configuration space) and clock time t is the fifth (the author, 8 Nov 2026: "SS-L5D should have scale as the fourth D"). The vacuum lapse N = e^u gives a Poincaré patch of AdS₅ (warp e^u, not DYN's sech²); its (t, x, u) geometry is the natural continuum that DYN's leaves would discretise [Conjecture]. [WN-04](WN-04_P2Parent.md) is left unchanged; this section records the correction.

## 9. Files
- This report: [WN-14](WN-14_P3ScaleSpectra.md) (working file `SS_WS1_P3_scale_spectroscopy_2026-11-08_v1.md`, not included).
- Scripts and outputs (not included in this release):
  - `c9_scale_spectrum.py` (not included) / `c9_out.txt` (not included): scale spectrum for G = F, 1, F²; DYN's 3 leaves.
  - `c10_spectral_rigidity.py` (not included) / `c10_out.txt` (not included): sech^{2q} family, Gaussian carrier, reflection test.
  - `c11_exampleB_spectral.py` (not included) / `c11_out.txt` (not included): SS-MULTI Example B slope ratios and k⁴ term.
- Requirements: Python 3, numpy.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-GEO v6**: D. G. Palmer (2026). *SS-GEO: Logarithmic Scale as a Geometric Coordinate: Exact-Distance Projection and Radial Scale Response* (version 6). Zenodo. [doi:10.5281/zenodo.23603029](https://doi.org/10.5281/zenodo.23603029). Published; current version.
- **SS-L5D v1** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-L5D: Clock Geometry and Consistent Five-Dimensional Extensions of Scale Space* (version 1). Zenodo. [doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609). Published; current version.
- **SS-MAT v1** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MAT: Scale-Extended Matter Sources: Protected Matching, Scale Transport and Completion Gates* (version 1). Zenodo. [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555). Published; current version.
- **SS-MULTI v2**: D. G. Palmer (2026). *SS-MULTI: Physical Scale as a Location Coordinate: A Multi-Scale Framework in Scale Space* (version 2). Zenodo. [doi:10.5281/zenodo.23873325](https://doi.org/10.5281/zenodo.23873325). Published; current version.
- **Paper 20**: D. G. Palmer (2026). *Paper 20: Dynamical Closure of the Scale-Space Framework: Complex Scale Potential, Newtonian Recovery, and the Hidden Configurational Sector*. Zenodo. Retired series (historical record), replaced by SS-DYN; published versions v2 to v10, the last being version 10, [doi:10.5281/zenodo.21684395](https://doi.org/10.5281/zenodo.21684395). The Paper 20 gate documents this note refers to (for example P20_NS_gate_v1) are unpublished working documents and are not included.

Other working notes referred to by label:

- P2: [WN-04](WN-04_P2Parent.md)

Material named in this note but not included in this release: `SS_WS1_P3_scale_spectroscopy_2026-11-08_v1.md`, `c10_out.txt`, `c10_spectral_rigidity.py`, `c11_exampleB_spectral.py`, `c11_out.txt`, `c9_out.txt`, `c9_scale_spectrum.py`.
