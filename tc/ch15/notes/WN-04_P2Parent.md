> **Public edition of evidence note WN-04.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P2Parent.md`, a working note dated 7 November 2026. Not peer reviewed.
> - **Source content hash:** `dd41f74fb393e388fe398372f92a19f1167b1bf1b694714b94ce0f085b27965e` (6141 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** Its §2 statement about the clock geometry paper is corrected in [WN-14](WN-14_P3ScaleSpectra.md) §8. An editorial note marks the affected passage; the original wording is kept.

# SS WS1 P2: search for a ghost-free Scale Space parent (first pass)

Date: 7 November 2026. Status: **draft for the author's review. Not independently reviewed.**
Done on the author's instruction "Please start the search" (7 Nov 2026), after asking "Can we find a parent?". Follows [WN-01](WN-01_P1Gate.md), [WN-02](WN-02_P1Gate_b.md), [WN-03](WN-03_P1Gate_c.md) (WS1 MAT-DYN).
Labels as in [WN-01](WN-01_P1Gate.md): [Derived], [Computed], [Literature], [Assumed], [Conjecture]; [Read] = stated in the named document.

## 1. Short answer
A candidate parent passes the first two tests. Gravity is DYN's independent-leaf parent (one metric per leaf, minimal square-root links). Matter is given **its own copy on every leaf**, coupled only to that leaf's metric, with each leaf's matter action weighted by the same F_n = sech⁴ as gravity, and neighbouring copies linked by a "hopping" potential.
- It is ghost-free in the variable-independent test on the 3-site chain [Computed C7].
- Its lightest matter mode gives exactly the protected source at linear order, for any hopping strength [Computed C8].
- In the strong-hopping limit it reduces to DYN v8's printed shared-matter coupling [Computed C8(5)]. So the printed coupling looks like the low-energy limit of this parent, valid below the hopping scale, rather than a fundamental coupling [Conjecture].
This is not yet a full theory: see §5.

## 2. What the corpus already has
> **Editorial note (public edition, 19 November 2026):** A later working note states that the description of SS-L5D below ("the extra coordinate is clock time, not scale") is wrong: in SS-L5D, scale u is the fourth dimension, forming the 4D configuration space with the three space directions, and clock time t is the fifth. See [WN-14](WN-14_P3ScaleSpectra.md) §8. The text below is unchanged from the working note.

- **SS-L5D v1 [doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609)** [Read]: a 5D *clock* geometry, g = −c²N²dt² + e^{2u}dx² + a²du²; the extra coordinate is clock time, not scale. No 5D action, no leaves, no kink; "no reduction or dynamical equivalence is asserted" with SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) (§1.1). It does not contain a parent.
- **SS-DYN v8** [Read]: the parent action itself is not printed (it is in SS-DYN v6 [doi:10.5281/zenodo.23604782](https://doi.org/10.5281/zenodo.23604782), not read here). The parent warp appears as a comparison geometry, ds₅² = e^{2𝒜}g dz dz + dλ² with e^{𝒜} = sech²; F₀ = e^{2𝒜} = sech⁴ and M₄² = M₅³∫F₀. Ordinary matter has no gradient along the scale direction; the parent uses "the same matter scalar" on every leaf, c_n = w_n F₀ₙ a_n³ (the coupling that fails, P1Gate M0).

## 3. Ghost test (C7)
Same machinery as C6: 3-site chain, square-root links 1–2 and 2–3, six multipliers (N₁, N₂, N₃, s₁, s₂, s₃); ghost-free requires on-shell Hessian rank 2. Matter: one scalar per leaf with generic (P_n, φ′_n, V_n), plus hopping μ·W·(φ_n − φ_{n+1})².

| Matter | Rank | Verdict |
|---|---|---|
| Per-leaf scalars, no hopping | 2 | ghost-free |
| + hopping, split leaf measure (det e_n + det e_{n+1})/2 | 2 | ghost-free |
| + hopping, link measure det(e_n + e_{n+1})/16 | 2 | ghost-free |
| Control: hopping between leaves 1 and 3 (not gravitationally linked), det(e₁ + e₃) | 4 | BD ghost |

Reading [Derived]: field values φ_n are phase-space variables, not multipliers, so a hopping potential with a single-leaf measure, or with a measure of the same type as a gravitational link, keeps the lapses linear. Hopping must run only along gravitational links; the control shows why.

## 4. Protection (C8, linear, 3-site chain)
Lightest matter mode χ, its energy on each leaf, and its linear coupling to the two massive graviton modes ("leakage"; Yukawa strength α with the 4/3 tensor factor; a central-leaf-only source gives α = 0.47 as in P1Gate_c).

| Matter weighting | Lightest mode | Leakage to massive modes | α |
|---|---|---|---|
| (1) Whole leaf matter action weighted by F_n (kinetic and mass) | exactly flat, all μ | 10⁻¹⁶ | ~10⁻³¹ (zero) |
| (2) Unweighted leaf matter | flat | 0.92 | 1.14 |
| (3) 5D bulk scalar in the sech² warp: kinetic weight e^{2𝒜} = F, mass weight e^{4𝒜} = F² | nearly flat at large μ | 0.23 | 0.07 |
| (4) Massless 5D bulk scalar (kinetic weight F only) | exactly flat | 10⁻¹⁶ | zero |

Reading:
- With F-weighted leaf actions the mass and kinetic matrices are proportional, so the flat profile is an exact eigenvector and its source is ∝ F = M_n², which is the protected condition of P1Gate §3.2 [Derived; Computed].
- A plain 5D bulk scalar gives F for free only for the kinetic term; a mass term picks up sech⁸ and leaks (α ≈ 0.07 here). So the F-weighting of the *whole* leaf action is an assumption of the discrete parent, natural there but not supplied by a simple 5D bulk action [Derived].
- As μ → ∞ the copies lock together and the theory becomes one field on all leaves with weights F_n, the printed coupling of DYN v8 [Computed C8(5)]. The rank N−1 obstruction is then read as the trace of the heavy matter copies that were integrated out [Conjecture].

## 5. Costs and open points
- **Matter copies:** every matter field gets a copy per leaf. Besides ordinary matter (the flat mode) there are heavier matter modes, with masses set by the hopping strength; these do couple to the massive gravitons. Their scale and phenomenology are open.
- **Linear only:** the flat mode is exact at linear order. When the leaf metrics differ nonlinearly it mixes with the heavy copies. This matches DYN v8's own statement that protection holds for the linear source.
- **Scalars only:** fermions and gauge fields not tested. Under a 5D reading a gauge field's kinetic weight is uniform, not F, so it would not be protected without the same leaf weighting [Derived; untested].
- **Constraint closure:** the rank test checks the multiplier structure at sample points (planar, N = 3). Secondary and tertiary constraint closure for this matter sector is not shown.
- **Not read:** SS-DYN v6 (where the parent action is printed); w_n and a_n³ may change the weighting.

## 6. Files
- Scripts and outputs (not included in this release):
  - `c7_hopping_chain.py` (not included) / `c7_out.txt` (not included): ghost test with linked per-leaf matter (self-contained; gravity sector copied from c6).
  - `c8_protection_linear.py` (not included) / `c8_out.txt` (not included): linear protection of the lightest matter mode.
- Requirements: Python 3, mpmath, numpy.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v6**: D. G. Palmer (2026). *SS-DYN: A Scale-Localized Leafwise Dynamical Closure for Scale Space: Protected Tensor Gravity, a Repaired Scalar Continuum, and Constrained Collective Matter* (version 6). Zenodo. [doi:10.5281/zenodo.23604782](https://doi.org/10.5281/zenodo.23604782). Published; superseded by version 8 ([doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)).
- **SS-DYN v8** (written "DYN", "DYN v8" in this note): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-L5D v1**: D. G. Palmer (2026). *SS-L5D: Clock Geometry and Consistent Five-Dimensional Extensions of Scale Space* (version 1). Zenodo. [doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609). Published; current version.

Material named in this note but not included in this release: `c7_hopping_chain.py`, `c7_out.txt`, `c8_out.txt`, `c8_protection_linear.py`.
