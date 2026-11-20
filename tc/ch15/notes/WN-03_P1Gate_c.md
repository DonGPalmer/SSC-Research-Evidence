> **Public edition of evidence note WN-03.** Cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15; see the [evidence register](../README.md).
>
> - **Source:** `P1Gate_c.md`, a working note dated 7 November 2026. Not peer reviewed.
> - **Source content hash:** `d2290a1011d85d5c9336bf77fcf5c503227aa99b3e3f5c7d1466ac0066260262` (6696 bytes). Algorithm: Dropbox content hash, i.e. SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks (for a file this size, SHA-256 applied twice).
> - **This edition:** public edition, revision 1, 19 November 2026. Editorial changes only: internal folder paths, file locations and workflow lines removed or replaced, the author named as "the author", other AI sessions described without names, and published works cited by version DOI. Equations, numbers and conclusions are unchanged. Every change is listed in [PREPARATION.md](../PREPARATION.md).

# SS WS1 P1c: which direction is more productive? Fifth-force and dependency checks

Date: 7 November 2026. Status: **draft for the author's review. Not independently reviewed.**
Follows [WN-01](WN-01_P1Gate.md) and [WN-02](WN-02_P1Gate_b.md) (WS1 MAT-DYN). Done on the author's instruction "Run both checks, please" (7 Nov 2026).
Labels as in [WN-01](WN-01_P1Gate.md): [Derived], [Computed], [Literature], [Assumed], [Conjecture]; [Read] = stated in the named document.

## 1. Question
After P1b, two options remain: option 2 (couple matter to a single leaf, giving up the protected weights) or option 3 (keep the protected weights, keep DYN v8 as the restricted reference model, and record the parent coupling as a model-specific obstruction). Two checks were run to judge which is more productive.

## 2. Fifth-force check (does single leaf survive experiment?)

### 2.1 Strength of the extra force
- Central-leaf coupling on the 3-site sech⁴ chain: massive/massless scalar-exchange ratio 0.3528 [Computed C3(D)]. By the 1↔3 reflection symmetry only the symmetric massive mode couples to the central leaf, so there is one Yukawa term [Derived].
- Massive spin-2 exchange between non-relativistic sources carries an extra factor 4/3 relative to massless exchange (2/3 vs 1/2 from the trace terms) [Derived, standard].
- So V = −G m₁m₂/r · (1 + α e^{−r/λ}) with **α ≈ 0.47, attractive** [Derived; the toy link masses in C3 were arbitrary, so α is fixed but λ is not].

### 2.2 Range: what DYN v8 says
- DYN v8's reference model D_{N,L} is single-metric: "there is no independent massive-spin-2 tower in this defined model" [Read, DYN v8 §3].
- In the parent comparison the Fierz–Pauli masses m_a are used but never given values [Read, DYN v8 §4, §10].
- The only scale: λ_T = (2κ)⁻¹ = 9.9 mm, "a legacy parent benchmark convention, not a newly predicted tensor range"; absolute scale selection is open [Read, DYN v8 §11]. §11 also says the fixed positive-universal Yukawa benchmark keeps its excluded status [Read].

### 2.3 Experimental limit
- Lee, Adelberger, Cook, Fleischer, Heckel, PRL 124, 101101 (2020), arXiv:2002.11761: "any gravitational-strength Yukawa interaction must have λ < 38.6 μm" (95% CL, |α| = 1); heavy-graviton mass > 5.1 meV [Literature, full text read]. The exact limit at α ≈ 0.5 was not read off their exclusion curve; it is of the same order (a few tens of μm).

### 2.4 Verdict
- Single-leaf coupling survives only if the massive spin-2 range is below roughly 40 μm, i.e. masses above about 5 meV [Derived from 2.1–2.3].
- The legacy 9.9 mm benchmark would be excluded by a factor of about 250 [Derived].
- Because DYN v8 leaves the link masses free, this does not kill option 2. It moves it: option 2 would need a reason for meV-scale link masses, which nothing in the corpus currently supplies [Derived].
- Not checked: Vainshtein-type screening of the massive mode in laboratory sources; it could weaken the bound but needs its own analysis [Conjecture].

