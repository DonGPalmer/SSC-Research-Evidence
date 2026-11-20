> **Public edition of evidence note WN-06.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `SS_ParentMatter_Final_Decision_v1.md`. Not peer reviewed.
> - **Source content hash:** `e68bbe76e128e9be75eddff36e95c957cf8c4b15de00c7ed9f6e0fc86a5c31bb` (9981 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# SS parent-to-DYN universal matter: decision gate

**Date:** 2026-11-08  
**Status:** Independent, noncanonical, read-only technical synthesis plus separately verified restricted calculations. **No parent-to-DYN derivation achieved.**  
**Boundaries:** This note does not modify canonical SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). The finite example below is a controlled Fierz–Pauli quadratic *test member*, not an independently validated full nonlinear SS parent.

## Executive decision

**HOLD P2 as a proposed microscopic parent; ACCEPT only its restricted tree-level effective common-metric behavior, conditional on protected fixed weights and compatible backgrounds.** Do not promote P2's per-leaf construction into the canonical explanation of the atomic matter metric. The next work should be a *single* gate on regulator-compatible quantum matching and its constraint implementation, not an indefinite series of further interaction proposals. If no symmetry/action-derived Ward protection is supplied, close P2 as an illustrative low-energy parent rather than a derivation.

The current SS-DYN common-metric finite family retains its established status independent of P2. The atomic Dirac–Maxwell bridge remains internally consistent, but its universal matter metric is still specified by the common-metric action.

## 1. Source documents and authority

Reviewed working files: canonical `SS-DYN_leafwise_dynamical_closure_v8.tex` (LaTeX source of SS-DYN v8; not included); historical parent quadratic gate `P20_NS_gate_v1.tex` (not included); current unreviewed WS1 documents [WN-04](WN-04_P2Parent.md), [WN-05](WN-05_P15ParentClosure.md), a review note (not included), `P17CoreBoxOneLoop.md` (not included) and `P17ReviewBrief.md` (not included); previous independent noncanonical universality, Dirac-matching, constraint and Ward-exchange notes. Latest WS1 P17 is explicitly an unreviewed toy-model calculation; its reported radiative numbers are **not** independently reproduced here. The canonical DYN paper expressly separates the common-metric family from the independent-leaf parent and does not assert their nonlinear equivalence.

## 2. The complete leading conserved-source exchange in one fixed three-leaf test

Choose the positive leaf kinetic weights and Fierz–Pauli link mass matrix

\[
K=\operatorname{diag}(1,2,1),\quad
L=\mu\begin{pmatrix}1&-1&0\\-1&2&-1\\0&-1&1\end{pmatrix},\quad \mu>0.
\]

The K-orthonormal generalized eigenvectors and mass squares are

\[
v_0=\tfrac12(1,1,1),\quad m_0^2=0;\qquad
v_o=2^{-1/2}(1,0,-1),\quad m_o^2=\mu;\qquad
v_e=\tfrac12(1,-1,1),\quad m_e^2=2\mu.
\]

With canonically normalized quadratic tensor modes, assume a universal conserved symmetric stress tensor and linear matter sources `j_n T^{\mu\nu}h_{n\mu\nu}`. The protected leaf source is `j=K 1=(1,2,1)`, which gives `(g_0,g_o,g_e)=V^Tj=(2,0,0)`. For a fractional change in the central weight, `j=(1,2(1+epsilon),1)`, the couplings become `(2+epsilon,0,-epsilon)`.

For each *healthy* massive Fierz–Pauli mode and conserved external stress tensors at nonzero Fourier momentum, the linear exchange has the universal tensor structure

