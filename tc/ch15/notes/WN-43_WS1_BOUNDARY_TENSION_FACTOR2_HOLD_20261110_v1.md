> **Public edition of evidence note WN-43.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `WS1_BOUNDARY_TENSION_FACTOR2_HOLD_20261110_v1.md`, a working note dated 10 November 2026. Not peer reviewed.
> - **Source content hash:** `338a895053feaacd7dcefd0c4285ccafc9388d3685e029102658914a93f505b1` (2510 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).
> - **Later correction:** The factor-of-two discrepancy it holds is reconciled in [WN-44](WN-44_WS1_BOUNDARY_TENSION_FACTOR2_RECONCILED_20261110_v1.md), and the corrected working edition is [WN-42](WN-42_SS_5DParent_IntervalGate_v1r1.md). An editorial note marks the affected passage; the original wording is kept.

# WS1 MAT–DYN: boundary-tension factor-of-two — HOLD BEFORE REUSE

**Date:** 10 November 2026  
**Status:** Verified arithmetic correction notice, noncanonical  
**Source:** `SS_5DParent_IntervalGate_v1.md` (not included), equations (2), (4), (5), (6), (7).

> **Editorial note (public edition, 19 November 2026):** A later note reconciles the factor of two: with the source definitions the endpoint parameter is λ± = −12Mκ tanh(κL), and the printed −6Mκ tanh(κL) is τ_i, half of λ_i, the coefficient in the single physical interval boundary action, so equation (7) misidentified the two; the eigenvalue and tradeoff results were rerun and are unaffected. That note keeps v1 equation (7) on HOLD for reuse with the λ label, and the corrected working edition v1r1 states the boundary convention explicitly, pending independent review. See [WN-44](WN-44_WS1_BOUNDARY_TENSION_FACTOR2_RECONCILED_20261110_v1.md) (Mathematical disposition; Reuse gate) and [WN-42](WN-42_SS_5DParent_IntervalGate_v1r1.md) §2 and its correction register. The text below is unchanged from the working note.

## Immediate issue

In the source, the superpotential and boundary definitions are
\[
\mathcal W(\phi)=6M\kappa\sin\theta,\qquad
\lambda_i(\phi)=-2n_i\mathcal W(\phi),\qquad
n_-=-1,\quad n_+=+1,
\]
and the kink has
\[
\sin\theta(y)=\tanh(\kappa y),\qquad
A'(y)=-2\kappa\tanh(\kappa y).
\]

Writing \(t=\tanh(\kappa L)>0\), direct substitution gives
\[
\lambda_+(\phi(L))=-2(+1)(6M\kappa t)=-12M\kappa t,
\]
\[
\lambda_-(\phi(-L))=-2(-1)(-6M\kappa t)=-12M\kappa t.
\]

Independently, its junction equation (5),
\(n_i A'=\lambda_i/(6M)\), gives \(\lambda_i=6Mn_iA'=-12M\kappa t\)
at **both** endpoints.

**Therefore, with equations (2), (4), (5), and their declared double-sided/orbifold convention retained, the coefficient in displayed equation (7) should be 12, not 6.** The printed equation (7) states `-6Mκ tanh(κL)`, a factor-two discrepancy.

## Review instructions

**HOLD equation (7) from use in further boundary, radion, stability, or spectral computations until it is reconciled.** The factor discrepancy is definite within the source's own definitions; *it does not prove* that the full boundary variational problem has been correctly normalized.

Before applying a correction, independently verify the 5D Gibbons–Hawking–York term, single-sided versus doubled/orbifold junction convention, scalar boundary equation, and downstream numerical substitutions. If these definitions remain, the corrected displayed endpoint tensions are both negative and have coefficient 12. The qualitative conclusion **parent not yet established** and the unrelated composite-scattering results are unchanged.

This notice checks the *live text and its equations*, **not** the original evidence files or full boundary constraint implementation. It was prepared at the author's request.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-MAT v1** (written "MAT" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MAT: Scale-Extended Matter Sources: Protected Matching, Scale Transport and Completion Gates* (version 1). Zenodo. [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555). Published; current version.

Material named in this note but not included in this release: `SS_5DParent_IntervalGate_v1.md`.
