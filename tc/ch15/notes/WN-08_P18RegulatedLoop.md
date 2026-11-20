> **Public edition of evidence note WN-08.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P18RegulatedLoop.md`, a working note dated 9 November 2026. Not peer reviewed.
> - **Source content hash:** `cfc4056ffd5aa4dc2d6277354c091d6c167959e91838ba89289ea976aa40b0d7` (5218 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# P18 — Regulated one-loop test of the per-leaf parent, and corrections to P15 and P17

**9 November 2026 · noncanonical working note · WS1 MAT-DYN**
AI assistance: an unreviewed calculation by a Claude session working for the author, made in response to an AI-session review of P15–P17 (9 Nov 2026). Not an independent review. No canonical file changed.

## Verdict

The review's main point is right. P15 and P17 counted every matter copy fully in the loop, including copies far above the cutoff. With the real regulated tadpole, heavy copies decouple and the per-leaf parent is radiatively stable as long as the cutoff stays within a few copy masses: the light mode leaks 10% into the copies at Λ ≈ 7 m₁ for λ₀ = 1, between about 3 m₁ (λ₀ ≈ 16) and 15 m₁ (λ₀ = 0.1). Below the copy gap the leakage falls as Λ⁴. The result does not depend on leaf spacing, and barely on box size (6.3–7.1 m₁).

So P2's parent is not ruled out at one loop. The correct statement is an EFT condition: the matter copies must lie within roughly an order of magnitude of the matter cutoff; above that, each leaf needs its own counterterm, tuned by about (Λ/m₁)².

## Calculation (c26)

Leaves on |y| ≤ Y_c with weights w_n = F_nΔy, F = sech⁴y; action Σ_n w_n[½(∂φ_n)² + ½m²φ_n² + λ₀φ_n⁴/4!] + hopping (μ = 1, Neumann ends). Modes are w-orthonormal with masses M_k² = m² + h_k, copy gap m₁² = h₁, light mass m² = 0.01 m₁².

One loop, Euclidean sharp cutoff: ⟨φ_n²⟩ = Σ_k u_k(n)² I(M_k), with I(M) = [Λ² − M² ln(1 + Λ²/M²)]/16π². The generated term is ½ w_n(λ₀/2)⟨φ_n²⟩φ_n²; it is protected iff ⟨φ_n²⟩ is the same on every leaf. Leakage ε is the heavy-copy norm of the lowest mode after adding it (exact diagonalisation).

| Y_c | Δy | ε at Λ = 1.58 m₁ | ε at 3.16 m₁ | ε at 6.31 m₁ | ε = 0.1 at |
|---|---|---|---|---|---|
| 1.5 | 0.05 / 0.025 / 0.0125 | 1.6e-3 | 1.4e-2 | 9.3–9.5e-2 | 7.08 m₁ |
| 4.0 | 0.05 / 0.025 / 0.0125 | 1.8e-3 | 1.6e-2 | 0.11 | 6.31 m₁ |

Small-Λ slope d ln ε/d ln Λ = 3.98 (heavy-threshold decoupling, Λ⁴). Control: with the zero mode alone the spread of ⟨φ_n²⟩ across leaves is 5.5e-13, confirming the review's point that the light mode by itself is exactly protected.

Coupling dependence (Y_c = 1.5, Δy = 0.025): ε = 0.1 at Λ = 14.96, 10.00, 6.68, 4.22, 2.66 m₁ for λ₀ = 0.1, 0.3, 1, 4, 15.8. The dependence is weaker than λ₀^(−1/2) because of the logarithms.

## Corrections to P15 and P17

| Earlier claim | Status now |
|---|---|
| P15: per-leaf parent "fails as a natural theory"; leaf weights off by up to 1e13 | Withdrawn. That came from the all-copies-equal sum. Replaced by the EFT condition above. |
| P17: Λ ≲ 1.3 m₁/√λ₀, falling as √Δy | Withdrawn. The √Δy fall was an artefact of counting all copies; with regulation the bound converges in Δy. |
| P17: copies must sit at the cutoff | Softened: the cutoff may be at most about 3–15 times the copy gap m₁ (λ₀ from 16 to 0.1, 10% tolerance). |
| P15/c23 tree rule (gravity links plus hopping must form a tree) | Supported by one three-leaf chain and one loop in minisuperspace only; a conjecture for general graphs and inhomogeneous gravity. |
| P15/c24 tree-level truncation "to all orders" | Holds for static, equal leaf geometries with fixed weights; not shown for dynamical, unequal leaf metrics. |
| P15/c24 Y = 8 rows | Numerically unstable (already flagged in c24); the review's rerun confirms. Use Y = 4 and 6 only. |
| P17 §4 regulator lemma | Valid for a minimally coupled scalar in a local per-leaf loop approximation; not a general no-go for nonminimal couplings, extra symmetries or other matter. |
| c25b normalisation δ = λ₀Λ²/16π² | Convention was undefined. With V = λ₀φ⁴/4! the generated mass shift is (λ₀/2)I → λ₀Λ²/32π² at large Λ, as the review says; c26 uses this. |

What survives from P15 and P17: the classical minisuperspace counts and betas, the tree-level truncation identity, the box-size table and the observation that each leaf's counterterm is local. P16 is unaffected.

## Consequence for WS1

The per-leaf parent remains a viable effective theory, with a testable structural condition: its matter copies cannot sit far below the matter cutoff without per-leaf tuning. If the copies are light enough to matter at accessible energies, the matter cutoff must be low too. This is weaker than the earlier "reduces to SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)" claim. SS-DYN's restricted common-metric theory remains the established result, but the parent is not excluded.

## Limits

Static φ⁴ scalar on a one-dimensional chain, sharp four-momentum cutoff, one loop, quadratic term only, 10% leakage tolerance chosen by hand. Other regulators shift the numbers by O(1). Fermions, gauge fields, heavy-mode matching at two loops and the inhomogeneous constraint chain are untested.

## Files

`c26_regulated_tadpole.py` and its output `c26_out.txt` (not included in this release).

## Status

Noncanonical. P15 and P17 are left unchanged; this note supersedes the claims listed above.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.

Other working notes referred to by label:

- P2: [WN-04](WN-04_P2Parent.md)
- P15: [WN-05](WN-05_P15ParentClosure.md)
- P16: not included in this release (a review note).
- P17: not included in this release.