\[
\mathcal A_{a}(q)\propto\frac{g_ag_a'}{q^2+m_a^2}
\left(T_{\mu\nu}T'^{\mu\nu}-\tfrac13 TT'\right),\quad m_a>0.
\]

The massless mode instead has the `-1/2 TT'` coefficient. This difference is the standard linear vDVZ tensor-structure distinction, not new SS phenomenology. The precise overall factor, metric signature and the handling of scalar graviton/localizer mixing depend on the selected parent action and its full constraints; those were **not** separately solved in this test.

For two identical static nonrelativistic sources with the above same leaf weights, relative to their massless exchange the positive massive-even Yukawa strength is

\[
\boxed{\alpha_e=\frac43\left(\frac{\epsilon}{2+\epsilon}\right)^2}
\]

with Yukawa factor `exp(-sqrt(2mu) r)` in units where the mass-squared matrix above has standard canonical dimensions. The protected case epsilon=0 is exactly zero, at arbitrary finite positive mu, in this linearized quadratic model. In the zero-momentum site-only effective action, the corresponding even-mode contact is `epsilon^2/(4mu)` with the selected `1/2` convention. It is **not** a final Newtonian prediction: DYN scale normalization, actual finite regulator, the Q/localizer sector, 4D Planck factor, constraints and universal composition data are not supplied by this three-site test.

### Important boundary of the earlier Ward result

The previous pure-longitudinal linear response `h_n = p_n partial_mu partial_nu chi` contracts to zero with a conserved closed-system stress tensor after integration by parts. That does **not** remove transverse massive-spin-2 exchange when a real nonzero relative source exists. The two cancellations apply to different source/field sectors; one is not a proof of the other.

## 3. WS1 P17: one-loop all-mode versus Wilsonian threshold

P17 reports that with per-leaf `phi^4` and identical 4D cutoff on every leaf, a quadratic counterterm has the form `c_n proportional to K_n sum_a u_a(n)^2` where eigenprofiles are K-orthonormal. **When all N modes are included with equal divergent loop coefficient**, the completeness identity gives

\[
K_n\sum_{a=0}^{N-1}u_a(n)^2=1.
\]

Thus its uniform *full-tower leading quadratic* coefficient is algebraically correct for that declared regulator. However, a Wilsonian loop calculation at cutoff Lambda **below the first heavy copy gap** must not sum modes with masses above Lambda as if they had the same `Lambda^2` loop integral. With only the normalized constant light mode, `u_0(n)=1/sqrt(W), W=sum K_n`, the included site coefficient is instead

\[
\boxed{c_n^{\rm light}\propto K_n/W},
\]

which is exactly protected in the quadratic example. Our three-leaf case gives `(1/4,1/2,1/4)` for the low-mode contribution versus `(1,1,1)` for the degenerate-coefficient full-tower completeness limit.

For general Wilsonian matching, the right expression is

\[
c_n(\Lambda)\propto K_n\sum_a u_a(n)^2\,I(\Lambda,m_a),
\]

where `I` is the chosen cutoff-dependent loop integral and thresholds/counterterms must be treated consistently. Heavy modes can still generate nonuniversal *finite threshold corrections*, and an external symmetry might be needed to forbid them. Dimensional regulator, renormalization prescriptions and material fields change details. Consequently:

- **Supported**: Under a common hard cutoff applied to the entire discrete tower, equal loop integrals generate a uniform leaf-local leading term, not one proportional to the site gravitational weights; absent a protection principle this reveals a genuine naturalness concern.
- **Not established by that formula alone**: that the physical EFT below the first heavy-mode gap necessarily suffers the same full-tower divergence, that an unbounded `1/sqrt(Delta y)` physical cutoff restriction holds under a properly matched continuum regulator, or that all fermion/gauge loop renormalizations fail analogously.
- **Also not established**: quantum protection. Threshold matching, divergent/local counterterm structure, the physical ultraviolet cutoff and any UV symmetry are not derived from the present parent.

WS1's `P15` also finds a compatible homogeneous 3-site constraint chain only in minisuperspace, and does not establish inhomogeneous nonlinear closure with shifts. The numerical P17 conclusions remain unreviewed as an independent full script reproduction. This decision does not relabel those results as proven nonlinear no-go statements.

## 4. Unambiguous programme decision

| Gate | Disposition | Meaning |
|---|---|---|
| Universal light coupling for exactly protected source | **PASS, restricted** | Exact massless-only overlap in a normalized finite quadratic tensor model; pure-longitudinal Ward cancellation for conserved closed-system matter. |
| Physical relative massive exchange if source weights differ | **PASS, restricted** | Fierz–Pauli trace projector and positive quadratic massive-mode coupling, with declared graph normalization. |
| Exact finite-parent metric universality | **HOLD** | Leaf metrics can differ in active localizer sectors, and equal-metric consistent truncation is not proved across general backgrounds. |
| Quantum stability of the protected weights | **HOLD** | Full-tower loop concern is real within its regulator, but the Wilsonian threshold and full standard-model matching are open. |
| Full nonlinear constraint closure | **HOLD** | Homogeneous minisuperspace analysis does not replace field-theoretic shift/secondary checks. |
| SS-distinctive gravity prediction | **NOT ESTABLISHED** | The massive-spin-2 exchange structure is conventional. |

**Stop rule:** Do not invest in another broad P2 parameter search or append a new ad hoc matter interaction. A new P2 development is justified only if it resolves one of two independently predeclared gates: (A) identify a concrete symmetry or regulator and calculate matching across heavy-copy thresholds preserving protected source weights without leaf-by-leaf tuning, or (B) derive a fully constrained nonlinear map to one Jordan metric for physical matter on nontrivial localizer backgrounds. Otherwise the per-leaf parent remains illustrative, while canonical SS-DYN's chosen common metric and the atomic completion developed in a separate AI-assisted session remain valid restricted definitions, not consequences derived from the parent.

## 5. Provenance and reproduction

The accompanying `verify_decision.py` (not included) independently checks K-orthogonal eigenvectors, squared masses, protected and perturbed source overlaps, the static spin-2 relative Yukawa strength, the graph contact, the full-mode completeness coefficient, and the one-light-mode Wilsonian coefficient. Verification requires SymPy. The results are in `verification_results.json` (not included); all file hashes in `SHA256SUMS` (not included). No copying of full published data. The original working documents were read only; no original source code was edited.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.

Other working notes referred to by label:

- P2: [WN-04](WN-04_P2Parent.md)
- P17: not included in this release.

Material named in this note but not included in this release: `P17CoreBoxOneLoop.md`, `P17ReviewBrief.md`, `P20_NS_gate_v1.tex`, `SHA256SUMS`, `SS-DYN_leafwise_dynamical_closure_v8.tex`, `verification_results.json`, `verify_decision.py`.
