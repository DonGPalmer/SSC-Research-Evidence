> **Public edition of evidence note WN-31.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P23NonAbelianHiggs.md`, a working note dated 9 November 2026. Not peer reviewed.
> - **Source content hash:** `8f1918a8d02fffd5ea8de751c046e883fbd05712c99056d742b86f674175802a` (5476 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# SS WS1 P23: non-abelian chiral matter and a per-leaf Higgs with a top Yukawa

Date: 9 November 2026. Status: **working note, unreviewed AI calculation, noncanonical.** Written on the author's "Yes" (9 Nov 15:11Z) to building non-abelian matter with a Higgs Yukawa on the TeV branch (P20b gate 2). Follows P20, P20b, P22 (WS1). Labels: [Derived], [Computed], [Assumed], [Open].

## 1. Decision
**Standard-Model-like gauge groups and chiral quarks fit the per-leaf parent only in a narrow window, and a per-leaf Higgs does not fit.**
- Colour sets the window for the fermions. At r = μ₁/M₁ = 1 the light quark stays within about 10% of flat only for Λ ≲ 3 M₁ (gauge-exchange tilt 7.6%, plus wavefunction and Yukawa terms). r = 0.3 fails already at Λ = 2 (22%). r = 3 holds to Λ ≈ 8–10 M₁ (§3).
- The Higgs is the binding constraint. The top loop gives each leaf a Higgs mass that is not proportional to its weight w_n, and that tilts the Higgs zero mode by order one unless its copies are much heavier than the fermion copies: m_H1 ≳ 1.9, 3.5, 7, 21 M₁ for Λ = 2, 3, 5, 10 M₁ (§4). That puts the Higgs copies at or above the cutoff, so in the low-energy theory the Higgs is one rigid, flat field, not a per-leaf field. The alternative is to tune the Higgs mass on every leaf (N − 1 tunings).
- On the TeV branch (M₁ ≈ 0.6–11 TeV, P5) the window means a cutoff of a few times M₁: about 2–30 TeV at r = 1.

## 2. Non-abelian links [Derived; Computed]
- The link field is a bifundamental (N, N̄) of SU(N)_n × SU(N)_{n+1}. There is no "half charge", so P20's symmetric (½, ½) link fermion has no non-abelian analogue.
- Two constructions remain:
  - **ASYM:** L_e in (N, 1), hopping L̄_e R_n − L̄_e Σ_e R_{n+1}. The link tadpole multiplies only the second term and tilts the zero mode.
  - **MID:** a gauge group at each link midpoint, L_e in its fundamental, two half-links. Each hopping term gets its own half-link tadpole. The two nearly cancel, leaving a gradient-suppressed tilt.
- Coupling strength enters as F = C_F g²/e² (one loop, fixed copy spectrum; normalisation as c31 [Assumed]). Near 1 TeV: SU(3) F = 16.3, SU(2) 3.35, U(1)_Y 1.41.
- Link strong-coupling scale (largest per-link tadpole reaches 0.1), Y_c = 1.5, in M₁ (c36 A1):

| group | r = 0.3 | r = 1 | r = 3 |
|---|---|---|---|
| SU(3) | ASYM 1.3, MID 2.0 | ASYM 4.5, MID 6.3 | ASYM 12.6, MID 20 |
| SU(2) | 2.0 / 3.2 | 7.1 / 10 | 20 / 32 |
| U(1)_Y | 2.8 / 4.0 | 8.9 / 14 | 28 / 40 |

- Tadpole-only tilt: MID is about 40–60× smaller than ASYM (c36 A2). SU(3), r = 1, Λ = 3: ASYM 3.1%, MID 0.07%. Both fall with grid spacing (Δy = 0.05: ASYM 1.5%, MID 0.02%; c36 A3), so ASYM's tilt is partly a lattice effect, but MID is the safer construction.

## 3. Gauge-exchange tilt of the light quark (c36 B) [Computed]
MS-bar, truncated, Y_c = 1.5, Δy = 0.1. The c35 tilt with coupling factor F, recomputed from the null vector.

| | Λ = 2 | 3 | 5 | 10 |
|---|---|---|---|---|
| SU(3), r = 0.3 | 22% | 29% | 38% | 50% |
| SU(3), r = 1 | 2.5% | 7.6% | 14% | 21% |
| SU(3), r = 3 | 0 | 0 | 3.4% | 9.1% |
| SU(2), r = 0.3 | 7.0% | 12% | 18% | 28% |
| SU(2), r = 1 | 0.5% | 1.9% | 4.7% | 9.0% |
| SU(2), r = 3 | 0 | 0 | 0.8% | 3.3% |

(Zero where no gauge copy lies below Λ.) Wavefunction and vertex terms add about a third on top (P22, scaled by F: about 2% for SU(3), r = 1, Λ = 3). The non-abelian vertex diagram (triple-gluon, C_A) is not computed [Open].

## 4. Per-leaf Higgs and top Yukawa (c37) [Computed]
Model: chiral quark doublet Q and singlet t on the moose, a per-leaf Higgs H_n with its own hopping (copies m_Hj = s M_j), leaf-local Yukawa y Σ_n w_n Q̄_n H_n t_n with light top Yukawa y_t = 0.94. MS-bar, truncated, r = 1, Y_c = 1.5.
- **Higgs tilt (C1):** the top loop gives a leaf mass matrix Π_nm whose non-flat part feeds the Higgs copies. First-order tilt ε_H at s = 1: 0.37 (Λ = 2), 1.2 (Λ = 3), 4.8 (Λ = 5). Above about 0.3 the first-order number only says the tilt is order one. It scales as 1/s², so ε_H ≤ 0.1 needs m_H1 ≥ 1.9, 3.5, 7.0, 21 M₁ for Λ = 2, 3, 5, 10 (C3). Grid check Δy = 0.05 agrees within 15%.
- Zero-mode Higgs mass shift: +0.44, +1.5, +6.8 M₁² at Λ = 2, 3, 5. This is the usual hierarchy question; it is tuned by one zero-mode parameter, not leaf by leaf.
- **Yukawa leakage of the light quark into gluon copies (C2):** 0.4%, 0.9%, 2.4%, 6.7% at Λ = 2, 3, 5, 10. Ward identity for this loop holds to 1e-15.

## 5. Open, and what would change the decision
1. Gauge-boson and Higgs-quartic contributions to the Higgs leaf masses are not included; they change the leaf masses at the same order (gauge loops with the opposite sign).
2. A protected Higgs (Goldstone or gauge-component Higgs from the link fields, as in deconstructed gauge-Higgs unification) could remove the leaf-mass problem. This is the most promising route for the Higgs and is not examined.
3. The C_A vertex diagram, box diagrams and gauge-parameter independence (P22 open items).
4. Gate 3 (P21 redone with chiral, non-abelian content) is still open.
5. P5's TeV-branch range of M₁ is taken as given.

## 6. Files
Scripts and outputs (not included in this release): `c36_nonabelian_links.py`, `c36_out.txt` (reads c35, c34, c30); `c37_top_yukawa.py`, `c37_out.txt` (reads c34 and c30).

Requirements: Python 3, numpy.

---

## References and related notes (public edition)

Other working notes referred to by label:

- P5: [WN-24](WN-24_P5CommonScale.md)
- P20: [WN-28](WN-28_P20ChiralParent.md)
- P20b: [WN-29](WN-29_P20bReviewCorrections.md)
- P21: [WN-25](WN-25_P21MatterIntoGravity.md)
- P22: [WN-30](WN-30_P22SelfEnergyWard.md)

Material named in this note but not included in this release: `c36_nonabelian_links.py`, `c36_out.txt`, `c37_out.txt`, `c37_top_yukawa.py`.
