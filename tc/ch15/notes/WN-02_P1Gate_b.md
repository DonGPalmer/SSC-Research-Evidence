> **Public edition of evidence note WN-02.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P1Gate_b.md`, a working note dated 7 November 2026. Not peer reviewed.
> - **Source content hash:** `b64400fbb17bc50703ba58073d132134e923e7359c5ba5306bde70843c3e5e3a` (6805 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# SS WS1 P1b: composite coupling in the HKS variables, and the 3-site chain

Date: 7 November 2026. Status: **draft for the author's review. Not independently reviewed.**
Follows [WN-01](WN-01_P1Gate.md) (WS1 MAT-DYN, 7 Nov 2026). Done on the author's choice of option 4, "test more first" (7 Nov 2026).
Labels as in [WN-01](WN-01_P1Gate.md): [Derived], [Computed], [Literature], [Assumed], [Conjecture].

## 1. Questions
1. Can the composite coupling (M2) be rescued by the variables of Hassan, Kocic, Schmidt-May (HKS), arXiv:1409.1909? P1Gate §3.2 left this open.
2. Do the two-leaf results carry over to the 3-site chain?

## 2. What HKS argue
From the paper (read in full, v1 only on arXiv) **[Literature]**:
- They trade the shift difference for a Lorentz boost velocity v_a, with ν^i = λ^i + (L (φ̃⁻¹)^i_a + N (e⁻¹)^i_a) v^a (their eq. 3.11), and show the action is linear in the lapses N, L at fixed v_a.
- For matter on the effective metric, §4.3 argues the v_a equations are lapse-independent because "the Jacobian factor δν/δv is already linear in the lapses", so δS/δν "cannot depend on L and N".

Assessment **[Derived]**:
- In the planar two-leaf case their v is exactly the boost variable used in P1Gate (C1: s1 = s2 + (N1/A1 + N2/A2) v). So P1Gate's C2 and C3 tests are already tests in the HKS variables.
- Their step does not follow. With S = N1 C1(v) + N2 C2(v) + …, one has δS/δν = (N1 C1' + N2 C2')/(N1/A1 + N2/A2). That is a ratio of two lapse-linear expressions; it is lapse-independent only if A1·C1′ = A2·C2′, which is exactly the factorization tested in C2. Linearity of both factors does not force it.
- C2 shows that with composite matter the ratio does depend on the lapse ratio, so in their own variables the v equation brings lapse dependence back **[Computed C2, C3]**.

## 3. Variable-independent test (C5)
To settle whether *any* choice of variables could rescue the coupling, C5 uses a test that does not depend on the variables **[Derived]**:
- Metric formulation; non-dynamical variables (N1, N2, s1, s2); the boost is fixed by the symmetric-vielbein condition.
- H is homogeneous of degree 1 in them, so its Hessian always has one null direction.
- Ghost-free counting needs 3 of the 4 to enter linearly (overall lapse, overall shift, one BD-killing constraint), i.e. Hessian rank 1.
- The R-terms are linear, so every sample point can be placed on the constraint surface. There, under any invertible change of lapse/shift variables the Hessian transforms as Jᵀ·Hess·J, so its rank is the same in HR, HKS or any other variables.

Results **[Computed C5, C5b]** (60-digit numerics; null eigenvalues ~10⁻⁶², non-null 10⁻²–1):

| Case | Rank | Verdict |
|---|---|---|
| Gravity only (vielbein potential, all 5 β terms) | 1 | ghost-free, as expected |
| Matter on leaf 1, or on leaf 2 | 1 | ghost-free |
| Composite, generic matter (P, φ′, V) | 2 | BD ghost |
| Composite, potential only (P = φ′ = 0) | 1 | ghost-free |
| Composite, P = 0 or φ′ = 0, leaves relatively boosted | 2 | BD ghost (small eigenvalue ~10⁻⁸–10⁻⁶) |
| Composite, no relative boost, P = 0 or φ′ = 0 | 1 | ghost-free |
| Composite, no relative boost, P and φ′ both non-zero | 2 | BD ghost |

Reading:
- The composite coupling loses the BD-killing constraint whenever matter carries momentum (P·φ′ ≠ 0), or whenever the leaves are relatively boosted and matter has kinetic or gradient terms.
- Static, homogeneous configurations pass. That is why homogeneous (FRW-type) checks look fine.
- Because the rank does not depend on the variables, **no change of variables (HKS or other) rescues the composite coupling as a full theory** in this test **[Computed, planar N = 2]**. This agrees with de Rham, Heisenberg, Ribeiro, arXiv:1409.3834 **[Literature]**.
- Planar caveat **[Derived, Assumed]**: with reflection symmetry in y and z, the full lapse/shift Hessian is block-diagonal (x-block above, plus y- and z-shift blocks). If the y- and z-blocks keep the rank 1 they have in pure bimetric theory, the full rank is ≥ 4 against the required 3, so the ghost is not an artefact of the planar truncation.

## 4. 3-site chain (C6)
Leaves 1–2–3, square-root links on 1–2 and 2–3 only; leaf 2 as reference frame. Six non-dynamical variables; ghost-free counting needs Hessian rank 2 (three lapses plus the overall shift linear) **[Derived]**.

Results **[Computed C6]**:

| Case | Rank | Verdict |
|---|---|---|
| Gravity only (chain) | 2 | ghost-free |
| Matter on the central leaf only | 2 | ghost-free |
| Composite with protected weights b ∝ sech⁴ = (0.176, 1, 0.176) | 4 | both BD-killing constraints lost |
| Same composite, potential only (P = φ′ = 0) | 4 | still fails |

Reading:
- The chain makes the composite worse, not better. In the chain, leaves 1 and 3 are not linked, so their relative vielbein is not symmetric (residual 0.15 at the sample point). Then even det(e_eff), i.e. a pure vacuum-energy term, is nonlinear in the lapses.
- Single-leaf coupling stays ghost-free in the chain, with the short-range force found in P1Gate §3.3 (strength ratio 1.35 for the central leaf).

## 5. What this means for the four options
- **Option 1 (composite with a cutoff):** not rescued by HKS variables or by going to the chain. In the chain it fails even for vacuum energy, so any effective-theory reading would need its own cutoff analysis, not covered here **[Conjecture that the cutoff is lower in the chain]**.
- **Option 2 (single leaf):** the only coupling that stays ghost-free in every case tested (two leaves and the 3-site chain). It still costs the protected weights.
- **Option 3 (record the obstruction):** strengthened. The obstruction now holds in a variable-independent form and for the chain.
- So the test points to option 2 if a full parent is wanted, or option 3 if the protected weights are kept and the parent is left open.

## 6. Not done
- Framework v21 [doi:10.5281/zenodo.23840776](https://doi.org/10.5281/zenodo.23840776) check; SS-MAT v1 [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555) not read (as in P1Gate).
- y- and z-shift blocks not computed (planar code only).
- Chains longer than 3 sites; non-minimal or extra links (e.g. closing the chain with a 1–3 link).
- Independent review.

## 7. Files
- Scripts and outputs (not included in this release):
  - `c5_invariant_rank.py` (not included) / `c5_out.txt` (not included): variable-independent Hessian rank, two leaves.
  - `c5b_homogeneous.py` (not included) / `c5b_out.txt` (not included): zero-relative-boost edge cases. Needs `c5_invariant_rank.py` (not included) in the same folder.
  - `c6_chain3.py` (not included) / `c6_out.txt` (not included): 3-site chain.
- Requirements: Python 3, mpmath.

---

## References and related notes (public edition)

Published works cited:

- **SS-FRAMEWORK v21**: D. G. Palmer (2026). *The Scale Space–CNRS Programme: A Theoretical Framework* (version 21). Zenodo. [doi:10.5281/zenodo.23840776](https://doi.org/10.5281/zenodo.23840776). Published; current version.
- **SS-MAT v1**: D. G. Palmer (2026). *SS-MAT: Scale-Extended Matter Sources: Protected Matching, Scale Transport and Completion Gates* (version 1). Zenodo. [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555). Published; current version.

Material named in this note but not included in this release: `c5_invariant_rank.py`, `c5_out.txt`, `c5b_homogeneous.py`, `c5b_out.txt`, `c6_chain3.py`, `c6_out.txt`.
