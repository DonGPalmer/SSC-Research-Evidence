> **Public edition of evidence note WN-16.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P6ReflectionFold.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `55b1f12f123e7ab8476c815bd7b8d78e43283c888564a05b8f494f62ba39e91f` (8004 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** Its attribution of the tensor-exclusion sentence to SS-DYN v8 is corrected in [WN-18](WN-18_P11Rev.md) and [WN-19](WN-19_P11bDYNWording.md). An editorial note marks the affected passage; the original wording is kept.

# P6. Reflection: fold or symmetry? The decisive fork for the common-scale option

WS1 working note, 8 November 2026. Working material only: not reviewed, nothing published.
Follows [WN-24](WN-24_P5CommonScale.md). Script: `c15_reflection_goldstone.py`; output: `c15_out.txt` (not included in this release).

## 1. Verdict

The TeV common-scale option of P5 turns on one rule the framework has not stated: is the mirror reflection of the scale axis about the kink centre, P: (λ − λc) → −(λ − λc) with X → −X, a **fold** (configurations related by P are the same state, so only P-even states exist) or only a **symmetry** (P-odd states are physical and stable against decay into P-even ones)?

- **Fold.** The √3κ partners of every field are removed, and so is the kink's translation mode. The TeV option survives on the P5 bounds (about 0.6 TeV ≲ κ ≲ 4 to 11 TeV, crude collider analogy at the low end). Its matter-side signal is a single continuum threshold at 2κ, the same for gravity and every matter field. The 3 : 4 partner-to-threshold ratio that P5 put forward as the signature is not observable.
- **Symmetry.** The partners exist, but they are not the lightest P-odd states: a massless scale-shift (translation) mode is. Every partner decays into it with Planck-suppressed strength, after roughly 20 s to 2 × 10^5 s across the window, which is during big-bang nucleosynthesis. With an ordinary thermal history this is very likely excluded (section 5). The only clear escape is a reheating temperature well below the partner mass.

> **Editorial note (public edition, 19 November 2026):** Later notes find that SS-DYN v8 contains no exclusion of the 3κ² tensor state: the sentence quoted below ("excluded from the even leaf-metric sector") is in SS-DYN v6 and SS-PHEN v2, not v8. They confirm that v8 declares the odd perturbation family, the fixed centre and the odd scalar pencil. See [WN-18](WN-18_P11Rev.md) F6 and [WN-19](WN-19_P11bDYNWording.md) §4. The text below is unchanged from the working note.

SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)'s own construction already behaves as a fold: it removes the odd 3κ² tensor state ("excluded from the even leaf-metric sector"), keeps the localizer's odd-function sector (which is P-even and holds the Q pole), has no translation mode in its scalar spectrum, and treats λc as a fixed datum. **Recommendation: state the fold explicitly as a rule of the architecture and apply it to matter.** The P5 claim of a 1.155 level spacing is withdrawn; it holds only in the disfavoured symmetry reading.

## 2. Parity assignments (c15 §1)
- Action: F(X) = (1 − X²/v²)² is even; the localizer square and the gradient term are invariant under P; protected matter enters through F, so P is a symmetry of eq. (Sspec) with matter.
- Gauge and Higgs: zero mode flat (P-even); partner raw profile N1 sinh y, odd (P-odd).
- Fermions: kink mass m(X) ψ̄ψ is invariant with ψ → ±γ5 ψ. Choosing −γ5 for doublets and +γ5 for singlets makes every chiral zero mode P-even and leaves the Yukawa term invariant. The Dirac partner (L component odd function, R component even function) is P-odd as a whole.
- Localizer: odd-function δX (the Q sector, f̂ = −4 tanh y sech² y) is P-even. Even-function δX, which contains the translation mode sech² y, is P-odd.

## 3. The translation (scale-shift) mode (c15 §2, §3)
- The action has no explicit λ, so λ-translation is a global symmetry broken by the kink.
- K̂ sech² y = 0 and ⟨f̂, sech² y⟩ = 0, so in DYN's pencil the mode has zero mass for every r > 0. The box check gives zero (to discretization) next to the Q pole at 340.91 (DYN: 340.936).
- Decay constant: f_a² = rZ_X ∫(∂λX0)² dλ = r ζ_X κ² M4², so its couplings to κ-scale structure are of order 1/(√(r ζ_X) M4): Planck-suppressed. r ζ_X is 0.18 to 0.47 in the window.
- At the millimetre benchmark this mode is harmless (P-odd, so no linear coupling to protected matter, hence no fifth force). In the symmetry reading it is still an extra massless scalar that DYN's degree count does not list.
- Caveat: Scale Space geometry pairs scale shifts with spatial dilations (the T_c map in the Scale Space geometry notes). If the true symmetry is that combined one, ordinary mass scales may give this mode a mass; this has not been worked out.

