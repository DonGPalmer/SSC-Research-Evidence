> **Public edition of evidence note WN-25.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P21MatterIntoGravity.md`, a working note dated 9 November 2026. Not peer reviewed.
> - **Source content hash:** `79ccbee0fd59221b6c9baa58df8fddff7e3e9fbdfa0996719ec484aa210b38ef` (7016 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# SS WS1 P21: matter loops feeding the gravity sector of the per-leaf parent

Date: 9 November 2026. Status: **working note, unreviewed AI calculation, noncanonical.** Done on the author's "Yes" (9 Nov 02:03Z) to the question "Should I work out how matter loops feed the gravity weights next (vacuum energy per leaf and the P14 common mode)?". Follows P18–P20 (WS1). Labels: [Derived], [Computed], [Assumed], [Open].

## 1. Decision
**Matter loops do not threaten the parent's gravity weights. They do generate leaf-dependent ("relative") cosmological constants, and those decide between P5's two branches.**
- **TeV branch (P5: one common scale, κ ≈ 0.6–11 TeV): passes.** Relative cosmological constants shift the leaves' conformal factors by δ ≈ 1e-35 to 1e-28. Nothing needs tuning beyond the single ordinary cosmological constant every EFT has.
- **mm branch (graviton copies near 5 mm, matter copies ≳ 1 TeV): fails naturalness.** Integrating out even the first matter copy gives δ ≈ 0.02 per real degree of freedom at M₁ = 1 TeV, so O(1) for Standard Model field content. Above that it grows as Λ⁴: δ ≈ 0.8 per degree of freedom at Λ = 3 M₁. Each of the N − 1 relative cosmological constants would need its own tuning, or the mm branch has to drop the matter copies (the restricted common-metric theory, DYN v8).
- **Induced gravity weights:** the Einstein–Hilbert weight per leaf moves by δF/F ≈ 1e-29 (Λ = 10 M₁, M₁ = 20 TeV). The F-weighting of gravity is radiatively safe.

So the per-leaf parent selects the TeV branch. In that branch the matter-sector windows of P18–P20 (cutoff a few to tens of copy gaps, core box) are not shrunk by gravity-sector loops.

## 2. Setup [Assumed; P18 conventions]
- Matter: one real scalar copy per leaf on |y| ≤ Y_c, weights w_n = sech⁴(y_n)Δy for kinetic and mass terms, hopping along links. Two hopping choices: plain (as P18) and F-weighted (link weight as in P20).
- Leaf conformal factors σ_n: kinetic terms scale as e^{2σ_n}, mass and hopping as e^{4σ_n}, with hopping measure split half to each end leaf (P2 measure (a)).
- Leaf tadpole t_n = ∂Γ/∂σ_n (the trace of leaf n's vacuum energy). Protected means t_n ∝ w_n: then it is only the common cosmological constant. The relative part r_n = t_n/w_n − ⟨t/w⟩ is what sources relative leaf modes.
- Gravity: leaves with weight w_n and Fierz–Pauli links μ_e = sech⁴(y_e)/Δy (NS gate conventions, as P15/c24). Static linear response to a constant source on each massive graviton mode: h = ρ η/(3 m_a² M²). Per real bosonic degree of freedom this gives
  δ_rms = D · M₁⁴ / (96π² M₄² m_g1²),
  with D a dimensionless shape factor computed on the chain, M₁ the matter copy gap and m_g1 the lowest graviton copy mass.
- Induced Einstein–Hilbert weight (ξ = 0 scalar): leaf coefficient ∝ Σ_k a_kn I(M_k)/6.

## 3. Results (c32) [Computed]
**Light mode alone:** t_n ∝ w_n to 1e-13, so the light matter's vacuum energy is a pure common-mode cosmological constant.

**Counting every copy is not physical:** it does not converge with the grid (relative part 7.7e9 → 3.3e11 → 1.3e13 as Δy halves). It is dominated by lattice-scale copies, the same error P18 corrected for the mass term. The physical readings follow.

**Wilsonian (copies above Λ removed), relative cosmological constant, units M₁⁴/16π² per real dof (Y_c = 1.5, plain hopping):**

| Λ/M₁ | 0.9 | 1.2 | 1.5 | 2 | 3 | 5 | 10 | 30 |
|---|---|---|---|---|---|---|---|---|
| relative rms | 7e-14 | 0.096 | 0.14 | 5.2 | 52 | 950 | 3.2e4 | 7.3e6 |
| gravity shape D | 2e-14 | 0.014 | 0.020 | 0.62 | 7.6 | 150 | 4.9e3 | 1.1e6 |

- Grid-converged to a few percent (Δy = 0.05, 0.025, 0.0125).
- Y_c = 1.0–2.0 changes D by up to about 4×; F-weighted hopping raises it 4–40×.
- The relative part is 0.3–0.5 of the common part once several copies are inside the cutoff.

**Threshold floor:** integrating out the lowest K copies (dim reg, μ_R = M₁) leaves D ≈ 0.2 (K = 1), 0.14–0.22 (K = 2), 3.5–11 (K = 4). This is the natural size even when the EFT cutoff sits below M₁.

**Physical sizes (δ_rms per real dof; Yukawa strength of light matter to graviton copies α ~ δ²):**

| Branch | prefactor M₁⁴/(96π²M₄²m_g1²) | δ at Λ = 1.5 / 3 / 10 M₁ |
|---|---|---|
| TeV, M₁ = 1.73 TeV, m_g1 = 2 TeV | 4e-34 | 8e-36 / 3e-33 / 2e-30 |
| TeV top, M₁ = 20 TeV, m_g1 = 23 TeV | 5e-32 | 1e-33 / 4e-31 / 3e-28 |
| mm, M₁ = 1 TeV, m_g1 = 4e-5 eV (≈ 5 mm) | 0.11 | 2e-3 / 0.8 / 5e2 |

- mm floor from the first copy alone: δ ≈ 0.11 × 0.2 ≈ 0.02 per dof. With order 100 Standard Model degrees of freedom (bosons and fermions enter with opposite signs, no general cancellation), δ = O(1).
- δ scales as M₁⁴/m_g1². Staying natural in the mm branch would need matter copies below about 0.3 TeV, which P5's collider estimate (≳ 0.6–1 TeV) already excludes.

## 4. Reading [Derived]
- The gravity-sector couplings (Einstein–Hilbert weight, localizer) are gravitational-strength, so matter loops shift them only by ~Λ²/M₄² relative. That is why the F-weighting of gravity is stable.
- The relative cosmological constant is different: it is opposed only by the graviton copies' mass, so its effect is (Λ/M₄)²(Λ/m_g)²/16π². That is harmless when graviton copies are as heavy as matter copies (TeV branch). It is fatal when they are 10¹⁶ times lighter (mm branch).
- Light matter (Standard Model fields as flat modes) contributes only to the common cosmological constant. The relative part comes entirely from copies.

## 5. P14 common mode
- Matter loops at this order feed the common mode only through the ordinary cosmological constant.
- P14's open item (the parent's cubic inter-leaf potential and whether the Q self-Galileon cancels) is a tree-level gravity-sector question. Matter loops do not settle or change it.

## 6. Limits and open items
- One real scalar as the representative degree of freedom; fermion and gauge copies are expected to give the same structure with their own signs [Assumed]. Static, linear Fierz–Pauli response; constant tadpoles; sharp Wilsonian cutoff; core box. O(1) factors (Fierz–Pauli conventions, box-to-continuum mapping of m_g1 ≈ tensor gap) are not pinned down. The TeV verdict has ~28 orders of margin, so they do not matter there. In the mm branch they move the crossing by O(1) in M₁.
- Not computed: the localizer (Q) tadpole from matter loops. It is gravitational-strength with mass m_Q ≈ 340 κ, so it should be smaller than the graviton response by about (m_g/m_Q)² [Derived estimate].
- Still open: non-abelian groups with a Higgs Yukawa; graviton loops; a gauge-invariant chiral regulator; P14's cubic potential; the matching test being developed in a separate AI-assisted session.

## 7. Files
Script and output (not included in this release): `c32_matter_into_gravity.py`, `c32_out.txt`.

Requirements: Python 3, numpy.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN v8" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.

Other working notes referred to by label:

- P2: [WN-04](WN-04_P2Parent.md)
- P5: [WN-24](WN-24_P5CommonScale.md)
- P14: not included in this release.
- P15: [WN-05](WN-05_P15ParentClosure.md)
- P18: [WN-08](WN-08_P18RegulatedLoop.md)
- P20: [WN-28](WN-28_P20ChiralParent.md)

Material named in this note but not included in this release: `c32_matter_into_gravity.py`, `c32_out.txt`.
