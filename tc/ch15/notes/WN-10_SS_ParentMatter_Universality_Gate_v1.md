> **Public edition of evidence note WN-10.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `SS_ParentMatter_Universality_Gate_v1.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `b1bcaafeecad308abf3b287b4f85297455933611dc6fe81084cd96de66ccc155` (10652 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# Independent parent-to-DYN matter universality gate

**8 November 2026 · noncanonical research · separate from the WS1 working notes**

## Decision

**The universal physical matter metric is not derived by the available independent-leaf parent construction.** A precise **conditional sufficiency** statement and an **exact obstruction** can be established:

1. **Conditional sufficiency:** If the participating leaves share **exactly the same Lorentzian metric** \(g_i=g_J\), all light matter is restricted to a single diagonal multiplet, and the **total matter-action normalization is fixed, non-dynamical and species-independent**, then a sum of identical per-leaf minimal matter actions reduces to one universal action \(S_m[g_J,\psi]\), up to a constant normalization and consistently matched bare fields/parameters. In the canonical common-metric DYN Jordan action the Einstein rescaling \(g_E=\Phi g_J\) then fixes \(g_J=\Phi^{-1}g_E\). This is a consequence of the **declared** Jordan action and a conformal change of variables, not an independent derivation of the common-metric sector from the parent.
2. **Exact obstruction:** In the natural locked-field countermodel with conformal leaf metrics \(g_i=A_i^2g_E\), positive prescribed weights \(w_i\), one shared massive gauge-charged scalar and one Maxwell field, a universal minimally coupled conformal metric with the original common mass and charge does **not** exist if the \(A_i^2\) vary between participating leaves. It would require the weighted conformal-factor variance to vanish.
3. **Dynamical-weight obstruction:** Even if \(g_i=g_J\), promoting the overall matter prefactor \(W(X)=\sum_i w_i(X)\) to a dynamical localizer function introduces a direct source proportional to \(W_{,I}\mathcal L_m\), beyond the universal Jordan trace coupling, unless that variation vanishes or an independently justified mechanism cancels it.
4. These results identify missing assumptions in the proposed parent-to-DYN descent, but **do not prove no possible Scale Space parent could derive universality**. A specially constrained parent, a symmetry principle enforcing equal induced metrics, or justified microscopic matching might do so. None is established by the sources reviewed here.

## Source pinning and concurrent work

Sources read (read-only): `SS-DYN_leafwise_dynamical_closure_v8.tex` (LaTeX source of SS-DYN v8; not included) (canonical SS-DYN v8 [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)); [WN-04](WN-04_P2Parent.md), [WN-15](WN-15_P4CouplingWeight.md), [WN-24](WN-24_P5CommonScale.md), [WN-20](WN-20_P12FoldDilation.md), [WN-21](WN-21_P13L5DScaleGeometry.md); `WS3_AtomicBridge_v1.md` (not included); the author's internal project guide and logging standard (not included). This work was performed **without editing canonical files**. This result is a separate universality/identifiability lemma, not a competing parent design.

Canonical DYN v8 explicitly says its ordinary matter is one four-coordinate EFT coupled to one physical metric, *not* the same scalar independently coupled to multiple metrics. It says the parent comparison has background-fixed protected weights \(F_0\), and varying them changes the scalar charge. It also states that nonlinear equivalence to the independent-leaf parent is not established. WS1 P2 finds a linearly protected, flat light scalar profile with per-leaf weighted matter copies and hopping, while explicitly reserving nonlinear mixing, fermions and gauge sectors; P4 concludes the scale-gradient-to-leaf weight ratio is not fixed by the tested symmetries. These facts are consistent with the present obstruction.

## The locked-field multi-leaf calculation

Consider the specific diagnostic action, **not claimed as the unique WS1 parent**, with all participating leaf metrics conformal to one comparison Einstein metric:

\[
S= -\int d^4x\sqrt{-g_E}\left[\frac12 C_2\,g_E^{\mu\nu}(D_\mu\varphi)^*D_\nu\varphi
+\frac12 m^2 C_4 |\varphi|^2+\frac14 C_0 F_{\mu\nu}F_E^{\mu\nu}\right].
\]

For definiteness the complex scalar's conventional kinetic normalization can be adjusted consistently without affecting the proof; the same fixed microscopic mass \(m\) and gauge charge appear on every leaf. The locked scalar and gauge fields are shared, and each leaf's action has a **positive fixed** weight \(w_i\). With \(g_i=A_i^2g_E\) in four ordinary dimensions, determinant and inverse metric powers give

\[
C_0=\sum_iw_i,\qquad C_2=\sum_iw_iA_i^2,\qquad C_4=\sum_iw_iA_i^4.
\]

Four-dimensional Maxwell kinetic energy is conformally invariant, so its leaf coefficient is \(C_0\). Suppose the *entire* expression equals one universally minimally coupled Maxwell–massive-scalar action of the **same microscopic parameters** in a physical metric \(g_J=A_{\mathrm{eff}}^2g_E\), with the overall common constant normalization \(C_0\). Then

\[
C_2=C_0A_{\mathrm{eff}}^2,\qquad C_4=C_0A_{\mathrm{eff}}^4.
\]

Thus the metric-existence condition is

\[
\boxed{\ C_0C_4-C_2^2=\sum_{i<j}w_iw_j(A_i^2-A_j^2)^2=0.\ }
\]

**Proof:** expand both sides, or invoke the equality case of weighted Cauchy–Schwarz. Since the weights are positive, equality forces \(A_i^2=A_j^2\) for every participating pair. This is exact and independent of a numerical regulator, response amplitude or background warp. For non-conformal leaves the generic obstruction is stronger, because distinct tensor contractions cannot generally be represented by a single Lorentzian metric.

**Exact counterexample.** Three leaves with \(w=(1,2,1)\) and \(A_i^2=(1,2,3)\) give \((C_0,C_2,C_4)=(4,8,18)\). The kinetic term and Maxwell term would fix \(A_{\mathrm{eff}}^2=2\), predicting \(C_4=16\), whereas the actual mass coefficient is 18. The mismatch is 12.5% of the single-metric prediction. The moment defect is 8 and the normalized variance is 0.5. These are an **illustrative exact counterexample, not a measured SS signal**.

### What this test does *not* rule out

For a single isolated scalar, one may independently redefine its field and its mass to absorb the mismatch on a constant background, or add nonminimal/counterterm operators. Such choices do **not** demonstrate a universal metric for all charged, massive and massless species with the same fixed microscopic couplings. When the conformal ratios depend on fields, the required redefinitions induce new derivative couplings; to establish universal minimal coupling one must specify the regulator, frame and all parameter matching. If some weights vanish, only the leaves with positive weight participate. If the parent dynamical sector enforces the diagonal metric as a genuine constraint, the obstruction vanishes, but **that enforcement must be derived** rather than presumed.

## Extra scalar charge from dynamic weights

Even with common metric, the parent locked action may look like

\[
S_{m,\mathrm{lock}}=\int d^4x\sqrt{-g_E}\,W(X)\,\mathcal L_m[A^2(X)g_E,\psi].
\]

Taking a localizer variation at fixed Einstein metric and matter variables gives schematically, in the same trace convention as the canonical DYN comparison,

\[
\frac{\delta S_{m,\mathrm{lock}}}{\sqrt{-g_E}\,\delta X^I}
= W\,\alpha_I T_E + (\partial_I W)\mathcal L_{m,E},\qquad \alpha_I=\partial_I\ln A.
\]

The second term is a direct model-dependent coupling; it is not automatically the trace term and is sensitive to the physical matter Lagrangian and boundary terms. It vanishes if \(W\) is fixed along all allowed localizer variations, or can be canceled only by additional justified structure. This matches canonical DYN v8's explicit distinction between its constant \(W_0\) normalization and dynamical \(F(X)\) weighting.

## Dynamical locking is another nontrivial step

Strong hopping can make relative matter modes heavy. But \(\chi_i=\chi\) is not in general an exact solution of each parent matter equation when \(g_i\) differ. For a massive scalar at a constant conformal background, the individual wave equations are schematically \((A_i^{-2}\Box_E-m^2)\chi=0\); subtracting two of them gives \((A_i^{-2}-A_j^{-2})\Box_E\chi=0\), generally incompatible with nontrivial massive solutions. An effective diagonal theory can arise after integrating out heavy modes, but its induced higher-derivative, mass and species-dependent operators must be controlled. Exact universal minimal coupling cannot be asserted solely from a finite-hopping linear protection test.

## Relevance to the atom and clock result

The audited atomic Dirac–Maxwell action correctly follows the **selected** common Jordan metric. The atomic calculation therefore validates the consequences of universal coupling, not a parent derivation of that coupling. For the molecular/biological programme the same distinction applies: a common localizer geometry plus a matter mobility tensor does not itself fix a universally isotropic physical mobility.

The logically necessary routes to full derivation are:

1. Prove a **dynamical diagonal-metric constraint** or uniquely selected effective physical vierbein for all light matter with a positive, constraint-consistent parent completion.
2. Prove that integrating out relative matter and metric modes generates no uncontrolled species-dependent low-energy operators; give matching coefficients and errors on a stated energy domain.
3. Show the protected total matter weight is fixed under allowed localizer variations, or demonstrate why its extra direct source disappears.
4. Show how the selected physical metric transforms under parent-to-DYN reduction; **given the canonical Jordan action**, the last Weyl step then gives \(A=\Phi^{-1/2}\).
5. Derive a cross-sector observable or structural restriction beyond the universal-metric scalar–tensor comparator. A recovered universal metric alone is a consistency bridge, not unique evidence for Scale Space.

## Disposition

**THEORETICAL GATE: CONDITIONAL PASS / GENERIC PARENT DESCENT: NOT ESTABLISHED.** Equal participating metrics + genuinely constrained diagonal matter + fixed common normalization suffice. Generic distinct positive-weight conformal leaf metrics produce a strictly positive moment defect and therefore do not produce exactly the chosen minimal common metric from simple locking. The no-go statement is limited to the specified action and fixed microscopic parameters, not to every possible parent completion.

The results are independently reproducible with `verify_metric_moments.py` (not included) and `verification_results.json` (not included). Canonical files are untouched.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN", "DYN v8" in this note): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.

Other working notes referred to by label:

- P2: [WN-04](WN-04_P2Parent.md)
- P4: [WN-15](WN-15_P4CouplingWeight.md)

Material named in this note but not included in this release: `SS-DYN_leafwise_dynamical_closure_v8.tex`, `WS3_AtomicBridge_v1.md`, `verification_results.json`, `verify_metric_moments.py`.
