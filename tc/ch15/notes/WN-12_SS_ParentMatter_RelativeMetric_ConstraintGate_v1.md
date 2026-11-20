> **Public edition of evidence note WN-12.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `SS_ParentMatter_RelativeMetric_ConstraintGate_v1.md`, a working note dated 8 November 2026. Not peer reviewed.
> - **Source content hash:** `e1a5a5fe215183f05758c7e3bab9a0b0b0b0a1dd6a2ab7041c4e461a0f89bd32` (12171 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** Its relative-metric obstruction is qualified in [WN-13](WN-13_SS_ParentMatter_WardExchange_v1.md), which finds that a nonzero relative response does not by itself give a matter force. An editorial note marks the affected passage; the original wording is kept.

# Parent-to-DYN universal matter coupling: actual graph-constraint gate

**8 November 2026 | Noncanonical mathematical result | Independent complement to WS1 P2/P14 and WS3 AtomicBridge**

## Decision

> **Editorial note (public edition, 19 November 2026):** A later note finds that the nonzero relative metric response Bp derived here does not by itself give a matter force: its leading direct coupling to a fully conserved on-shell Dirac–Maxwell source cancels by the Ward identity, although the relative response is real and massive-mode exchange of an unprotected current is generically nonzero. See [WN-13](WN-13_SS_ParentMatter_WardExchange_v1.md) Decision and §2. The text below is unchanged from the working note.

**FAIL for automatic diagonal reduction under unrestricted orthogonal localizer perturbations of the declared finite-leaf linearized parent.** The existing parent gravitational constraint itself sources nonidentical leaf metrics for nonzero graph-orthogonal localizer source. A diagonal/common metric is a valid *algebraic subspace*, but the source equation does not keep an arbitrary localizer perturbation on that subspace. A genuine localizer projection/constraint, or a controlled finite-gap EFT matching calculation, remains necessary for the universal metric of canonical SS-DYN v8 [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) to be inherited rather than separately specified.

**This is a restricted result:** the parent linearization is sourced from P20_NS_gate_v1 and reviewed in WS1 P14, not newly derived from a full nonlinear dRGT/ghost-free Hamiltonian. It is not a no-go theorem against all Scale Space parent completions; in particular, the strongly coupled null sector may need redesign or removal. No new gravitational prediction is inferred.

## Sources

Sources:

1. `P20_NS_gate_v1.tex` (not included), 18 August 2026. Its finite-chain quadratic action explicitly contains leaf Einstein terms weighted by `w_n F_n`, localizer–Ricci mixing `w_n f_n ξ_n R_n^(1)`, and Fierz–Pauli edge weights `μ_e`. Its derived graph constraint is **`c_u² L_g p = 2s`**, with `s_n = w_n f_n v_n`, `∑s_n=0`, `L_g=Bᵀdiag(μ_e)B`, and `h_(n,μν)=p_n ∂_μ∂_ν χ`.
2. Canonical `SS-DYN_leafwise_dynamical_closure_v8.tex` (LaTeX source of SS-DYN v8; not included) (v8.0.0). This separately defines finite **common-metric** `D_{N,L}` with `S_m[g_J,ψ]`, `g_J=A²g_E`, `A=Φ^(-1/2)`. The independent-leaf parent and fully nonlinear common-metric uplift are not claimed equivalent; its protected parent weights are fixed at the background.
3. [WN-04](WN-04_P2Parent.md) (draft) gives a 3-site protected scalar zero mode for per-leaf **independent matter copies** with hopping; it explicitly acknowledges the scalar-only, 3-site, linear scope and incomplete constraint algebra.
4. `P14CommonMode.md` (not included) (draft, 20:37 UTC today) already records the graph invariant `K=sᵀ L_g⁺ s`, and studies graviton–localizer cubic vertices. The present note does **not** claim to discover that invariant; it tests what that same equation implies for *universal matter metric inheritance*.
5. The previously filed [WN-10](WN-10_SS_ParentMatter_Universality_Gate_v1.md) and [WN-09](WN-09_SS_ParentMatter_DiracMatching_v1.md) (noncanonical): fixed-positive-weight metric moment tests. These were restricted conformal comparators, not the full parent’s actual longitudinal relative response.

## 1. Exact consequence of the declared *linearized* parent constraint

Let `B` be an oriented incidence matrix for a **connected** graph of N leaves with edge coefficients `μ_e>0`, and define

\[
L_g=B^T\operatorname{diag}(\mu_e)B,\qquad
s_n=w_nf_nv_n,\quad \boldsymbol1^Ts=0.
\]

P20_NS_gate gives the constrained metric response

\[
c_u^2L_gp=2s,\qquad
h_{n\mu\nu}=p_n\partial_\mu\partial_\nu\chi.
\]

The graph Laplacian has kernel `span{1}`. Therefore a *single* metric perturbation for all leaves requires `Bp=0`, hence `p=constant` and `s=0`. Conversely, for any `s≠0` in the zero-sum subspace, the solution with zero common-mode average has

\[
p=\frac{2}{c_u^2}L_g^+s,\qquad Bp\neq0.
\]

The graph energy is a **strictly positive** indicator of a relative metric response:

\[
\boxed{\mathcal E_{\rm rel}=p^TL_gp=\frac4{c_u^4}s^TL_g^+s>0\quad(s\neq0).}
\]

The physical tensor difference along edge `e` is `(Bp)_e ∂_μ∂_ν χ`; it is nonzero where `χ` has a nonzero relevant Hessian. Although each individual pure-longitudinal perturbation has vanishing linearized curvature, differences among leaves cannot all be removed by the **single remaining diagonal diffeomorphism** once links couple the metrics. The expression is a constrained relative response, not by itself a healthy propagating relative degree of freedom.

**Important:** the source is the *localizer perturbation*, not a freely added matter force. The fact that a common light matter profile has protected linear tensor sourcing does not set `s_n=0` for every localizer profile.

## 2. Exact three-site finite-stiffness counterexample

Take the 1–2–3 chain, identical positive link strength `μ`, and an admissible zero-sum normalized-direction shape `s=z(1,-2,1)` for scalar excitation amplitude `z`:

\[
B=\begin{pmatrix}-1&1&0\\0&-1&1\end{pmatrix},\quad
L_g=\mu\begin{pmatrix}1&-1&0\\-1&2&-1\\0&-1&1\end{pmatrix}.
\]

The zero-average unique solution is

\[
\boxed{p=\frac{z}{3c_u^2\mu}(2,-4,2),\qquad Bp=\frac{2z}{c_u^2\mu}(-1,+1).}
\]

The resulting graph energy is

\[
\boxed{\mathcal E_{\rm rel}=\frac{8z^2}{c_u^4\mu}.}
\]

It is **not zero for finite μ and nonzero z**. When all link weights scale together as `μ→Λμ`, the relative response is `O(Λ⁻¹)` and the graph energy is `O(Λ⁻¹)`. A formal infinite-stiffness limit is thus compatible with an *approximate* common metric at this order, but this limit does not establish a UV-consistent strongly coupled parent or eliminate unrestricted relative initial data.

This example illustrates a permitted source pattern of the general graph equation; it is **not** a claim that this exact 3-site profile and normalization match a selected numerical kink regulator without checking its `w_n,f_n` and parity constraints.

## 3. Can the diagonal sector nevertheless be exact?

Yes, **conditionally**. Consider a parent with site actions

\[
S=\sum_i c_i\{S_{\rm EH}[g_i]+S_{\rm DM}[g_i,\psi_i]\}
+S_{\rm edge}[g_i]+S_{\rm hop}[g_i,\psi_i]+S_X.
\]

If (a) `c_i` is a positive fixed coefficient multiplying **the entire** site gravity-plus-matter action; (b) the full edge potential has no relative *first variation* at `g_i=g` (or its variations are proportionate to `c_i` and can be absorbed into a common equation); (c) hopping has zero first variation when `ψ_i=ψ`; and (d) localizer equations and stress terms reduce to the **same normalized site equation**, then the common field configuration `g_i=g`, `ψ_i=ψ` is a consistent classical truncation of the parent field equations. This follows by dividing each site's Euler–Lagrange equation by `c_i`.

**These are sufficient conditions, not established properties of the current parent.** In the P20 linearized parent, active orthogonal `ξ_n` violates condition (d) precisely through the nonuniform localizer–Ricci source `w_n f_n v_n`. The graph-constraint theorem proves it cannot remain strictly diagonal for all such excitations. Moreover, a rank test on lapse variables at sampled finite sites is not a full nonlinear secondary/tertiary constraint proof for these additional matter fields.

An exactly diagonal **selected sector** is therefore different from a dynamical theorem that **all low-energy solutions flow to it**. Massive relative modes can remain excited by initial data even when matter's light mode is protected and the diagonal sector is consistent in a restricted solution class.

## 4. Matter consequences and the previous metric-moment gate

The earlier Dirac–Maxwell matching gate establishes that a **fixed-positive-weight, simply locked** collection of conformally related leaf metrics with factors `A_i` has coefficient moments

\[
C_0=\sum_iw_i,\quad C_3=\sum_iw_iA_i^3,\quad C_4=\sum_iw_iA_i^4,
\]

and exact single-conformal-metric matching with unchanged microscopic parameters requires `C_3^4=C_0 C_4^3`. Weighted Hölder gives `C_3^4≤C_0 C_4^3` with equality for equal participating factors. A symmetric two-leaf deformation `A_±=1±ε` produces relative coefficient mismatch `2ε²+O(ε⁴)` after choosing the metric using the Dirac kinetic term. This is a **separate conformal diagnostic**; the actual parent response above is `h_n=p_n∂∂χ`, generally nonconformal, and this `2ε²` coefficient must **not** be assigned to it without a full vierbein calculation.

The reproducibility verifier includes an additional fixed-normalization Maxwell diagnostic in a static rank-one spatial deformation `g_{xx}^{±}=1±q`; its normalized coefficient product is `1+q²/4+3q⁴/16+...`. This illustrates distinct nonlinear optical normalization once unequal metrics are simply averaged. It is not a birefringence or phenomenological prediction.

## 5. Constraints needed for the *actual* parent-to-DYN physical claim

| Gate | What would establish it | Disposition |
|---|---|---|
| G1 | Protected linear matter profile with fixed background leaf weights | WS1 P2's restricted scalar test supports it |
| G2 | A **first-class/second-class constraint or exact symmetry** setting `s=0` for all *physical* relative sources, or otherwise eliminating `Bp` | **OPEN** — P20 gate explicitly gives nonzero `Bp` for orthogonal sources |
| G3 | Full nonlinear, ghost-consistent edge interaction and common-metric invariant submanifold including localizer | **OPEN**; quadratic FP and sampled lapse rank insufficient |
| G4 | Controlled heavy relative metric/matter mode elimination with operator remainders and energy domain | **OPEN**; formal stiffness limit insufficient |
| G5 | Dirac–Maxwell low-energy effective vierbein, charge/kinetic/mass normalization, and gauge constraints | **OPEN**; previous conformal moment obstruction remains relevant |
| G6 | Exact identification of emergent `g_J` and `Φ` with canonical DYN v8 in one frame | **OPEN**; `A=Φ^-1/2` is specified in canonical DYN but not established from parent |

## 6. Scientific decision and next gate

**Bounded decision:** For the specific active orthogonal localizer channel of the retained parent linearization, common leaf metrics are not automatically enforced at finite interleaf stiffness. The graph forcing result is exact within the declared linearized equations. This refines the prior general statement “fields locked, then metrics perhaps equal” into an explicit obstruction derived from the actual parent source.

**Not decided:** Whether an improved constrained parent can remove those modes and yield universal matter exactly; whether a finite-gap low-energy EFT makes the unwanted corrections experimentally negligible; whether nontrivial relative eigenmodes survive quantum and stability tests; and whether the current parent can be completed consistently beyond the gate's known null-sector cutoff limitations.

**Next research target:** Construct the Dirac–Maxwell **low-energy effective operator matching on one fixed, fully specified finite parent member**, allowing for the actual longitudinal metric perturbations and all physical field normalizations. In particular, do not impose `g_i=g` at the outset; compute the first nonredundant `T_rel L_g^+ T_rel` term and decide whether protected species produce it at quadratic order. A proof of zero would be a genuine new universality result; a nonzero coefficient would quantify the EFT correction. A complete metric-vierbein and nonlinear ghost analysis is still necessary for a physical statement.

## Verification

`verify_parent_constraint.py` (not included) uses SymPy to derive the three-site exact solution, graph-energy identity, zero-source and stiff-link limits, prior Dirac–Maxwell Hölder mismatch, and an independent fixed-normalization anisotropic Maxwell example. `verification_results.json` (not included) is the executable output. `SHA256SUMS` (not included) certifies the generated working files. This is an independent symbolic check of the stated equations, not an independent full parent Hamiltonian implementation.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN", "DYN v8" in this note): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.

Other working notes referred to by label:

- P2: [WN-04](WN-04_P2Parent.md)
- P14: not included in this release.
- P20: the retired Paper 20 series and its unpublished gate documents (see References).

Material named in this note but not included in this release: `P14CommonMode.md`, `P20_NS_gate_v1.tex`, `SHA256SUMS`, `SS-DYN_leafwise_dynamical_closure_v8.tex`, `verification_results.json`, `verify_parent_constraint.py`.
