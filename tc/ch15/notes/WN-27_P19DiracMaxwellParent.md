> **Public edition of evidence note WN-27.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P19DiracMaxwellParent.md`, a working note dated 9 November 2026. Not peer reviewed.
> - **Source content hash:** `7536b48f3635d81d314ffca38672a6a68a2888d9883dbfb8861a2eb3d0050cfb` (8139 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** Its Y_c = 4 scans are judged unreliable in [WN-28](WN-28_P20ChiralParent.md). An editorial note marks the affected passage; the original wording is kept.

# SS WS1 P19: per-leaf Dirac + Maxwell parent candidate

Date: 9 November 2026. Status: **working note, unreviewed AI calculation, noncanonical.** Written on the author's instruction "yes to building the fermion and Maxwell candidate" (9 Nov 01:22Z). Follows P2, P15, P17, P18 (WS1) and answers the Dirac–Maxwell gate in [WN-09](WN-09_SS_ParentMatter_DiracMatching_v1.md). Labels: [Derived], [Computed], [Assumed], [Open].

## 1. Short answer
- **Tree level [Computed c27]:** the light electron-like fermion and the photon are exactly the flat modes, for any hopping strengths and any leaf weights. The light photon couples to every light species with the same charge e_eff = e/√W (W = Σ w_n). Light currents do not source heavy photons. This is protected to all orders by the unbroken diagonal U(1) [Derived].
- **Nonlinear relative metrics [Computed c27 T3]:** if leaf conformal factors differ by δ (DiracMatching's case), light masses shift as ln m_phys/m = c(m) δ². The species-independent part reproduces DiracMatching's locked C4/C3 (two-leaf check exact). The species-dependent part is small: c(m) ≈ c_lock − 0.35 (m/m₁) for m ≪ m₁.
- **One loop [Computed c28]:** the light fermion leaks into heavy copies. Leakage ε ∝ Λ⁴ below the copy gap and reaches 10% at Λ ≈ 4 m₁ (photon gap μ₁ = 0.3 m₁), 13–16 m₁ (μ₁ = m₁) or 40–50 m₁ (μ₁ = 3 m₁). This is the same kind of EFT window as the scalar case in P18.
- **Verdict:** the per-leaf Dirac + Maxwell parent is a viable restricted EFT candidate below a cutoff of a few to ~50 fermion copy gaps, with exact charge universality. It is not a derivation of the Standard Model coupling (chirality, Higgs mass, non-abelian groups and gravity loops are untested).

## 2. Model [Assumed]
Leaves n on |y| ≤ Y_c, w_n = F_n Δy, F = sech⁴ y (as P2/P18). On each leaf: a Dirac copy ψ_n with charge 1 under its own U(1)_n and a photon A_n. Neighbouring leaves are joined by a link field U_e = exp(iπ_e/f) of charge (+1, −1) (dimensional deconstruction):

L = Σ_n w_n [ −F_n²/(4e²) + ψ̄_n(iγ·D_n − m)ψ_n ] + Σ_e (f²/2)|D U_e|² − κ Σ_e (ψ̄_n − ψ̄_{n+1}U_e†)(ψ_n − U_e ψ_{n+1}).

Hopping runs only along gravitational links (P2's ghost rule). With L = BᵀB/Δy and L u_k = h_k W u_k (u_k W-orthonormal, h_0 = 0):
- Fermion copies: M_k = m + κ h_k, gap m₁ = κ h_1.
- Photon copies: μ_k = e f √h_k, gap μ₁. Write r = μ₁/m₁.
- Both sectors share the eigenvectors u_k, because both hop with the same L.

Units throughout: m₁ = 1. Coupling e² = 4π/137.

## 3. Tree level (c27)
**T1, flat modes [Computed].** For three choices of (m, κ, f) on Y_c = 1.5 and 4: the lowest fermion mode is flat with mass exactly m, and the photon zero mode is flat. Deviation ≤ 1e-11.

**T2, charge universality [Computed; Derived to all orders].**
- The light-photon coupling equals e/√W to all digits.
- Heavy photon to light current: ≤ 7e-14. Light–heavy fermion–light photon vertex: ≤ 7e-14.
- To all orders: the diagonal U(1) is unbroken and its gauge field is the null vector of the link mass matrix. So the massless photon stays flat whatever the loop corrections to the kinetic matrix, and it couples to the total charge Σ J_n.
- Charge universality across species therefore holds exactly. It does not depend on the leaf weights.

**T3, relative conformal factors [Computed].** Leaf metrics A_n² g_E with A_n = exp(δ s_n), where s is the lowest copy profile (orthogonal to flat).
- Weights: Dirac kinetic w A³, Dirac mass w A⁴ m, Maxwell w (conformal). Hopping link weight A^p, p = 0 or 4.
- Results (Y_c = 1.5, Δy = 0.025):

| m/m₁ | 0.001 | 0.01 | 0.1 | 1 |
|---|---|---|---|---|
| c(m) | 1.3012 | 1.2981 | 1.2646 | 0.930 |

- Locked limit: c_lock = 1.3018. Y_c = 4 gives c_lock = 1.235 with the same slope. p barely matters (≤ 2e-4).
- Two-leaf check against DiracMatching (w = 1, A = 1 ± 0.1, strong hopping): m_phys/m = 1.029223 = (1+6δ²+δ⁴)/(1+3δ²).

Reading [Derived]:
- Light matter does not source δ at linear order (P2 protection). So δ appears only at second order in the source, and the leading non-universal effect is the species-dependent part of c, about −0.35 (m/m₁) δ².
- The universal part c_lock δ² is a common mass rescaling and does not violate the equivalence principle.
- DiracMatching's "exact common metric iff identical A" stands. In this parent, unequal A are heavy fields that light matter does not source linearly.

## 4. One loop (c28)
Setup:
- Feynman–'t Hooft gauge: heavy photons a_j and eaten link Goldstones G_j, both of mass μ_j. Sharp Euclidean cutoff Λ on the loop momentum. Self-energy at p → 0 (m ≪ m₁).
- The light-fermion–copy-j–Goldstone-j coupling is (M_j − m)e/(μ_j√W) (equivalence theorem).
- Leakage into copy k is ε_k = (b_{k0} − m a_{k0})/(m − M_k), where a and b are the kinetic and mass parts of the self-energy.
- Checks: loop integrals against mpmath (1e-9); QED limit δm → (3α/4π)M ln Λ²; uniform-weight ring control ε = 5e-15.

> **Editorial note (public edition, 19 November 2026):** A later note found that this note's Y_c = 4 scans were not checked for link strong coupling, and says this note should be read through its Y_c = 1.5 results; the ranges in the table below include Y_c = 4. See [WN-28](WN-28_P20ChiralParent.md) §5. The text below is unchanged from the working note.

Results (light mass m = 0.01 m₁):

| μ₁/m₁ | ε at Λ = 1 | 3.16 | 10 | ε = 1% at | ε = 10% at |
|---|---|---|---|---|---|
| 0.3 | 4–8e-4 | 6–8e-2 | 2–3.5 | 2–2.5 m₁ | 4 m₁ |
| 1 | 1.5e-4 | 6–8e-4 | 4–6e-2 | 6–8 m₁ | 13–16 m₁ |
| 3 | 2e-5 | 4e-4 | 3e-3 | 25–32 m₁ | 40–50 m₁ |

- Ranges cover Y_c = 1.5 and 4 and Δy = 0.1 and 0.05. Thresholds agree across Y_c and Δy within one step of the Λ grid (10 points per decade). The tail above about 30 m₁ is not converged, but that is outside the window anyway.
- Small-Λ slope: 3.5–3.95, i.e. heavy copies decouple as Λ⁴.
- Split by loop (Λ = 10 m₁, Y_c = 1.5): photon loop alone gives ε = 0.4–1.3%. The Goldstone loop dominates when μ₁ < m₁ (2.4 at r = 0.3).
- Reason: with mass-type hopping the fermion copy masses grow like h_k, faster than photon masses (√h_k), so the equivalence-theorem coupling grows up the tower.
- ε is nearly independent of the light mass (4.10e-2 at m/m₁ = 0.001–0.1). So leakage-induced couplings to heavy modes are universal across species that share κ and charge.

## 5. Corrections and limits
- **Chirality [Open, main gap].** The copies are vector-like Dirac fermions with a bare mass and Wilson-type mass hopping. Standard Model fermions are chiral, with Higgs masses. A first-derivative (chiral) hopping would give M_k ∝ μ_k and a slower-growing Goldstone coupling; it is untested.
- **Regulator [Open].** A sharp cutoff is not gauge invariant. A Pauli–Villars or dimensional-regularization rerun is needed before quoting thresholds to better than a factor of ~2.
- **Not computed:** graviton loops; fermion loops feeding the gravity sector (per-leaf vacuum energy, P14 common mode); radial link modes; non-abelian groups.
- **Species with different hopping κ** would leak differently. Universality of heavy-mode couplings then fails at order ε.
- The whole-leaf F-weighting is P2's assumption, not derived from a 5D action.

## 6. For the matching test (fields of a coordination note, not included)
- **Action:** §2. Conventions: Euclidean loops, mostly-plus Minkowski elsewhere; leaf metrics A_n² g_E; leaf weights w_n = sech⁴ y_n Δy; per-leaf e² = 4π/137 in the scans (illustrative: the measured α fixes e_eff = e/√W).
- **Retained:** one flat Dirac fermion per species (mass m) and the flat massless photon.
- **Eliminated:** heavy fermion copies M_k = m + m₁ h_k/h_1; heavy photons and Goldstones μ_k = r m₁ √(h_k/h_1); radial link modes (assumed heavy).
- **Regulator and matching scale:** sharp 4-momentum cutoff Λ; matching at p ≪ m₁.
- **Validity:** E ≪ min(m₁, μ₁); Λ ≲ 4 m₁ (r = 0.3), 13 m₁ (r = 1), 40 m₁ (r = 3) for ε ≤ 10%.
- **Open assumptions:** §5.

## 7. Files
Scripts and outputs (not included in this release): `c27_dirac_maxwell_tree.py`, `c27_out.txt`, `c28_dirac_maxwell_one_loop.py`, `c28_out.txt`.

Requirements: Python 3, numpy, mpmath.

---

## References and related notes (public edition)

Other working notes referred to by label:

- P2: [WN-04](WN-04_P2Parent.md)
- P14: not included in this release.
- P15: [WN-05](WN-05_P15ParentClosure.md)
- P17: not included in this release.
- P18: [WN-08](WN-08_P18RegulatedLoop.md)

Material named in this note but not included in this release: `c27_dirac_maxwell_tree.py`, `c27_out.txt`, `c28_dirac_maxwell_one_loop.py`, `c28_out.txt`.
