> **Public edition of evidence note WN-11.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `SS_ParentMatter_FiniteSpectrum_v1.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `4cb1294b7a17d874f0b046ee8d2f53017df788583a332aa5b7af58f3b92c89bc` (9236 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# Finite-leaf parent: normalized matter-source projection and massive-mode exchange

**Date:** 8 November 2026  
**Status:** Noncanonical research, independent bounded analytic calculation. Not a parent action adoption or a physical particle-physics prediction.  
**Sources:** Read WS1 [WN-05](WN-05_P15ParentClosure.md) and a review note (not included), canonical SS-DYN v8 [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) and the original P20 nonlinear null-sector gate.

## Decision

**Exact finite linear protection:** For the declared finite positive-weight graph model on a *common flat background*, if the source couples to each leaf metric in precisely the same positive weights as the leaf Einstein kinetic terms, it couples to the massless common metric and has zero overlap with every positive generalized-mass metric mode. This result holds for **all connected positive weighted graphs** at the quadratic kinetic level. It does not depend on increasing the link stiffness.

**Controlled violation:** If the matter-source weights depart from the gravitational weights, the mismatch creates positive summed massive-mode overlap equal to a weighted variance. For an explicit three-site graph with gravitational weights (1,2,1), equal links mu, and a centre-leaf matter-source factor 1+epsilon, the only massive coupling is -epsilon to the even relative mode of squared mass 2mu. Integrating out the **abstract scalar graph coefficients** at zero momentum gives epsilon²/(4mu) times the square of the externally factored source amplitude. This is not the physical Dirac–Maxwell spin-2 coefficient: tensor traces, helicity projectors, the gravitational coupling and additional constraint modes have not been determined from a fully specified parent member.

**Result relative to prior Ward gate:** The previously found localizer-induced relative metric response `h_n ∝ p_n ∂_μ∂_ν χ` is pure longitudinal, and its **direct first-order** coupling to a conserved complete on-shell Dirac–Maxwell stress tensor vanishes by the Ward identity (with appropriate boundary/constant-weight assumptions). The new massive-mode spectral source calculation addresses a distinct transverse/traceless or otherwise physical source sector. The Ward cancellation does not imply that the massive eigenmodes are absent, or that generic unprotected matter sources cannot excite them.

## 1. Exactly specified finite quadratic model

Consider N metric fluctuations `h_i` around the *same* Minkowski reference metric, with fixed positive leaf Einstein weights `f_i` and a connected tree or graph of positive linearized Fierz–Pauli link weights. After suppressing the common Lorentz tensor operator for the site-space calculation, define

\[
K=\operatorname{diag}(f_1,\ldots,f_N)>0,\qquad
L=B^T\operatorname{diag}(\mu_e)B\ge0.
\]

Here L is the *linearized site mass matrix*, not a complete nonlinear multigravity action. The generalized metric eigenproblem is

\[
Lv_a=m_a^2Kv_a,\quad v_a^T K v_b=\delta_{ab}.
\]

For a connected graph, the unique massless vector is

\[
v_0={\mathbf 1\over\sqrt{F}},\qquad F=\sum_i f_i,\qquad m_0^2=0.
\]

A total conserved matter stress `T_{μν}` coupled identically on each leaf with the protected weights has site current `j_i=f_i T_{μν}`. Its normalized metric-mode coupling is

\[
g_a=v_a^T j/T=v_a^T f.
\]

By generalized orthogonality `v_a^T K v_0=0` for `a>0`, one gets the **exact protection identity**

\[
\boxed{g_0=\sqrt F,\qquad g_a=0\quad(a>0).}
\]

This is a genuine finite-dimensional source-overlap theorem. It is a consistency test of the weighted quadratic graph and the chosen leaf matter weights; it **does not derive those weights** from a more fundamental symmetry.

### General source mismatch

Let `j_i=f_i(1+ε_i)T`. Removing its massless projection gives

\[
j_{\perp,i}=f_i(\epsilon_i-\bar\epsilon)T,
\qquad\bar\epsilon={\sum_i f_i\epsilon_i\over F}.
\]

The sum of squared, **canonically normalized** couplings to all massive modes is

\[
\boxed{\sum_{a>0}(v_a^Tj/T)^2
=\sum_i f_i(\epsilon_i-\bar\epsilon)^2.}
\]

The right-hand side is a weighted variance. It is zero if and only if every active positive-weight leaf has the same relative perturbation `ε_i`. A shared overall rescaling therefore changes the common-mode normalization but does not excite a massive relative mode at this order. A spatially/leaf-dependent perturbation generally does.

If all massive squared masses are at least `m_gap²>0`, the static site-contact amplitude satisfies

\[
0\le {1\over2}\sum_{a>0}{(v_a^Tj/T)^2\over m_a^2}
\le {\sum_i f_i(\epsilon_i-\bar\epsilon)^2\over 2m_{\rm gap}^2}.
\]

This is a *site-mode coefficient bound*, not a bound for the full relativistic scattering amplitude.

## 2. Concrete three-site spectrum and matching

Set

\[
K=\begin{pmatrix}1&0&0\\0&2&0\\0&0&1\end{pmatrix},\qquad
L=\mu\begin{pmatrix}1&-1&0\\-1&2&-1\\0&-1&1\end{pmatrix},\quad\mu>0.
\]

A complete K-orthonormal generalized eigenbasis is

\[
\begin{array}{c|c|c}
\text{mode}&v_a&m_a^2\\\hline
\text{common}&(1,1,1)^T/2&0\\
\text{odd relative}&(1,0,-1)^T/\sqrt2&\mu\\
\text{even relative}&(1,-1,1)^T/2&2\mu
\end{array}
\]

The protected current `j=(1,2,1)T` projects as `(2,0,0)T`: no massive-mode coupling.

A centre-leaf source perturbation

\[
j=(1,2(1+\epsilon),1)T
\]

projects as

\[
\boxed{(g_0,g_{\rm odd},g_{\rm even})=(2+\epsilon,0,-\epsilon).}
\]

At zero momentum, the massive-mode site contact coefficient becomes

\[
\boxed{\mathcal C_{\perp}={1\over2}{\epsilon^2\over 2\mu}={\epsilon^2\over4\mu}.}
\]

The same expression follows using the Euclidean graph pseudoinverse acting on the zero-sum source `j_⊥=(-ε/2,ε,-ε/2)T`. The coefficient varies continuously and tends to zero as μ tends to infinity, or as the source is restored to the protected weight pattern.

### Field-theory limitation

The actual quadratic Fierz–Pauli propagator has Lorentz-index projectors and a helicity-0 component. The exchange of conserved stresses typically involves different `T_{μν}T'^{μν}` and trace terms for massive versus massless spin-2 exchange. Recovering those factors requires the exact parent lapse/shift constraints, the complete quadratic action, the matter/Planck normalization and the chosen backgrounds. This audit does **not** call epsilon²/(4mu) a predicted physical fifth-force strength, nor extend it to a bound on nonconserved stress or a generic dynamical localizer.

