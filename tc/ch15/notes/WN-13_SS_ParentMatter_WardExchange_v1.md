> **Public edition of evidence note WN-13.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `SS_ParentMatter_WardExchange_v1.md`. Not peer reviewed.
> - **Source content hash:** `20781d62efc0f37673d9fbb978f986d1402e7139f787ca51620b15fe424c8355` (8416 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

---
title: Parent-to-DYN matter source Ward and relative-mode exchange gate
status: additive noncanonical working result
created_utc: 2026-11-08
authoritative_for: none
scope: SS-STRATEGY / independent parent matter coupling
---

# Relative-metric response does not automatically imply a matter force

## Decision

**Conditional analytic PASS** for the leading conserved-source Ward cancellation, including the actual P20_NS linear source equation. **Nonlinear parent universality remains OPEN**. The important correction to the prior relative-metric obstruction is that a nonzero pure-longitudinal leafwise response does **not** automatically give a physical coupling to an on-shell conserved Dirac–Maxwell source. The leading direct source vanishes after integration by parts, even though adjacent leaf metrics differ.

The separate **massive transverse exchange** of a genuinely unprotected matter current is generically nonzero and generates an effective quadratic current interaction of size `source²/link stiffness` in a specified low-momentum graph example. The formula is a controlled graph/Tensor-sector proxy, **not** the complete all-helicity nonlinear dRGT effective action.

### Sources and scope

* Canonical `SS-DYN_leafwise_dynamical_closure_v8.tex` (LaTeX source of SS-DYN v8; not included): common-metric finite family is declared; no nonlinear equivalence to independent-leaf parent claimed.
* Original parent linear-constraint derivation, `P20_NS_gate_v1.tex` (not included) (retained historical support, not canonical), with `c_u² L_g p = 2s`, `h_nμν=p_n∂μ∂νχ`, and `s_n=w_n f_n v_n`, `sum s=0`.
* WS1 [WN-04](WN-04_P2Parent.md) (draft): per-leaf scalar field copies and weighted hopping protect a linear light mode in selected tests.
* WS1 [WN-05](WN-05_P15ParentClosure.md) (draft, read live 8 Nov 2026): claims tree-level matter-copy protection in an equal-metric background and serious radiative/strong-coupling problems in the discretized parent. Its numerical and one-loop estimates were **not independently rerun in this gate**.

## 1. Exact leading source Ward cancellation

On the common flat four-dimensional background let `h_n^{μν} = p_n ∂^μ∂^ν χ` be the **relative** metric response from the P20 parent constraint. The first variation of the complete minimally coupled Dirac–Maxwell matter action is, up to the convention for metric variation,

\[
\delta S_m=\frac12\sum_n w_n\int d^4x\,T_n^{\mu\nu}\,h_{n\mu\nu}.
\]

At a fixed localizer background and fixed `p_n,w_n`, a single **locked** on-shell matter configuration with a common conserved stress `∂_μT^{μν}=0` and constant leaf normalizations has `T_n^{μν}=c_n T^{μν}`. Thus

\[
\delta S_m=\frac12\int d^4x\,(\sum_n w_nc_np_n)\,T^{\mu\nu}\partial_\mu\partial_\nu\chi
=\frac12\int d^4x\,\chi(\sum_nw_nc_np_n)\,\partial_\mu\partial_\nu T^{\mu\nu}=0
\]

on fields with boundary terms controlled. It follows because `k_μ T^{μν}=0` implies `k_μk_νT^{μν}=0`. The total stress **must** include electron, proton, Maxwell fields and interactions. Free constituent stress tensors are not separately conserved in interacting QED; discarding the electromagnetic exchange destroys this Ward cancellation.

**Crucial distinction:** the metric perturbation is nonzero and relative, but is pure-longitudinal *at this linear constrained order*. The absence of a direct conserved-source vertex is a statement about the tested vertex, **not** vanishing of all metric corrections or a generally covariant identification of the leaves. Finite-momentum external sources with boundaries, off-shell matter, dynamical localizer weights and higher-order non-longitudinal metric responses can evade the cancellation.

### Moving weights

If `a_n(x)=w_n(x)c_n(x)p_n(x)` varies, integration by parts gives

\[
\int a_nT^{\mu\nu}\partial_\mu\partial_\nu\chi
=-\int\partial_\mu(a_nT^{\mu\nu})\partial_\nu\chi+\mathrm{boundary}
=-\int(\partial_\mu a_n)T^{\mu\nu}\partial_\nu\chi+\mathrm{boundary}
\]

for a common conserved `T`. Therefore a moving localizer may reintroduce precisely the terms whose coefficients are derivatives of the protected weights/response. This is **not** computed for a dynamical localizer in the present gate.

## 2. P20 relative response remains real

For an unweighted three-leaf chain with positive edge strength `μ`, use

\[
B=\begin{pmatrix}-1&1&0\\0&-1&1\end{pmatrix},\quad
L_g=\mu B^TB,\quad s=z(1,-2,1)^T.
\]

The unique zero-mean constrained solution is

\[
 p=\frac{2z}{3c_u^2\mu}(1,-2,1)^T,\quad
 Bp=\frac{2z}{c_u^2\mu}(-1,1)^T,
\]

and its positive weighted graph energy is

\[
\mu\|Bp\|^2=\frac{8z^2}{c_u^4\mu}.
\]

Both the nonzero relative response and the conserved-stress Ward cancellation therefore hold at the **same order**. Do not use the existence of `Bp≠0` alone to assert a new long-range atomic gravitational force.

## 3. Massive-mode current exchange for an unprotected source

For the **transverse/tensor graph block only**, after fixing the common zero mode, the low-energy static quadratic model is

\[
L_{\rm massive}= -\tfrac12 h_\perp^T L_g h_\perp +j_\perp^T h_\perp,\qquad
\mathbf1^Tj_\perp=0.
\]

Eliminating the massive variable gives

\[
\Delta L_{\rm eff}=\frac12j_\perp^T L_g^+ j_\perp.
\]

The overall Lorentzian tensor sign, trace-projector factors, graviton normalization, and derivative corrections **are not fixed by this scalar graph proxy**. It establishes the source-projector structure and mass/stiffness scaling only. In the three-leaf symmetric example `j_⊥=ε(1,-2,1)` one obtains

\[
\boxed{\tfrac12j_\perp^TL_g^+j_\perp=\frac{\epsilon^2}{\mu}.}
\]

An aligned common source `j∝(1,1,1)` projects to zero. For the unequal-background parent one must instead use the common graviton mode defined by the *actual* positive kinetic weights `F_n w_n` and the full massive spin-2 operator. The toy uniform projector is **not** substituted for this physical projector.

### Conditions for an exact absence of this contact

1. In the relevant background and field basis, the full conserved matter source has no projection onto massive metric eigenmodes.
2. Relative metric modes are eliminated by actual first-/second-class constraints, not merely by taking a large but finite mass; **or** their sources vanish by a genuine selection rule.
3. The locked light matter configuration solves the complete matter equations including localizer gradients and boundary conditions.
4. The weighted matter prefactor is protected, and radiative matching does not regenerate direct localizer or species-dependent couplings.

These are **additional obligations**, not proved properties of the currently described independent-leaf parent. In particular P15's one-loop note questions item 4, although its calculation is not rerun here.

## 4. Decision and next task

- **PASS:** Exact leading direct coupling to a fully conserved on-shell Dirac–Maxwell source vanishes for the pure-longitudinal relative metric at fixed background.
- **PASS (finite graph diagnostic):** Relative metric field and relative massive-mode exchange need not vanish; a nonaligned matter source generates a quadratic effective interaction proportional to `1/μ`.
- **HOLD:** A physical finite-member coefficient for electron/proton/Maxwell nonuniversality; must use actual weighted tensor projector, full dRGT helicities, localizer dependence, boundary conditions and source normalization.
- **HOLD:** Universality at quantum level; WS1 P15 reports nonprotected counterterms and strong coupling, which remain independently unverified here.

**Next substantive independent gate:** an actual member-specific low-energy operator calculation using fully specified finite leaf weights, the proper common/massive graviton eigenbasis, tensor propagators and a controlled conserved composite source. Only that calculation could yield a meaningful coefficient rather than a graph proxy. WS1's ghost/loop analysis and the wall–charge investigation developed in a separate AI-assisted session are outside this note.

## Verification

`verify_ward_exchange.py` (not included) performs a fresh SymPy check of the constraint, edge response, graph norm, Moore–Penrose Green operator, common-mode annihilation, relative-current contact and conserved stress contraction. No original WS1 verifier is imported. `verification.json` (not included) and `SHA256SUMS` (not included) record replay and file integrity. This is analytic/local-linear reproducibility, not a numerical parent solution.

---

## References and related notes (public edition)

Other working notes referred to by label:

- P15: [WN-05](WN-05_P15ParentClosure.md)
- P20: the retired Paper 20 series and its unpublished gate documents (see References).

Material named in this note but not included in this release: `P20_NS_gate_v1.tex`, `SHA256SUMS`, `SS-DYN_leafwise_dynamical_closure_v8.tex`, `verification.json`, `verify_ward_exchange.py`.
