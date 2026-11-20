> **Public edition of evidence note WN-01.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P1Gate.md`, a working note dated 7 November 2026. Not peer reviewed.
> - **Source content hash:** `34fa33a47e090e60d71202c51a2bcc9bc80b3d7dd33c10ad5cb6c8e247c058f7` (11539 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# SS WS1 P1: MAT–DYN parent-coupling gate (two-leaf test)

Date: 7 November 2026. Status: **draft for the author's review. Not independently reviewed.**
Prepared by: Claude (one session), on the author's instruction "Start MAT-DYN work" (7 Nov 2026).

Epistemic labels used below:
**[Derived]** shown analytically here. **[Computed]** shown by exact-rational or 40-digit numerics in the attached scripts, at the stated sample points (not a general proof). **[Literature]** taken from a cited paper; abstract checked, full argument not re-derived here. **[Assumed]** a modelling choice made to run the test. **[Conjecture]** a statement I believe but have not shown.

---

## 1. What MAT–DYN asks (source)

Source: `SS_P1_scale_velocity_route_closed_20261106.md` (not included), §4, rank 1 (supported by `SS_PhaseB5_parent_answer_20261105.md` (not included), the five bounded next actions, and `SS_WS1_closure_recommendations_2026-10-24_v1.md` (not included)).

In my words: declare one corrected, fully specified common-parent or two-site matter action; do the full inhomogeneous lapse/shift constraint analysis (Dirac rank, plus secondary and tertiary closure); check it keeps exactly the intended tensor and matter modes; and report a positive or negative outcome, not only a toy Hessian.

Dependencies:
- **SS-DYN v8 [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)** (`SS-DYN_leafwise_dynamical_closure_v8.tex` (LaTeX source of SS-DYN v8; not included)): the finite common-metric multiplet is the restricted reference model; its section "Why the full parent remains open" records that the printed shared-matter coupling H = Σ N_n C_n + p²/(2K), K = Σ c_n/N_n, has a relative-lapse Hessian of rank N−1 (the D3a obstruction).
- **Framework v21 [doi:10.5281/zenodo.23840776](https://doi.org/10.5281/zenodo.23840776)**: not checked in this package (see §7).
- **SS-MAT v1 [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555)**: not read in this package (see §7).

## 2. The test

Two leaves (N = 2), each with its own metric written in vielbein (ADM upper-triangular) form, linked by the standard square-root (dRGT/vielbein) potential, i.e. the independent-leaf parent with minimal links. The gravity sector alone is the Hinterbichler–Rosen vielbein theory, whose Hamiltonian is linear in the lapses after the boost/shift redefinition **[Literature]**. The question is only which **matter coupling** keeps that structure.

Gate used (standard argument): with the symmetric-vielbein condition, the relative shift is s1 = s2 + (N1/A1 + N2/A2) tanh w, where w is the relative Lorentz boost **[Derived; Computed C1]**. The Hamiltonian then has the form Σ N_i C_i(w) + (shift terms) at fixed w. Eliminating w by its own equation keeps lapse-linearity iff that equation factors as (N1/A1 + N2/A2)·F(w). Lemma **[Derived]**: if H = Σ N_i C_i(w) and w* solves Σ N_i C_i'(w) = 0, the reduced lapse Hessian is −c cᵀ / (Σ N_i C_i''(w*)) with c_i = C_i'(w*); it vanishes iff c = 0, i.e. iff the factorization holds. A non-zero (rank-1) reduced Hessian means the lapses no longer give a Hamiltonian constraint, so the Boulware–Deser mode returns in this parametrization.

Three matter couplings were declared **[Assumed: these three]**:

| Label | Matter coupling | Why considered |
|---|---|---|
| M0 | The printed shared scalar: one field with weights c_n = w_n F0n a_n³ on every leaf (DYN v8 form) | It is what DYN v8 prints |
| M1 | Matter on a single leaf, or separate matter fields each on its own leaf | Standard ghost-free bimetric choice |
| M2 | Composite vielbein metric e_eff = b1 e1 + b2 e2 (de Rham–Heisenberg–Ribeiro) | The only candidate that couples one field to both leaves non-trivially |

Matter used in the tests: one scalar with kinetic momentum P, gradient φ' (planar, along x) and potential V. Pointwise algebra; gradients enter as numbers.

## 3. Results

### 3.1 M0, printed shared scalar: fails
- Homogeneous relative-lapse Hessian has rank N−1 (= 1 for N = 2), reproducing D3a **[Computed C3(C)]**.
- Including the shifts, the 4×4 Hessian in (N1, N2, N1ˣ, N2ˣ) has rank 1, also for P = 0 or φ' = 0 alone **[Computed C3(C)]**.
- Conclusion: the printed coupling is not a consistent parent coupling. This confirms, it does not change, the DYN v8 statement.

### 3.2 M2, composite metric: passes the easy checks, fails the decisive one
- At fixed boost, det e_eff, the effective lapse, the effective shift and the matter Hamiltonian are all linear in N1, N2 (boosts v = 0, 5/13, 3/5) **[Computed C1]**.
- With b_n ∝ M_n² (the gravitational kinetic weights) the composite gives exactly the **protected linear source**: matter couples only to the massless mode **[Derived; Computed C3(D)]**. So M2 is the coupling that would match DYN v8's protected weights.
- But the boost equation does **not** factor once matter has kinetic or gradient terms: Q = (∂H/∂w)/(N1/A1 + N2/A2) depends on the lapse ratio (e.g. at tanh(w/2) = 1/2: Q = −0.380, −0.160, −0.653, −0.189 at four lapse ratios) **[Computed C2]**. Gravity potential terms, the leaf momentum terms and the matter potential term alone do factor **[Computed C2]**.
- After eliminating the boost, the reduced lapse Hessian is (3.98, −3.98, 3.98)×10⁻² (rank 1); for gravity alone, or matter on either single leaf, it is zero to 10⁻²⁸ **[Computed C3(A)]**.
- The failure holds for every mixed weight tested (b = 3/20:17/20, 1/2:1/2, 17/20:3/20, 1:1/1000); only the single-leaf limits b = (1,0) or (0,1) pass **[Computed C4]**.
- Conclusion: in the standard parametrization the composite coupling **loses the Hamiltonian constraint on generic inhomogeneous matter data**. Homogeneous (w = 0) configurations pass, which is why a homogeneous toy would not see this.
- Agreement with literature: de Rham, Heisenberg, Ribeiro, PRD 90 124042 (2014), arXiv:1409.3834, find the constraint is lost on generic backgrounds and the ghost returns above the strong-coupling scale **[Literature]**. Their earlier CQG 32 035022 (2015), arXiv:1408.1678, shows ghost-freedom in representative limits and conjectures the general case **[Literature]**.
- Tension: Hassan, Kocic, Schmidt-May, arXiv:1409.1909, claim ghost-freedom from a nonlinear Hamiltonian analysis in different variables **[Literature]**. I have not resolved that tension, so I do not exclude a rescue by a different choice of variables. Huang, Ribeiro, Xing, Zhang, Zhou, arXiv:1505.02616, argue the composite is the unique consistent non-minimal coupling *below* the strong-coupling scale **[Literature]**. The honest reading is: M2 is acceptable only as an effective theory with a cutoff, not as a full parent.

### 3.3 M1, single-leaf (or one-field-per-leaf) coupling: passes, but loses the protected source
- Boost equation factors; reduced lapse Hessian zero to 10⁻²⁸ for matter on leaf 1, on leaf 2, or separate fields on both **[Computed C3(A,B)]**.
- Full secondary/tertiary closure then follows from the published Hassan–Rosen / Hinterbichler–Rosen constraint analysis for minimally coupled matter **[Literature; not re-derived here]**.
- Cost: matter sources the massive spin-2 modes. For N = 2 with matter on leaf 1, the massive/massless strength ratio is M2²/M1² (×4/3 from the massive tensor structure: a Yukawa correction to Newtonian gravity) **[Derived; Computed C3(D)]**.
- For the 3-site chain with sech⁴ weights and matter on the central leaf, the short-range/long-range scalar-exchange strength ratio is ΣM²/M_c² = **1.3528** **[Computed C3(D)]**. That is an O(35%) short-range modification, which fifth-force tests bound strongly unless the Yukawa range (set by the massive-mode masses) is very short.
- Conclusion: M1 is the consistent parent coupling in this test, but it does not reproduce DYN v8's protected weights.

### 3.4 Summary table

| Coupling | Lapse-linear (fixed boost) | Boost eq. factors | Reduced Hessian | Protected source | Verdict |
|---|---|---|---|---|---|
| M0 printed shared scalar | No | n/a | rank 1 (N−1) | n/a | Fails |
| M1 single leaf / per-leaf fields | Yes | Yes | 0 | No (Yukawa, ratio 1.35 for 3-site chain) | Passes, loses protection |
| M2 composite, b ∝ M² | Yes | No (kinetic, gradient) | rank 1 | Yes | Fails as full parent; EFT only |

**Main result [Computed for N = 2; Conjecture for general N]:** within the minimal-link independent-leaf parent, no tested matter coupling is both ghost-free and protected. Protection needs matter on a weighted combination of leaves; ghost-freedom needs it on one leaf. This is a model-specific obstruction, which is the outcome B5 action 5 provides for (recording a model-specific obstruction).

## 4. Consistency with DYN v8
- DYN v8's common-metric multiplet remains valid as the restricted reference model; nothing here contradicts it **[Derived from §3]**.
- DYN v8's statement that the full parent is open is sharpened: the printed coupling fails (as DYN v8 says), the natural repair (composite) fails in the standard analysis, and the ghost-free repair (single leaf) gives up the protected weights.
- What DYN v8 claims about protected weights F0 = sech⁴ at the parent sites holds for the linear source only **[Derived]**; it has no nonlinear ghost-free completion among the three couplings tested.

## 5. Assumptions to flag
1. Localizer kinetic terms are site-local, and link or gradient terms use det-type measures **[Assumed]**.
2. Minimal square-root links only; non-minimal or non-nearest-neighbour links not tested **[Assumed]**.
3. Planar symmetry with shift along x only; pointwise algebra **[Assumed]**. A failure at a generic sample point suffices for M2; the passes for M1 are numerical at sample points plus the published theorem.
4. N = 2 computed; N-site chain left open.

## 6. Decisions only the author can make
1. Accept the composite parent (M2) as an effective theory with a cutoff above the strong-coupling scale, keeping the protected source?
2. Give up the protected source and couple matter to a single leaf (M1), accepting the tensor-Yukawa consequence?
3. Keep DYN v8 as the restricted reference model and record this as a model-specific obstruction (B5 action 5)?
4. Extend the test to the N-site chain, or test the HKS variables before deciding?

## 7. Not done in this package
- Framework v21 consistency check.
- SS-MAT v1 not read; its matter assumptions may differ from the scalar used here.
- Independent re-derivation of secondary/tertiary closure for M1.
- General-N composite; HKS-variable rescue.
- No publication or review.

## 8. Files
- Scripts and outputs (not included in this release):
  - `c1_composite_planar.py` (not included) / `c1_out.txt` (not included): symmetric-vielbein condition; composite lapse-linearity at fixed boost.
  - `c2_boost_equation.py` (not included) / `c2_out.txt` (not included): boost-equation factorization test.
  - `c3_reduced_and_linear.py` (not included) / `c3_out.txt` (not included): reduced lapse Hessian after boost elimination; printed shared scalar rank; protected-source condition; single-leaf strengths.
  - `c4_weight_scan.py` (not included) / `c4_out.txt` (not included): composite failure versus leaf weights. Needs `c2_boost_equation.py` (not included) in the same folder.
- Requirements: Python 3, sympy, mpmath, numpy.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN", "DYN v8" in this note): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-FRAMEWORK v21**: D. G. Palmer (2026). *The Scale Space–CNRS Programme: A Theoretical Framework* (version 21). Zenodo. [doi:10.5281/zenodo.23840776](https://doi.org/10.5281/zenodo.23840776). Published; current version.
- **SS-MAT v1** (written "MAT" in this note): D. G. Palmer (2026). *SS-MAT: Scale-Extended Matter Sources: Protected Matching, Scale Transport and Completion Gates* (version 1). Zenodo. [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555). Published; current version.

Material named in this note but not included in this release: `SS-DYN_leafwise_dynamical_closure_v8.tex`, `SS_P1_scale_velocity_route_closed_20261106.md`, `SS_PhaseB5_parent_answer_20261105.md`, `SS_WS1_closure_recommendations_2026-10-24_v1.md`, `c1_composite_planar.py`, `c1_out.txt`, `c2_boost_equation.py`, `c2_out.txt`, `c3_out.txt`, `c3_reduced_and_linear.py`, `c4_out.txt`, `c4_weight_scan.py`.