## 3. Relation to WS1 P15 and the atomic bridge from a separate AI-assisted session

P15 reports, at tree level for its **static-localizer, equal-metric, F-weighted** candidate, a protected constant matter mode. This note confirms the **metric-source analogue** of that result with an exact finite site-spectrum calculation. Neither implies that localizer-induced relative metric perturbations disappear, or that the same protection remains radiatively stable.

P15 also reports one-loop generation of non-F-proportional leaf matter weights and strong coupling near the edge of its regulator box; the present investigation **did not independently rerun** P15's loop or constrained Hamiltonian calculations. If such unequal counterterm weights persist after a valid quantum completion, the weighted-variance theorem shows precisely how they can create massive-mode source overlaps. The size and even physical validity of a naive one-loop estimate require a trustworthy EFT regime and renormalization matching; the prior numerical box-edge estimates should not be used as precision predictions.

That session's atomic bridge, by contrast, uses a single **chosen** physical Jordan metric for the electron–proton–Maxwell system. It passes its bounded microscopic action checks, but this finite graph calculation still does **not** derive the Jordan metric from the independent-leaf parent. It supplies a sharp matching condition to be checked in such a derivation.

## 4. Acceptance and next gate

- **PASS:** explicit finite graph, K-normalized mass spectrum and source overlaps; exact protected-mode theorem, weighted-variance mismatch identity, and graph-site contact coefficient.
- **HOLD:** canonical parent-derived universal Dirac–Maxwell metric, physically normalized massive spin-2 exchange, full localizer-dependent metric/matter dynamics, inhomogeneous constraint closure and radiative protection.
- **NEXT:** select a **fully specified** finite member with actual values `f_n=w_nF_n`, actual dRGT-type link tensor structure and a physically constrained Dirac–Maxwell matter action. Derive physical tensor projectors and trace coupling and identify a consistent renormalized source prescription, starting in the weakly coupled core. Compare the resulting amplitude with the present graph overlap as a strict source-selection gate.

## Provenance and file integrity

Read WS1 [WN-05](WN-05_P15ParentClosure.md), a review note (not included), WS1 [WN-04](WN-04_P2Parent.md), canonical SS-DYN v8, and the historical `P20_NS_gate_v1.tex` (not included). The P20 source gives the linearized graph notation and the pure-longitudinal source constraint; the finite three-leaf numerical weights are a **new illustrative selection**, not a reconstructed unique adopted parent member. Exact calculations and manifest were bundled with this report (not included in this release). No original papers were modified.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8**: D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.

Other working notes referred to by label:

- P15: [WN-05](WN-05_P15ParentClosure.md)
- P20: the retired Paper 20 series and its unpublished gate documents (see References).

Material named in this note but not included in this release: `P20_NS_gate_v1.tex`.
