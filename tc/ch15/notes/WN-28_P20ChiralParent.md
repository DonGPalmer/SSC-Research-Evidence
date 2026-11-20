> **Public edition of evidence note WN-28.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P20ChiralParent.md`, a working note dated 9 November 2026. Not peer reviewed.
> - **Source content hash:** `031cadde1039ab7ea8210f64be2fe1702f29a479eec39f934aa52a7c895d7b19` (7065 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** Several of its claims are corrected in [WN-29](WN-29_P20bReviewCorrections.md) and [WN-30](WN-30_P22SelfEnergyWard.md). Editorial notes mark the affected passages; the original wording is kept.

# SS WS1 P20: chiral per-leaf fermions, regulator check, and a decision on the per-leaf parent

Date: 9 November 2026. Status: **working note, unreviewed AI calculation, noncanonical.** Written on the author's instruction "Please continue until you have a decision or a stop point" (9 Nov 01:40Z). Follows P18 and P19 (WS1). Labels: [Derived], [Computed], [Assumed], [Open].

## 1. Decision
> **Editorial note (public edition, 19 November 2026):** A later note restates this decision: a single charged chiral species is anomalous, so the chiral candidate is conditional on anomaly cancellation, and the cutoffs of about 4.5, 16 and 45 M₁ are first crossings of a chosen link-fluctuation tolerance, not derived physical cutoff bounds. The distortion at the link scales is corrected there to 5–7%, and in a further note to 6–10% once wavefunction and vertex corrections are included. See [WN-29](WN-29_P20bReviewCorrections.md) §1–§2 and [WN-30](WN-30_P22SelfEnergyWard.md) §5. The text below is unchanged from the working note.

**The per-leaf parent (P2) stands as a restricted effective theory for scalar, vector-like Dirac + Maxwell and chiral abelian matter.** Three conditions apply:
1. It holds in a weakly coupled core of the scale direction (|y| ≲ 1.5).
2. The cutoff must lie below the link strong-coupling scale: about 4.5, 16 or 45 times the fermion copy gap M₁ for photon/fermion gap ratio r = 0.3, 1 or 3.
3. Chiral fermions need symmetric link charges (½, ½).

Inside that regime:
- Light matter stays within about 5–10% of the flat (protected) profile.
- Charge universality is exact.

It is not a derivation of the Standard Model coupling. Untested: non-abelian groups, Higgs Yukawas, graviton loops, and matter loops feeding the gravity sector. **The matter-sector work reaches a stop point here.** The remaining threats are in other sectors (§6).

## 2. Regulator check for P19 (c29) [Computed]
c28's loop integrals were rerun with three regulators:
- **sharp:** sharp cutoff on k², as in c28.
- **expo:** smooth form factor exp(−k²/Λ²).
- **trunc:** Wilsonian truncation. Copies heavier than Λ are removed, and the remaining loop is in dimensional regularization, MS-bar at μ_R = Λ. This imposes flatness at Λ and is gauge invariant within the truncated tower.

Λ (in units of m₁) at which the vector-like light fermion's leakage reaches 1% / 10% (Y_c = 1.5, Δy = 0.05):

| r = μ₁/m₁ | sharp | expo | trunc |
|---|---|---|---|
| 0.3 | 2.5 / 4.0 | 2.0 / 4.0 | 4.0 / 16 |
| 1 | 7.9 / 16 | 6.3 / 13 | 20 / 40 |
| 3 | 32 / 50 | 25 / 40 | 20 / 126 |

> **Editorial note (public edition, 19 November 2026):** A later note withdraws the statement below that the sharp cutoff is the conservative end: the smooth cutoff is as strict or stricter in every case, and the truncated MS-bar reading is a different matching prescription that should be reported separately, not folded into a regulator band. See [WN-29](WN-29_P20bReviewCorrections.md) §2. The text below is unchanged from the working note.

- Hard and smooth cutoffs agree within about 25%. The Wilsonian reading loosens the 10% window by 2.5–4×.
- So P19's thresholds hold to within a factor of about 4, and the sharp cutoff is the conservative end.
- In the truncated scheme leakage starts only once an even (parity +) copy is below Λ, because odd copies cannot mix with the even light mode.

## 3. Chiral per-leaf fermion (c30) [Assumed model; Computed]
Model (deconstructed 5D fermion):
- Right-handed R_n on leaves, weight w_n, charge 1 under U(1)_n.
- Left-handed L_e on links, weight (w_n + w_{n+1})/2, charge ½ under each neighbouring U(1).
- Link field V_e = exp(iπ_e/2f_e), charge (½, −½).
- Hopping κω_e[L̄_e V_e† R_n − L̄_e V_e R_{n+1}] + h.c., with ω_e ∝ link weight and photon link constants f_e² ∝ link weight.
- Fermion and photon copies then share eigenvectors and have matched spectra: M_k = κ√h_k, μ_k = eφ√h_k, constant ratio r.

Tree level:
- Exactly one massless chiral mode, and it is flat (distortion 3e-15).
- Its charge is exactly 1, the same as every other species, because the flat photon couples to the total charge.
- Copy masses 1, 1.43, 1.89, … (M₁ = 1).

> **Editorial note (public edition, 19 November 2026):** A later note narrows the statement below that kinetic corrections cannot move the zero mode: it holds for the null vector of the p = 0 mass matrix, but wavefunction corrections can change the protected-source condition. A further note finds that wavefunction and vertex corrections do move the light source into the heavy photon copies, adding to the mass-matrix tilt with the same sign. See [WN-29](WN-29_P20bReviewCorrections.md) §2 and [WN-30](WN-30_P22SelfEnergyWard.md) §1, §4. The text below is unchanged from the working note.

One loop at p → 0 (sharp cutoff):
- Photon exchange and eaten-Goldstone exchange correct the L–R mass matrix. The zero mode is the null vector of the corrected matrix.
- Kinetic corrections vanish at p = 0 and cannot move it. π² tadpoles are proportional to the tree pattern and leave it flat.
- Mode sums were checked against a direct site-basis quadrature (agreement 3e-5).

Distortion ε_χ (W-norm of the non-flat part) in the core box (Y_c = 1.5; Δy = 0.1 and 0.05 agree within 5%):

| r | Λ = 1 | 3.2 | 10 | 32 | 100 | 10% at |
|---|---|---|---|---|---|---|
| 0.3 | 6e-3 | 4.4e-2 | 0.13 | 0.23 | 0.31 | 8 |
| 1 | 5.6e-4 | 7.8e-3 | 3.5e-2 | 8.8e-2 | 0.14 | 50–63 |
| 3 | 7e-5 | 1.7e-3 | 1.3e-2 | 4.2e-2 | 8.9e-2 | 160–250 |

- Below the copy gap ε_χ ∝ Λ⁴ (decoupling). Above it, growth is slow, roughly logarithmic.
- Reason: with matched spectra the equivalence-theorem coupling M_k/μ_k stays fixed up the tower, unlike P19's mass-type hopping.
- A smooth cutoff changes ε_χ by ≤ 15% (c31 A).
- Y_c = 4 gives a larger ε_χ at low Λ, but see §4: its tails are not perturbative.

## 4. Two conditions found (c31) [Computed]
> **Editorial note (public edition, 19 November 2026):** A later note narrows this condition: in this hopping construction the (½, ½) assignment cancels the link-tadpole tilt of the asymmetric assignment, but it is not shown to be the only consistent assignment and does not by itself protect the full quantum-corrected mode. See [WN-29](WN-29_P20bReviewCorrections.md) §2. The text below is unchanged from the working note.

**Symmetric link charges are required (c31 B).**
- With the usual asymmetric assignment (L_e charged only under the left leaf), the link tadpole multiplies only one hopping term, by ⟨Σ_e⟩ = 1 − ⟨π_e²⟩/2f_e².
- That tilts the zero mode on every link: a radiatively generated bulk mass, giving domain-wall-like localization.
- Example (Y_c = 1.5, r = 1): distortion 1.1e-3 at Λ = 3.2, 3.8e-2 at Λ = 10, and the mode is fully localized (0.999) at Λ = 32.
- The symmetric (½, ½) assignment cancels this exactly.

> **Editorial note (public edition, 19 November 2026):** A later note qualifies the link-scale cutoffs below as model diagnostics (first crossings of the chosen tolerance ⟨π²⟩/2f² = 0.1), not derived physical cutoff bounds, and corrects the distortion at those scales from "about 5%" to 6.62%, 5.35% and 5.50%. A further note gives 6–10% once wavefunction and vertex corrections are included. See [WN-29](WN-29_P20bReviewCorrections.md) §2 and [WN-30](WN-30_P22SelfEnergyWard.md) §4–§5. The text below is unchanged from the working note.

**Link strong coupling sets the real cutoff (c31 C).** Λ at which the largest per-link ⟨π_e²⟩/2f_e² reaches 0.1:

| Y_c | r = 0.3 | r = 1 | r = 3 |
|---|---|---|---|
| 1.0 | 7.1 | 25 | 71 |
| 1.5 | 4.5 | 16 | 45 |
| 2.0 | 2.8 | 8.9 | 28 |
| 4.0 | 0.32 | 1.0 | 3.2 |

- The link constants scale with the leaf weight, so the tails (small sech⁴ y) are strongly coupled. This is the gauge-sector version of P15's strongly coupled copies at |y| ≳ 1.1–1.7.
- At Y_c = 4 the tails are already non-perturbative near Λ ≈ M₁, so the Y_c = 4 numbers in c30 are not reliable.
- In the core box, at the link scale (4.5 / 16 / 45 M₁), ε_χ ≈ 6% / 5% / 5%. So the chiral zero mode stays within about 5% of flat wherever the theory is perturbative.

## 5. Corrections to P19
> **Editorial note (public edition, 19 November 2026):** A later note withdraws the statement below that the sharp cutoff is the conservative end (see the editorial note in §2), and agrees that P19's Y_c = 4 scans should be kept as exploratory, not as evidence of a perturbatively controlled parent. See [WN-29](WN-29_P20bReviewCorrections.md) §2. The text below is unchanged from the working note.

- P19's Y_c = 4 scans were not checked for link strong coupling. Read P19 through its Y_c = 1.5 results. A uniform-f link sector should be checked the same way.
- P19's thresholds carry a regulator uncertainty of up to about 4× (§2), and the sharp cutoff is the conservative end.

## 6. Open, and what would change the decision
- **Matter loops feeding the gravity sector [Open, most important].** Per-leaf vacuum energy and matter-induced corrections to the gravity weights F_n (P15's regulator lemma, P14 common mode). If these destroy the F-weighting faster than the matter sector does, the window shrinks.
- **Non-abelian groups and Higgs Yukawas [Open].** Per-leaf Higgs copies give the chiral zero modes masses. The Yukawa needs the same protection test.
- **Graviton loops [Open].**
- **Species dependence.** Neutral species get no photon-loop distortion. Charged species' ε_χ scales with q². Heavy-graviton couplings of light matter (∝ ε_χ) are therefore species dependent at order ε_χ, which the matching test should bound.
- **Probe matching** is handled in a separate AI-assisted session (a coordination note, not included).

## 7. Files
Scripts and outputs (not included in this release): `c29_regulator_check.py`, `c29_out.txt`, `c30_chiral_zero_mode.py`, `c30_out.txt`, `c31_chiral_checks.py` (reads c30), `c31_out.txt`.

Requirements: Python 3, numpy, mpmath.

---

## References and related notes (public edition)

Other working notes referred to by label:

- P2: [WN-04](WN-04_P2Parent.md)
- P14: not included in this release.
- P15: [WN-05](WN-05_P15ParentClosure.md)
- P18: [WN-08](WN-08_P18RegulatedLoop.md)
- P19: [WN-27](WN-27_P19DiracMaxwellParent.md)
- P20: [WN-28](WN-28_P20ChiralParent.md)

Material named in this note but not included in this release: `c29_out.txt`, `c29_regulator_check.py`, `c30_chiral_zero_mode.py`, `c30_out.txt`, `c31_chiral_checks.py`, `c31_out.txt`.
