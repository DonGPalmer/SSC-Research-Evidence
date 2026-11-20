> **Public edition of evidence note WN-26.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P24ScaleKinkWeight.md`, a working note dated 9 November 2026. Not peer reviewed.
> - **Source content hash:** `6552e119699ba50f1cbc9d48ce6c7f52d4c184bf5eac488f61a9a7bec1b983eb` (6869 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# SS WS1 P24: the sech⁴ weight is the localizer's own BPS flow, squared

Date: 9 November 2026. Status: **working note, unreviewed AI calculation, noncanonical.** Written on the author's instruction (9 Nov 15:34Z): "Please work on the sech^4 weight item to see if we can get any improvement in the foundation." Follows P3, P5, P23 (WS1). Labels: [Derived], [Computed], [Read], [Literature] (cited from memory, not re-read), [Conjecture], [Open].

## 1. Decision
**Yes, one real gain: sech⁴ need not be an independent input.** SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)'s localizer is already a Bogomolny perfect square with flow function f(X) = 1 − X²/v_X². Five items that DYN and WS1 state separately are all f:
- the kink X₀ = v_X tanh y (DYN derives this one);
- the weight F(X) = f(X)², which DYN states without derivation;
- the warp e^𝒜 = f(X₀) = sech² y, which DYN also states;
- W₀ = 4/(3κ), the kink's topological charge W(+v) − W(−v);
- the chiral fermion operator D + 2κ tanh y (DYN v6), which is the coupling that keeps the light fermion flat.

The cost is one postulate in place of those statements: **matter's weight on each level equals the localizer's gradient energy density there**, F = X′²/(κv_X)². This also fixes P20's free ratio r at 1 and ties every matter threshold to the mass of the localizer quantum, 2κ.

It does not fix the loop problems of P17–P23 by itself. It says what has to be protected: the ratio of matter couplings to the localizer flow (§4).

## 2. What DYN already has [Read, SS-DYN v8 and the v6 extract]
- B[X] = ∂_λX − κv_X(1 − X²/v_X²) and U = (Z_X/2)∫B²: a perfect square, solved by X₀ = v_X tanh y.
- F(X) = (1 − X²/v_X²)², "stated"; no reason given for the square or the exponent.
- e^𝒜 = sech² y, "retained localized parent comparison", not solved.
- W = ∫F dλ, W₀ = 4/(3κ), M₄² = M₅³W₀; the v8 valley section has the boundary identity ∫x′(1 − x²)dy = W.
- v6: chiral fermion operator D_λ + 2κ tanh y with kernel sech² y.
- DYN never names the superpotential, BPS, domain-wall or Jackiw–Rebbi structure, and never notes that F = f² or e^𝒜 = f.

## 3. Derivations and checks (c38) [Derived; Computed]
With W(X) = X − X³/3 (v_X = 1, κ = 1), all identities were checked symbolically:
- BPS equation X′ = W′(X) gives tanh y. Its energy density X′² = W′(X₀)² = sech⁴ y = F, and F(X) = W′² = 2V(X).
- The localizer's fluctuation operator −∂² + V″(X₀) is −∂² + 4 − 6 sech² y (Pöschl–Teller ℓ = 2). The F-weighted matter operator −(1/F)(Fχ′)′ is the same operator under χ = ψ/√F. A localizer quantum has mass² V″(±1) = 4, so mass 2κ.
- **Flatness lemma.** A chiral zero mode ψ₀ = exp(−∫W_f) is flat in the F-norm if and only if W_f = −(ln√F)′ = 2 tanh y. That means Yukawa g = 2 = |W″(±1)|, the BPS value.
- **Supersymmetric pair.** With W_f = 2 tanh y, Q†Q = −∂² + 4 − 6 sech² has spectrum {0, 3, ≥ 4} and QQ† = −∂² + 4 − 2 sech² has {3, ≥ 4}. Both chiralities share the partner at √3κ and the threshold at 2κ, and the gauge field (weight F) has the same spectrum. So P20's photon-to-fermion gap ratio is r = 1.
- **Jackiw–Rebbi.** Perturbing W_f by smooth bumps of size 0.3–0.9 leaves the zero mode at 10⁻¹² (exactly massless), while its flatness error goes from 0.002 to 0.17–0.43. Existence is topological; flatness is the BPS relation and nothing else.
- **W₀ is topological.** ∫sech⁴ = W(1) − W(−1) = 4/3, the kink's charge. So on the BPS solution M₄² = M₅³ × (kink charge), which depends only on the two vacua, not on the profile's details.

## 4. What it changes
- **Box versus line.** P20–P23 worked in a box |y| ≤ 1.5. There the first copy is M₁ = 1.866κ (line value √3κ = 1.732κ) and M₂/M₁ = 1.433, where the line has a continuum from 1.155 M₁. The box levels above M₁ are box artefacts (c38 B; Y_c = 6 and 12 recover 0, 3, 4.0 …). The windows "Λ ≲ 3 M₁" of P23 are about Λ ≲ 5.6κ, or 2.8 times the 2κ threshold.
- **Leakage.** On this reading the P20–P23 tilt is a loop-induced departure of the matter couplings from the BPS relation. Supersymmetry along the scale direction would protect that relation (standard for BPS kinks) [Literature; Conjecture for SS]. Without it, nothing does, and the narrow windows stand.
- **Far region.** F = f² → 0 where the localizer sits in its vacuum, so gauge couplings g²/F become strong there. P8, P17 and P20 treated this as a pathology. In domain-wall physics it is the Dvali–Shifman mechanism: a confining bulk is what localizes the gauge field on the wall (Dvali and Shifman 1997) [Literature; Conjecture for SS].
- **Prior art.** The structure is a φ⁴ domain wall in the scale direction: Rubakov–Shaposhnikov localization (1983), the Jackiw–Rebbi zero mode (1976), and the kink's internal mode at √3/2 of the meson mass (standard) [Literature]. What is new for SS is that scale is the wall's transverse direction and that one flow function fixes DYN's separately stated items.

## 5. What it predicts that a plain extra dimension does not (c38 D, D2) [Computed]
A source at our level (y = 0) sees only the even states. The fold removes the odd partner at √3κ.
- **No discrete copies.** There is only a continuum starting at 2κ, the same threshold for every species and the localizer quantum. A flat orbifold gives an even tower at 2n/R (ratios 2 : 4 : 6); a warped (RS) interval gives a discrete Bessel tower.
- **Threshold rise.** The spectral density is ρ(s) = (s − 3)/(2πs√(s − 4)), s = m²/κ², reflectionless. It is checked against the scattering solution to six digits. The 1/√(s − 4) rise at threshold needs integer ℓ: the control 4 − 5 sech² is 40× lower at s = 4.001 and 0.6 of ℓ = 2 at s = 4.05.
- **Pinning the exponent.** sech⁶ would add an even partner at √8κ below its threshold 3κ, and sech² has no partner level. "No even partner, threshold rise at 2κ, odd partner at √3κ" picks sech⁴.
- **Scale not fixed.** κ stays free. P5's TeV range was set by other bounds.

## 6. Open
1. Why F = f²: the postulate (weight = localizer energy density) is stated, not derived. A scale-direction supersymmetry would derive it and would also protect it.
2. Redo a leakage gate on the full line with the continuum, treating the far region as Dvali–Shifman confinement instead of a box.
3. Graviton: DYN's tensor operator is the same ℓ = 2 problem (P3). Check whether e^𝒜 = f follows from a 5D BPS (fake-supergravity) flow or stays a comparison.
4. P23's Higgs problem is untouched.

## 7. Files
Script and output (not included in this release): `c38_bps_kink_weight.py`, `c38_out.txt`.

Requirements: Python 3, numpy, sympy.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v6** (written "DYN v6" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: A Scale-Localized Leafwise Dynamical Closure for Scale Space: Protected Tensor Gravity, a Repaired Scalar Continuum, and Constrained Collective Matter* (version 6). Zenodo. [doi:10.5281/zenodo.23604782](https://doi.org/10.5281/zenodo.23604782). Published; superseded by version 8 ([doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)).
- **SS-DYN v8** (written "DYN" in this note): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.

Other working notes referred to by label:

- P3: [WN-14](WN-14_P3ScaleSpectra.md)
- P5: [WN-24](WN-24_P5CommonScale.md)
- P8: [WN-22](WN-22_P8CutoffBox.md)
- P17: not included in this release.
- P20: [WN-28](WN-28_P20ChiralParent.md)
- P23: [WN-31](WN-31_P23NonAbelianHiggs.md)

Material named in this note but not included in this release: `c38_bps_kink_weight.py`, `c38_out.txt`.