## 3. Dependency check (what would option 2 force to be revised?)
Latest canonical versions read, read-only [Read; helper search of the author's working folder and Framework v21 [doi:10.5281/zenodo.23840776](https://doi.org/10.5281/zenodo.23840776)]:

| Document | Reliance on protected weights | Class |
|---|---|---|
| SS-PHEN v3 [doi:10.5281/zenodo.24044658](https://doi.org/10.5281/zenodo.24044658) | Eq. protectedsource T=F₀T⁴; protected Yukawa law (α_Q≈0.3208), universal charge, protected binary-radiation verdict; claims C04, C11, C12, C13, C20 | Heavy |
| SS-MAT v1 [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555) | Eq. protected T^prot=F₀T⁴; claim M01 "Protected source factorization"; δT defined relative to F₀ | Heavy |
| Framework v21 | Boxed "exact positive weight" F₀=sech⁴; KeyResult on universal zero-mode overlap; predictions on protected binaries (built on DYN v5) | Heavy |
| Book, "The Forgotten Coordinate" (v06, 15 Oct 2026) | Ch. 6 definition of protected matter; Ch. 7 central result (zero coupling to the massive continuum); Ch. 14 | Heavy (conceptual) |
| SS-DYN v8 [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296) | Parent comparison only (FP quadratic equivalence, 0.0012 bound, lapse obstruction); the reference model already uses one matter metric | Light for the reference model |
| SS-PIVOT v9 [doi:10.5281/zenodo.24044579](https://doi.org/10.5281/zenodo.24044579) | MAT interface T=F₀T⁴+δT; modal illustration | Light |
| SS-MEAS v2 [doi:10.5281/zenodo.23865651](https://doi.org/10.5281/zenodo.23865651), SS-BIO v4 [doi:10.5281/zenodo.23874087](https://doi.org/10.5281/zenodo.23874087) | Citation only | Light |
| SS-MULTI [v2, doi:10.5281/zenodo.23873325](https://doi.org/10.5281/zenodo.23873325), SS-QM [v2, doi:10.5281/zenodo.23875502](https://doi.org/10.5281/zenodo.23875502), SS-GEO [v6, doi:10.5281/zenodo.23603029](https://doi.org/10.5281/zenodo.23603029), SS-L5D [v1, doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609), SS-COS [v2, doi:10.5281/zenodo.23898678](https://doi.org/10.5281/zenodo.23898678), SS-CQMH [v1, doi:10.5281/zenodo.23875992](https://doi.org/10.5281/zenodo.23875992), SS-GCM [v1, doi:10.5281/zenodo.23875094](https://doi.org/10.5281/zenodo.23875094) | — | None |

Unaffected either way: the gravity-sector uses of sech (F(X)R measure, W₀ = 4/(3κ) fixing M₄², the sech² warp, the kink operator) [Read].
Not read: the newer Book review build (v13, 16 Oct 2026); SS-CQMH only searched.

## 4. Which is more productive
- **Option 3 is more productive now** [my judgement]. It needs no revision of any canonical paper, it matches what DYN v8 already says ("full parent remains open"), and P1Gate/P1b give it a sharp, variable-independent statement.
- **Option 2 costs four heavy revisions** (PHEN, MAT, Framework v21, the Book's central chapters) and needs a new, unsupported input: massive spin-2 masses above about 5 meV.
- One finding cuts the other way and is worth keeping: DYN v8's reference model already couples matter through a single metric, so the reference model itself does not need the protected weights. If option 3 is recorded, the open question becomes narrower: "find a ghost-free parent whose low-energy limit reproduces the protected source" (e.g. non-minimal links, or a cutoff analysis of the composite), rather than "repair the coupling".

## 5. Ruling
The author's ruling, 7 November 2026 (22:04 UTC), answering whether to go with recording the obstruction: **"Yes"**.
- Option 3 adopted: DYN v8's common-metric model stays the restricted reference model, and the protected weights are kept.
- Recorded outcome for MAT-DYN rank 1 (B5 action 5): within the minimal-link independent-leaf parent, no tested matter coupling is both ghost-free and protected. The printed shared scalar fails (rank N−1); the composite metric fails in a variable-independent test (two leaves) and in the 3-site chain, even for vacuum energy; single-leaf coupling is ghost-free but gives up the protected source and needs massive spin-2 masses above about 5 meV.
- Open question carried forward: a ghost-free parent whose low-energy limit reproduces the protected source (for example non-minimal links, or a cutoff analysis of the composite).
- Not done by this ruling: no canonical paper changed.

## 6. Files
- No new scripts: the strength ratio is from c3; the rest is reading.

---

## References and related notes (public edition)

Published works cited:

- **SS-BIO v4**: D. G. Palmer (2026). *SS-BIO: Scale-Extended Biological Dynamics in Scale Space: Configurational Structure, Transport, and Reaction–Diffusion Tests* (version 4). Zenodo. [doi:10.5281/zenodo.23874087](https://doi.org/10.5281/zenodo.23874087). Published; current version.
- **SS-COS v2** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-COS: Cosmological Geometry and Observational Diagnostics in Scale Space: Geodesic Optics, Clock–Ruler Tests and Conditional Confined Radiation* (version 2). Zenodo. [doi:10.5281/zenodo.23898678](https://doi.org/10.5281/zenodo.23898678). Published; current version.
- **SS-CQMH v1** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-CQMH: Hidden-Sector Projection and Conditional Hydrogenic Observables in Scale Space* (version 1). Zenodo. [doi:10.5281/zenodo.23875992](https://doi.org/10.5281/zenodo.23875992). Published; current version.
- **SS-DYN v5** (written "DYN v5" in this note; version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-DYN: A Scale-Localized Leafwise Dynamical Closure for Scale Space: Protected Tensor Gravity, a Repaired Scalar Continuum, and Constrained Collective Matte* (version 5). Zenodo. [doi:10.5281/zenodo.22731550](https://doi.org/10.5281/zenodo.22731550). Published; superseded by version 8 ([doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296)).
- **SS-DYN v8** (written "DYN v8" in this note): D. G. Palmer (2026). *SS-DYN: Nonlinear Common-Metric Dynamics and the Limits of Leafwise Completion* (version 8). Zenodo. [doi:10.5281/zenodo.23862296](https://doi.org/10.5281/zenodo.23862296). Published; current version.
- **SS-FRAMEWORK v21**: D. G. Palmer (2026). *The Scale Space–CNRS Programme: A Theoretical Framework* (version 21). Zenodo. [doi:10.5281/zenodo.23840776](https://doi.org/10.5281/zenodo.23840776). Published; current version.
- **SS-GCM v1** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-GCM: Bulk Sources, Junction Exchange and Smooth-Wall Controls for Scale Space Clock-Reading Geometry* (version 1). Zenodo. [doi:10.5281/zenodo.23875094](https://doi.org/10.5281/zenodo.23875094). Published; current version.
- **SS-GEO v6** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-GEO: Logarithmic Scale as a Geometric Coordinate: Exact-Distance Projection and Radial Scale Response* (version 6). Zenodo. [doi:10.5281/zenodo.23603029](https://doi.org/10.5281/zenodo.23603029). Published; current version.
- **SS-L5D v1** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-L5D: Clock Geometry and Consistent Five-Dimensional Extensions of Scale Space* (version 1). Zenodo. [doi:10.5281/zenodo.23874609](https://doi.org/10.5281/zenodo.23874609). Published; current version.
- **SS-MAT v1** (written "MAT" in this note): D. G. Palmer (2026). *SS-MAT: Scale-Extended Matter Sources: Protected Matching, Scale Transport and Completion Gates* (version 1). Zenodo. [doi:10.5281/zenodo.23863555](https://doi.org/10.5281/zenodo.23863555). Published; current version.
- **SS-MEAS v2**: D. G. Palmer (2026). *SS-MEAS: Measurement Projection and Identifiability in Scale Space: Calibrated Observables, Null Spaces, and Withheld-Probe Tests* (version 2). Zenodo. [doi:10.5281/zenodo.23865651](https://doi.org/10.5281/zenodo.23865651). Published; current version.
- **SS-MULTI v2** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-MULTI: Physical Scale as a Location Coordinate: A Multi-Scale Framework in Scale Space* (version 2). Zenodo. [doi:10.5281/zenodo.23873325](https://doi.org/10.5281/zenodo.23873325). Published; current version.
- **SS-PHEN v3** (written "PHEN" in this note): D. G. Palmer (2026). *SS-PHEN: Experimental Phenomenology of Scale Space: Protected Short-Range Scalar Response, Radiative Null Tests, and Matched Source Corrections* (version 3). Zenodo. [doi:10.5281/zenodo.24044658](https://doi.org/10.5281/zenodo.24044658). Published; current version.
- **SS-PIVOT v9**: D. G. Palmer (2026). *SS-PIVOT: From Scale Geometry to Gravitational Dynamics: What the Configuration Manifold Determines—and What It Does Not* (version 9). Zenodo. [doi:10.5281/zenodo.24044579](https://doi.org/10.5281/zenodo.24044579). Published; current version.
- **SS-QM v2** (version not stated in the note; the version current on the note's date is given): D. G. Palmer (2026). *SS-QM: Quantum States and Scale Profiles on Four-Dimensional Scale Space* (version 2). Zenodo. [doi:10.5281/zenodo.23875502](https://doi.org/10.5281/zenodo.23875502). Published; current version.

Other working notes referred to by label:

- P1b: [WN-02](WN-02_P1Gate_b.md)
