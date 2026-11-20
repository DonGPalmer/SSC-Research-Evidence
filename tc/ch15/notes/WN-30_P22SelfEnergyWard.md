> **Public edition of evidence note WN-30.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P22SelfEnergyWard.md`, a working note dated 9 November 2026. Not peer reviewed.
> - **Source content hash:** `93f44d10b67b54696465ef20af3360a906c41fde959323697d9d40f6ae004fd1` (6355 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# SS WS1 P22: gauge-invariant self-energy, Ward identity and wavefunction leakage of the chiral light mode

Date: 9 November 2026. Status: **working note, unreviewed AI calculation, noncanonical.** Written on the author's "Yes" (9 Nov 14:36Z) to running the first next gate of P20b §4. Follows P20 and P20b (WS1). Labels: [Derived], [Computed], [Open].

## 1. Outcome
**Gate 1 of P20b passes, with the window narrowed slightly.**
- The one-loop self-energy and vertex of the chiral light mode satisfy the Ward identity of the unbroken diagonal U(1) to 1e-14 (c34). This holds for photon exchange and Goldstone exchange separately, in a gauge-invariant regulator.
- Wavefunction and vertex corrections do move the light source into the heavy photon copies, as the review said. They add to the mass-matrix tilt with the same sign, adding about a third to a half on top of it at the link scales.
- Total leakage at the P20 link-fluctuation scales, core box Y_c = 1.5: **about 9–10% (r = 0.3), 6–7% (r = 1), 6.6% (r = 3)**. P20b quoted 5–7% from the tilt alone.
- So the protected-source condition survives at the 10% level in the weakly coupled core, but with little margin at r = 0.3.

## 2. Method [Derived]
- Regulator: dimensional regularization, MS-bar, Wilsonian truncation. Copies (fermion, photon, Goldstone) with mass below Λ are kept, and μ_R = Λ. This is gauge invariant within the truncated tower. A sharp momentum cutoff is not, so it cannot be used for a Ward check.
- Gauge: Feynman–'t Hooft. The abelian link kinetic term is quadratic in π, so there is no photon–Goldstone–Goldstone vertex. The hopping term contains no gauge field, so there is no contact vertex.
- One-loop diagrams for the right-handed light mode:
  - photon-copy exchange (internal R–R kinetic, and R→L→R through two mass insertions);
  - eaten-Goldstone exchange (Yukawa coupling κω_e/2f_e to L̄_e(R_n + R_{n+1}); internal L–L kinetic, and L→R→L).
- The vertex for an external photon copy j at zero momentum transfer inserts the charge matrix of mode j on the internal fermion line: C^R_abj = Σ_n w_n ρ_a ρ_b u_j on R components, C^L_abj = Σ_e wL_e l_a l_b (u_j(n) + u_j(n+1))/2 on L components.
- Leakage measure: η_j = (one-loop vertex of the light mode to copy j) / (tree coupling to the flat mode). A tilt h of the zero mode gives η_j = 2⟨h, u_j⟩, so ε = |η_{j≥1}|/2 is the same measure as ε_χ in P20.
- The tilt was recomputed in the same scheme (c35), replacing c30's sharp-cutoff loop integrals by their MS-bar forms.

## 3. Ward identity (c34) [Computed]
Diagonal U(1) (j = 0): the vertex Λ₀ computed from the triangle diagrams equals the p-slash coefficient Z of the self-energy computed directly, which is a separate formula.

| r | Λ | Z (photon) | Λ₀ (photon) | Z (Goldstone) | Λ₀ (Goldstone) |
|---|---|---|---|---|---|
| 0.3 | 10 | −1.48824e-2 | −1.48824e-2 | −1.38937e-1 | −1.38937e-1 |
| 1 | 10 | −3.75321e-3 | −3.75321e-3 | −6.93970e-3 | −6.93970e-3 |
| 3 | 30 | −7.89818e-3 | −7.89818e-3 | −1.00135e-3 | −1.00135e-3 |

Relative agreement is 1e-14 to 1e-16 in the eight cases with massive copies inside Λ (Y_c = 1.5, Δy = 0.1). The ninth (r = 3, Λ = 3) keeps only the massless photon, so both sides are zero up to rounding (1e-32). Charge universality of the light mode (total charge 1) is therefore preserved at one loop, including wavefunction renormalization.

## 4. Leakage into heavy copies (c35) [Computed]
Core box Y_c = 1.5. ε_tilt: mass-matrix tilt; ε_Z: wavefunction plus vertex; ε_tot: both with signs. All MS-bar, truncated, μ_R = Λ. Δy = 0.1 (Δy = 0.05 in brackets).

| r | Λ (M₁) | ε_tilt | ε_Z | ε_tot |
|---|---|---|---|---|
| 0.3 | 3.0 | 4.1% (4.0%) | 2.0% (2.0%) | 6.1% (6.0%) |
| 0.3 | 4.47 (link scale) | 6.1% (5.9%) | 3.5% (3.1%) | **9.6% (9.0%)** |
| 0.3 | 10 | 11% (10%) | 10% (8.7%) | 21% (19%) |
| 1 | 10 | 3.3% (3.3%) | 0.7% (0.8%) | 4.0% (4.0%) |
| 1 | 15.85 (link scale) | 5.2% (4.7%) | 1.8% (1.4%) | **7.0% (6.1%)** |
| 1 | 30 | 7.4% | 3.5% | 10.8% |
| 3 | 30 | 3.7% | 0.75% | 4.5% |
| 3 | 44.67 (link scale) | 5.2% | 1.5% | **6.6%** |

- The two pieces have the same sign in every case (dominant copy j = 2: e.g. r = 1, Λ = 15.85: tilt +0.098, wavefunction + vertex +0.031). They add; they do not cancel.
- Odd-parity copies (j = 1, 3, …) get exactly zero leakage, as for the tilt.
- The wavefunction piece is largest at small r, where the Goldstone (longitudinal) coupling κ/μ is strongest. At r = 0.3 the Goldstone part of Z reaches −0.14 by Λ = 10, another sign of the link strong coupling found in P20 §4.
- Grid dependence: Δy = 0.1 and 0.05 agree to within about 10–25%; the finer grid gives slightly less leakage.
- In the MS-bar scheme the tilt at the link scales is about 5–6%, close to P20b's sharp-cutoff 5–7%.

## 5. What this does and does not settle
- **Settled:** the Ward identity of the light current holds at one loop in a gauge-invariant regulator; wavefunction corrections are included; the protected source stays within about 10% of flat at the P20 link scales in the core box.
- **Not settled [Open]:**
  1. The q → 0 vertex to an off-shell heavy copy is gauge dependent in general. A gauge-invariant low-energy amplitude needs box diagrams too. Gauge-parameter independence was not tested.
  2. The leakage grows with log Λ: the loops renormalize leaf-localized kinetic and charge terms that are not w-weighted. Above the window, flatness needs counterterms (fine-tuning of leaf-local operators). This is the same UV sensitivity seen in P15–P19.
  3. Non-abelian content with a Higgs Yukawa (P20b gate 2) is untouched, and so is the chiral redo of P21 (gate 3).
- Changes to earlier notes: P20b's "light matter within 5–7% of flat at the link scales" should read **6–10%** once wavefunction and vertex corrections are included. P20 and P20b are left unchanged; this note records the update.

## 6. Files
Scripts and outputs (not included in this release): `c34_selfenergy_ward.py`, `c34_out.txt` (Ward check); `c35_total_leakage.py`, `c35_out.txt` (leakage table; reads c34 and c30). Both scripts read `c30_chiral_zero_mode.py`.

Requirements: Python 3, numpy.

---

## References and related notes (public edition)

Other working notes referred to by label:

- P15: [WN-05](WN-05_P15ParentClosure.md)
- P19: [WN-27](WN-27_P19DiracMaxwellParent.md)
- P20: [WN-28](WN-28_P20ChiralParent.md)
- P20b: [WN-29](WN-29_P20bReviewCorrections.md)
- P21: [WN-25](WN-25_P21MatterIntoGravity.md)

Material named in this note but not included in this release: `c30_chiral_zero_mode.py`, `c34_out.txt`, `c34_selfenergy_ward.py`, `c35_out.txt`, `c35_total_leakage.py`.
