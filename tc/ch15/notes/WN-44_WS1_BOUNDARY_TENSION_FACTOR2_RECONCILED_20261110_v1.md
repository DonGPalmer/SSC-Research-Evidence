> **Public edition of evidence note WN-44.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `WS1_BOUNDARY_TENSION_FACTOR2_RECONCILED_20261110_v1.md`, a working note dated 10 November 2026. Not peer reviewed.
> - **Source content hash:** `b752ebcef9d758e9be6a685e10aa75b8de9a5674d9672232a4840e0306e734a1` (2730 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# WS1 MAT–DYN — boundary factor-two reconciliation

**Date:** 10 November 2026  
**Status:** Noncanonical correction **CALCULATED AND VERIFIED**, independent review pending.  
**Predecessor alert:** [WN-43](WN-43_WS1_BOUNDARY_TENSION_FACTOR2_HOLD_20261110_v1.md).  
**Source report:** `SS_5DParent_IntervalGate_v1.md` (not included).

## Mathematical disposition

The original defined `λ_i=-2n_i W`, `W=6Mκ sin θ`, and `n_i A'=λ_i/(6M)`. At both endpoints the defined parameter is

\[
\boxed{\lambda_\pm=-12M\kappa\tanh(\kappa L).}
\]

The originally printed `−6Mκtanh(κL)` equals **`τ_i=λ_i/2`**, the actual coefficient in the single physical interval boundary action when the doubled/orbifold junction parameter convention is used. The numerical error is a misidentification of these two definitions in equation (7), not a failure of the stated negative sign or bulk background solution.

The corrected working edition specifies `S_boundary=−½Σ∫√−h λ_i`, with GHY terms and explicitly calculated metric/scalar endpoint variation. This yields the same equations (4)–(5). The original symbolic/Galerkin and independent finite-element scripts were rerun; their eigenvalue and tradeoff results are unaffected. A new boundary checker tests both endpoints and the formerly unchecked printed coefficient.

## Working files for independent review

- [WN-42](WN-42_SS_5DParent_IntervalGate_v1r1.md) — complete corrected report.
- `SS_5DParent_IntervalGate_v1r1.tex` (not included in this release) — editable complete source, with explicit boundary action.
- An evidence package with the independent boundary test, rerun original scripts, numerical outputs and technical audit (not included in this release).

## Reuse gate

- **v1 equation (7) remains HOLD**; it must not be copied with the `λ` label.
- **v1r1 is a verified corrected *working candidate***, with its mathematical boundary convention explicit. Independent review should check full GHY/Israel sign and normal conventions, then any radion/stability reuse.
- Do **not** interpret this repair as a proof of a stable radion, ghost-free boundary system, 5D-to-SS-DYN [v8, doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) equivalence, or quantum validity.
- No canonical paper has been overwritten.

Scientific correction and independent audit remain distinct.

---

## References and related notes (public edition)

Published works cited:

- **SS-DYN v8** (written "DYN" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-MAT v1** (written "MAT" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MAT: Scale-Extended Matter Sources: Protected Matching, Scale Transport and Completion Gates* (version 1). Zenodo. [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555). Published; current version.

Material named in this note but not included in this release: `SS_5DParent_IntervalGate_v1.md`, `SS_5DParent_IntervalGate_v1r1.tex`.
