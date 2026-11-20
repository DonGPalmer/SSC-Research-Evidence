> **Public edition of evidence note WN-29.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P20bReviewCorrections.md`, a working note dated 9 November 2026. Not peer reviewed.
> - **Source content hash:** `dea93d5cd67c2c112f549a7d61ad55bdd9249494dd799072342bb6c99db44d6d` (5601 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** Its 5–7% figure for light matter at the link scales is corrected to 6–10% in [WN-30](WN-30_P22SelfEnergyWard.md). An editorial note marks the affected passage; the original wording is kept.

# SS WS1 P20b: corrections to P20 after the AI-session review, and the anomaly count

Date: 9 November 2026. Status: **working note, unreviewed AI calculation, noncanonical.** Responds to an AI-session technical review of P20 (9 Nov 2026, 02:21Z). That review is not an independent external validation. P20 itself is left unchanged; this note records which of its claims stand, which are corrected and what was added. Labels: [Derived], [Computed], [Open].

## 1. Outcome
The review is right on all four points. The decision in P20 §1 is restated as:

> The per-leaf parent has a promising finite-chain chiral abelian realization. Its tree-level flat zero mode and bounded one-loop mass-matrix distortion are supported by reproducible calculations. A single charged chiral species is anomalous. With an anomaly-free set of zero-mode charges, every gauge anomaly of the moose cancels (c33). Wavefunction corrections, a gauge-invariant self-energy and Ward-identity check, and complete protected-current matching remain open.

The matter-sector stop point stays, with this narrower reading. P21 (matter loops into gravity) used scalar copies and does not depend on the chiral or anomaly questions. Its TeV-versus-mm branch result stands as written.

## 2. Corrections to P20

> **Editorial note (public edition, 19 November 2026):** A later note finds that, once wavefunction and vertex corrections are included, the distortion of light matter at the link scales given as 5–7% in the table below should read 6–10%. See [WN-30](WN-30_P22SelfEnergyWard.md) §5. The text below is unchanged from the working note.

| P20 claim | Status |
|---|---|
| §1, §6: the chiral candidate is a consistent per-leaf parent for chiral abelian matter | **Corrected.** One charged chiral species is anomalous: diagonal U(1)³ = 1, mixed U(1)–gravity² = 1 (c33 B). Every product-group anomaly is also nonzero: U(1)_n³ = 3/4 in the interior and 7/8 at the ends, U(1)_n²U(1)_{n+1} = −1/8. The candidate is conditional on anomaly cancellation (§3). |
| §4: "symmetric link charges are required" | **Narrowed.** In this hopping construction the (½, ½) assignment cancels the link-tadpole tilt that the asymmetric assignment produces. It is not shown to be the only consistent assignment. It does not by itself protect the full quantum-corrected mode. |
| §3: "kinetic corrections vanish at p = 0 and cannot move it" | **Narrowed.** This holds for the null vector of the p = 0 mass matrix, which is what c30 computes. The leaf distribution that matters for coupling to the graviton copies uses the corrected kinetic weight, K_R + Σ_R(0) on each leaf. Wavefunction corrections can therefore change the protected-source condition even when the null vector stays flat. Not computed [Open]. |
| §1, §4: cutoff "about 4.5, 16 or 45 times M₁" | **Qualified.** These are first crossings of a chosen link-fluctuation tolerance, ⟨π²⟩/2f² = 0.1. They are model diagnostics, not derived physical cutoff bounds. |
| §1, §4: light matter within "about 5%" of flat at the link scale | **Corrected to 5–7%.** Distortion evaluated at those three scales: 6.62%, 5.35%, 5.50% (c33 A; the review found 6.61%, 5.35%, 5.50%). |
| §2, §5: "the sharp cutoff is the conservative end" | **Wrong; withdrawn.** The smooth cutoff is as strict or stricter in every case. At r = 1 the 10% threshold is 15.85 (sharp) and 12.59 (smooth). Smooth/sharp is 0.79–0.80, except r = 0.3 at 10%, where they are equal (c33 C). The truncated MS-bar reading is a different matching prescription and should be reported separately, not folded into a regulator band. |
| §5: P19's Y_c = 4 scans | Agreed with the review: keep them as exploratory, not as evidence of a perturbatively controlled parent. |

The same withdrawal applies to the posting of P20, which said the sharp cutoff gives the strictest numbers.

## 3. Anomaly cancellation (c33) [Derived; Computed]
- A species of charge q contributes q³ (cubic) and q (mixed gravitational) times a fixed pattern over the leaf groups. The pattern is the same for every species and is set by the moose: chirality s on sites, −s on links, link charges q/2 at each end.
- So every product-group anomaly, and the diagonal one, is proportional to Σ s q³ or Σ s q over species. **All of them cancel exactly when the light zero-mode content is anomaly free.** The Dirac copies are vector-like and contribute nothing net.
- Checked on N = 7:
  - A vector-like pair cancels identically.
  - The chiral anomaly-free set of left-handed zero modes with q = 1, 5, −7, −8, 9 (Σq = Σq³ = 0) gives every A_abc and A_a = 0.
- Caveat on that example: it uses large charges. The photon-loop distortion scales as q², so charge 9 would be strongly coupled at e ≈ 0.3. It shows the mechanism works; it is not a realistic sector.
- The realistic route is Standard-Model-like content, which is anomaly free only together with its non-abelian groups. That ties this to the open non-abelian + Higgs Yukawa item.
- Anomaly inflow (a Chern–Simons-type term in the deconstructed bulk) is an alternative not examined.

## 4. Next gates, in the review's order
1. Gauge-invariant self-energy, including wavefunction corrections Σ_R(0) per leaf, and a Ward-identity check of the light current.
2. Non-abelian extension with Standard-Model-like anomaly-free content and a Higgs Yukawa.
3. Matter loops into the gravity weights: done in P21 with scalars. Redo with the chiral content once gates 1–2 pass.

## 5. Files
Script and output (not included in this release): `c33_anomaly_and_checks.py` (reads `c30_chiral_zero_mode.py`), `c33_out.txt`.

The fuller version of the review that it mentions ("WS1 P20 chiral-parent technical review") was not available to this working note and is not included.

---

## References and related notes (public edition)

Other working notes referred to by label:

- P19: [WN-27](WN-27_P19DiracMaxwellParent.md)
- P20: [WN-28](WN-28_P20ChiralParent.md)
- P21: [WN-25](WN-25_P21MatterIntoGravity.md)

Material named in this note but not included in this release: `c30_chiral_zero_mode.py`, `c33_anomaly_and_checks.py`, `c33_out.txt`.