## 4. Partner couplings and decays (c15 §4, §7)
- Tree couplings repeat the minimal universal-extra-dimension pattern: f0-f0-A1 = 0, f0-f1-A1 = g4 exactly, f1-f1-A0 = g4. A1 links f0 only to f1 (ψ0·sinh y is exactly proportional to ψ1), so there is no f0-continuum coupling.
- Couplings to the translation mode: d_A = 3π/(4√2) for gauge and Higgs, d_f = 3π/(8√2) for fermions.
- Widths (massless final states): vector d_A² m³/(96π r ζ M4²), scalar d_A² m³/(64π r ζ M4²), fermion d_f² m³/(32π r ζ M4²), with m = √3κ.
- Lifetimes, over the r window: about 1–2 × 10^4 s at κ = 1 TeV, about 300–800 s at 4 TeV, and 17–35 s at 11.35 TeV (falling as κ^-3).

## 5. Nucleosynthesis comparison (symmetry reading only)
- Partners are degenerate at tree level, so they freeze out together. Rough relic before decay (c15 §5):
  - generous colour-dominated annihilation (σv = 10π αs²/m²): m Y ≈ 1e-11 GeV at κ = 1 TeV, 2e-10 at 4 TeV, 1.6e-9 at 11 TeV;
  - unitarity floor: about 100 times lower.
- The decays carry TeV-scale energy, and colored partners decay to gluons (hadronic branching ≈ 1).
- Kawasaki, Kohri, Moroi and Takaesu (arXiv:1709.01211) say in their text that the 4He constraint is strongest for τ ≲ 10² s and D overproduction from hadrodissociation is strongest for 10² to 10⁷ s. The only bound value their text states is a constraint around m Y ~ 1e-9 GeV, from D overproduction via a larger n/p (b b̄ decays). Their limits at the lifetimes here are given only in figures, which were not read for this note.
- Status: for κ ≲ 4–6 TeV (τ ≳ 10² s) the predicted m Y lies in the regime the paper calls most constraining. Exclusion is likely but not confirmed against the figures. Near the top of the window (τ ~ 20–100 s) the comparison with ~1e-9 GeV is marginal.
- To settle this, read the hadronic-decay figures of 1709.01211 at m = 1–20 TeV.

## 6. The continuum (flag, not resolved; c15 §7)
- Fields with weight F have local coupling g5²/F(λ), which grows as cosh⁴ y away from the centre.
- At energy E ~ 2κ, gauge couplings become strong beyond roughly 1.5 to 2 widths from the centre (QCD first).
- Continuum states spread into that region. Their mutual interactions, and the link between two partners and the continuum (whose overlap tends to a constant, N1² tanh² y), are dominated by it.
- Consequence: the continuum's threshold location (2κ) is reliable, but its production rates and decays are not calculable in the weakly coupled theory. This affects collider predictions above 4κ.
- Whether the lightest continuum states decay promptly is open: tree-level single-excitation vertices vanish, and loop-level decays are expected but not shown.

## 7. What changes
1. P5: drop the √3κ partner and the 1.155 ratio from the TeV branch; keep the window, with the collider floor from the continuum-only line (κ ≳ 0.55–0.75 TeV, crude).
2. Paper-20 [retired series; see References] matter obstruction: with the fold, the √3 c_i κ partners never existed. The obstruction reduces to the matter continuum at 2 c_i κ, which is still far too light at the millimetre scale.
3. Scale spectroscopy (P3): only P-even levels are observable. For the l = 2 operator that leaves 0 and the 4κ² threshold, so the across-scale test becomes "the same threshold in every sector" rather than a 3 : 4 ratio. Discrete ratio tests need operators with two or more even bound levels (l ≥ 3).
4. Meaning for SSF: the fold makes λc a mirror point of the scale axis. Scales e^{λc+δ} and e^{λc−δ} label the same leaf. That pins the centre (no translation mode), but it is a physical statement about scale space that needs its own justification.

## 8. Open points
- Read the BBN figures to close or reopen the symmetry reading.
- Decide whether the fold is a postulate or follows from the Scale Space geometry; check the T_c combined symmetry.
- Far-region strong coupling of weight-F fields: is it physical, or a sign that the F weight must be cut off?
- Decay of the lightest continuum states under the fold.

## 9. Files
- This note. Script `c15_reflection_goldstone.py` and output `c15_out.txt` (not included in this release).

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **Paper 20**: D. G. Palmer (2026). *Paper 20: Dynamical Closure of the Scale-Space Framework: Complex Scale Potential, Newtonian Recovery, and the Hidden Configurational Sector*. Zenodo. Retired series (historical record), replaced by SS-DYN; published versions v2 to v10, the last being version 10, [doi:10.5281/zenodo.21684395](https://doi.org/10.5281/zenodo.21684395). The Paper 20 gate documents this note refers to (for example P20_NS_gate_v1) are unpublished working documents and are not included.

Other working notes referred to by label:

- P3: [WN-14](WN-14_P3ScaleSpectra.md)
- P5: [WN-24](WN-24_P5CommonScale.md)
