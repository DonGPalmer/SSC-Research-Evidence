# Preparation record: public editions of the Chapter 15 evidence notes

This record traces each note from the working file cited in *The Forgotten Coordinate: Technical Companion*, Chapter 15, to its public edition in this repository.

## How the editions were made (19 November 2026)

1. **Source.** Each edition starts from the exact bytes of the cited working file, checked against the source content hash that Chapter 15 cites. The working files are kept by the author and are not part of this release.
2. **Script pass.** A script added the provenance header and the closing "References and related notes" section. It replaced internal file names and folder paths with links to released notes or with "not included", and it added a version DOI at the first mention of each published paper. Each paper is cited by the version the note used, with its status: current, superseded or retired. Unpublished works are named as unpublished and are not included.
3. **Editorial pass.** The author's first name was replaced with "the author". Other AI sessions are described without names; a named product such as ChatGPT is kept. Workflow lines (saving, uploading, logging, review routing) were removed, internal coordination text was condensed, and Files sections were shortened. Every statement of scientific status was kept.
4. **Correction notes.** Where a later note corrects, withdraws or limits a claim, an editorial note sits just before the affected passage and names the correcting note. The original wording follows it unchanged.
5. **Check.** For every note, all numbers, mathematical symbols and operators were compared before and after the editorial pass. The only items removed were dates inside deleted workflow lines and internal folder names.
6. **Not done.** No equation, number, verdict or conclusion was changed, and no error was repaired. Known errors are flagged, not fixed.

Two source files (WN-04 and WN-26) were first read through a tool that garbled their mathematical symbols. The stored files were never damaged: their exact text was recovered and matched to the source content hash before editing.

The full line-by-line change log, which includes the removed internal text, is kept with the author's working files and is not published.

**Hashes.** Each public edition is identified by the SHA-256 of the file as published (check with `sha256sum FILE`). The source content hash uses the Dropbox algorithm: SHA-256 of the concatenated SHA-256 digests of the file's 4 MiB blocks, which for these files equals SHA-256 applied twice.

**Release.** The editions are first published by the repository commit that adds this file.

## Notes

### WN-01

- **Source:** `P1Gate.md`, 7 Nov 2026; 11539 bytes; content hash `34fa33a47e090e60d71202c51a2bcc9bc80b3d7dd33c10ad5cb6c8e247c058f7` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-01_P1Gate.md`](notes/WN-01_P1Gate.md), revision 1; 13541 bytes; SHA-256 `42cdcd9014eab641010ed5863d7dd713e0213ecddccda2db0c336692ad570cba`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 21 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN v8"; "SS-MAT v1"; "Framework v21".
- **Editorial changes:** the author named as "the author" (3); workflow lines removed or made neutral (3); Files section condensed (1); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-02

- **Source:** `P1Gate_b.md`, 7 Nov 2026; 6805 bytes; content hash `b64400fbb17bc50703ba58073d132134e923e7359c5ba5306bde70843c3e5e3a` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-02_P1Gate_b.md`](notes/WN-02_P1Gate_b.md), revision 1; 8456 bytes; SHA-256 `cb28e53811c58f08d17f341734e335d507f84ddbf107f74d24bf299f2b152f80`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 14 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-MAT v1"; "Framework v21".
- **Editorial changes:** the author named as "the author" (2); workflow lines removed or made neutral (1); internal locations removed or replaced (1); Files section condensed (1); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-03

- **Source:** `P1Gate_c.md`, 7 Nov 2026; 6696 bytes; content hash `d2290a1011d85d5c9336bf77fcf5c503227aa99b3e3f5c7d1466ac0066260262` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-03_P1Gate_c.md`](notes/WN-03_P1Gate_c.md), revision 1; 13433 bytes; SHA-256 `5893b18d94b056acf4fe5e1ed6d205321b4e81b745f6a9a519fb088089f860fc`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 6 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-PHEN v3"; "SS-MAT v1"; "SS-DYN v8"; "SS-PIVOT v9"; "SS-MEAS v2"; "SS-BIO v4"; "SS-MULTI"; "SS-QM"; "SS-GEO"; "SS-L5D"; "SS-COS"; "SS-CQMH"; "SS-GCM"; "Framework v21".
- **Editorial changes:** the author named as "the author" (3); workflow lines removed or made neutral (3); internal locations removed or replaced (3); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-04

- **Source:** `P2Parent.md`, 7 Nov 2026; 6141 bytes; content hash `dd41f74fb393e388fe398372f92a19f1167b1bf1b694714b94ce0f085b27965e` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-04_P2Parent.md`](notes/WN-04_P2Parent.md), revision 1; 8928 bytes; SHA-256 `acea779f60e51307869a8a824ed75ecec47472ba884097fd1fc74e4d611f8d69`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 12 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-L5D v1"; "SS-DYN"; "SS-DYN v6".
- **Editorial changes:** the author named as "the author" (2); workflow lines removed or made neutral (2); internal locations removed or replaced (1); Files section condensed (1); footer list of material not included updated (1).
- **Editorial correction notes inserted:** 1 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-05

- **Source:** `P15ParentClosure.md`, 8 Nov 2026; 8752 bytes; content hash `7d01a89a09c930b3d58e80a097a5a5f782c6bc72b9d4fc5a4aeb964eb9a431ad` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-05_P15ParentClosure.md`](notes/WN-05_P15ParentClosure.md), revision 1; 11783 bytes; SHA-256 `6b21fbd4e9d0919105df682a267b8a82d0f74cfa3907d245fad42b1f9642eae2`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 8 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN".
- **Editorial changes:** the author named as "the author" (2); workflow lines removed or made neutral (3); Files section condensed (1); footer list of material not included updated (1).
- **Editorial correction notes inserted:** 1 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-06

- **Source:** `SS_ParentMatter_Final_Decision_v1.md`, 8 Nov 2026; 9981 bytes; content hash `e68bbe76e128e9be75eddff36e95c957cf8c4b15de00c7ed9f6e0fc86a5c31bb` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-06_SS_ParentMatter_Final_Decision_v1.md`](notes/WN-06_SS_ParentMatter_Final_Decision_v1.md), revision 1; 11825 bytes; SHA-256 `5abbc36c89b58f0e04d73dc7f1c8561489e049fb57e1284817b1f000719c3356`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 10 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN".
- **Editorial changes:** other AI sessions described without names (2); internal locations removed or replaced (2); internal coordination text condensed (1); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-07

- **Source:** `SS_ParentMatter_Phase_Closeout_v1.md`, 8 Nov 2026; 6041 bytes; content hash `e56e3cb441daf84f1595d376e29c393d00b472e67a1d75bddffb5786e8634bf5` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-07_SS_ParentMatter_Phase_Closeout_v1.md`](notes/WN-07_SS_ParentMatter_Phase_Closeout_v1.md), revision 1; 8520 bytes; SHA-256 `f8ba66ebb13e611048a4336edc9acb239aeea09a614eee5d077c8939a77cf231`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 12 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN v8"; "SS-BIO"; "SS-MULTI".
- **Editorial changes:** the author named as "the author" (2); other AI sessions described without names (5); workflow lines removed or made neutral (1); internal locations removed or replaced (3); internal coordination text condensed (4); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-08

- **Source:** `P18RegulatedLoop.md`, 9 Nov 2026; 5218 bytes; content hash `cfc4056ffd5aa4dc2d6277354c091d6c167959e91838ba89289ea976aa40b0d7` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-08_P18RegulatedLoop.md`](notes/WN-08_P18RegulatedLoop.md), revision 1; 6760 bytes; SHA-256 `c6bed572360f6083a1ec2a68acc5c51580d6bbda66e1e2a6d1dbc55a3ef2dbf2`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **DOI citations added at first mention:** "SS-DYN".
- **Editorial changes:** the author named as "the author" (1); workflow lines removed or made neutral (3); internal locations removed or replaced (1); Files section condensed (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-09

- **Source:** `SS_ParentMatter_DiracMatching_v1.md`, 8 Nov 2026; 10074 bytes; content hash `8c76004ebe998eed916cdbc41f9a29d85a49a96169185fc88246160f37f099cc` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-09_SS_ParentMatter_DiracMatching_v1.md`](notes/WN-09_SS_ParentMatter_DiracMatching_v1.md), revision 1; 12017 bytes; SHA-256 `17de1c2f0d7000f69fefb72606899981583bd60d6454a1c9d70cdc0b25c094c1`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 7 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN v8".
- **Editorial changes:** internal locations removed or replaced (3); internal coordination text condensed (3).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-10

- **Source:** `SS_ParentMatter_Universality_Gate_v1.md`, 8 Nov 2026; 10652 bytes; content hash `b1bcaafeecad308abf3b287b4f85297455933611dc6fe81084cd96de66ccc155` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-10_SS_ParentMatter_Universality_Gate_v1.md`](notes/WN-10_SS_ParentMatter_Universality_Gate_v1.md), revision 1; 12147 bytes; SHA-256 `d4e4c55476fff5afe1acc7414c4e72a49d803ed4f1df4daec28b2bcc9c575649`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 12 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN v8".
- **Editorial changes:** internal locations removed or replaced (2); internal coordination text condensed (3); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-11

- **Source:** `SS_ParentMatter_FiniteSpectrum_v1.md`, 8 Nov 2026; 9236 bytes; content hash `4cb1294b7a17d874f0b046ee8d2f53017df788583a332aa5b7af58f3b92c89bc` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-11_SS_ParentMatter_FiniteSpectrum_v1.md`](notes/WN-11_SS_ParentMatter_FiniteSpectrum_v1.md), revision 1; 10898 bytes; SHA-256 `5026780e3fc2263c792677ca164bf6538f1308c757758b4967dae8091e3505ce`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 6 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN v8".
- **Editorial changes:** other AI sessions described without names (3); internal coordination text condensed (3); Files section condensed (1); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-12

- **Source:** `SS_ParentMatter_RelativeMetric_ConstraintGate_v1.md`, 8 Nov 2026; 12171 bytes; content hash `e1a5a5fe215183f05758c7e3bab9a0b0b0b0a1dd6a2ab7041c4e461a0f89bd32` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-12_SS_ParentMatter_RelativeMetric_ConstraintGate_v1.md`](notes/WN-12_SS_ParentMatter_RelativeMetric_ConstraintGate_v1.md), revision 1; 14413 bytes; SHA-256 `f5e298e0abb8fffdfc31c8af07735f6c2d61ddc5c0cb11c9468e0a621a85c128`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 9 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN v8".
- **Editorial changes:** workflow lines removed or made neutral (1); internal locations removed or replaced (1); internal coordination text condensed (4).
- **Editorial correction notes inserted:** 1 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-13

- **Source:** `SS_ParentMatter_WardExchange_v1.md`, 8 Nov 2026; 8416 bytes; content hash `20781d62efc0f37673d9fbb978f986d1402e7139f787ca51620b15fe424c8355` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-13_SS_ParentMatter_WardExchange_v1.md`](notes/WN-13_SS_ParentMatter_WardExchange_v1.md), revision 1; 9836 bytes; SHA-256 `fc26201837358aa28477692d12ea8913ff9680357ad1e2221c35bfd598847876`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 7 (links to released notes, or "not included").
- **Editorial changes:** other AI sessions described without names (2); workflow lines removed or made neutral (1); internal coordination text condensed (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-14

- **Source:** `P3ScaleSpectra.md`, 8 Nov 2026; 11615 bytes; content hash `3fc5105343e0dea54bc7a8d5731395fcbd14ab45b7e60da91a81022a771480c9` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-14_P3ScaleSpectra.md`](notes/WN-14_P3ScaleSpectra.md), revision 1; 17281 bytes; SHA-256 `6a949f8f77d3a4972de19e4dce2de70720306e00c451198baa6c87ee0fb0c100`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 15 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-MULTI v2"; "SS-DYN v8"; "SS-MAT"; "SS-GEO v6"; "SS-L5D"; "Paper 20".
- **Editorial changes:** the author named as "the author" (4); workflow lines removed or made neutral (2); internal locations removed or replaced (1); Files section condensed (1); footer list of material not included updated (1).
- **Editorial correction notes inserted:** 3 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-15

- **Source:** `P4CouplingWeight.md`, 8 Nov 2026; 8053 bytes; content hash `6e45847bf61348be90f32f518807db758ec4d6328cb5d70801741f4f5cc59ca5` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-15_P4CouplingWeight.md`](notes/WN-15_P4CouplingWeight.md), revision 1; 11043 bytes; SHA-256 `abb4ebcb8e970b5ba7f2e2c6b8ce0e3a3549e44f749635f6ea980500c02a110a`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 2 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN"; "SS-MULTI"; "SS-DYN v6"; "Paper-20".
- **Editorial changes:** workflow lines removed or made neutral (1); internal locations removed or replaced (4); Files section condensed (2).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-16

- **Source:** `P6ReflectionFold.md`, 8 Nov 2026; 8004 bytes; content hash `55b1f12f123e7ab8476c815bd7b8d78e43283c888564a05b8f494f62ba39e91f` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-16_P6ReflectionFold.md`](notes/WN-16_P6ReflectionFold.md), revision 1; 10841 bytes; SHA-256 `d11d266ff2030295d87466276b964d1b43cb97651b42435e85f9fcacaddf4486`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 2 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN"; "Paper-20".
- **Editorial changes:** workflow lines removed or made neutral (1); internal locations removed or replaced (1); Files section condensed (2).
- **Editorial correction notes inserted:** 1 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-17

- **Source:** `P7FoldRule.md`, 8 Nov 2026; 5819 bytes; content hash `689f5646c3420416447f442bf5a6022371882ed0c1f2e40023fda49801dc044c` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-17_P7FoldRule.md`](notes/WN-17_P7FoldRule.md), revision 1; 10180 bytes; SHA-256 `069f1d3a810f10d73e857d86139e532890fbe404d2b2c3521f1c254733e3bfd9`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 2 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-L5D"; "SS-DYN"; "Paper-20".
- **Editorial changes:** the author named as "the author" (2); workflow lines removed or made neutral (1); internal locations removed or replaced (1); internal coordination text condensed (2); Files section condensed (2).
- **Editorial correction notes inserted:** 3 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-18

- **Source:** `P11Rev.md`, 8 Nov 2026; 14550 bytes; content hash `8c4f411f2170a186df578174602f126b0aba87186bf4ee46470919d4ccb90a6e` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-18_P11Rev.md`](notes/WN-18_P11Rev.md), revision 1; 18258 bytes; SHA-256 `32f809f57eeb528996fafd0eac5ab166efcf13563f3f3612226092b4d95dcfe1`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 1 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN"; "SS-DYN v6"; "SS-PHEN v2"; "SS-L5D".
- **Editorial changes:** the author named as "the author" (8); other AI sessions described without names (1); workflow lines removed or made neutral (1); internal locations removed or replaced (1); internal coordination text condensed (1); Files section condensed (2).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-19

- **Source:** `P11bDYNWording.md`, 8 Nov 2026; 8738 bytes; content hash `8d6168a54041df24dc8bbf05db37a9549c39e90401418ec5d555a745f35876ec` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-19_P11bDYNWording.md`](notes/WN-19_P11bDYNWording.md), revision 1; 12699 bytes; SHA-256 `50380638c78d5769c04fa74a2d53c6701a20c407285296d1f7852fa13daf6250`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 8 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN"; "SS-DYN v6"; "SS-PHEN v2"; "SS-L5D".
- **Editorial changes:** the author named as "the author" (2); workflow lines removed or made neutral (1); internal locations removed or replaced (4); internal coordination text condensed (2); Files section condensed (2).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-20

- **Source:** `P12FoldDilation.md`, 8 Nov 2026; 5326 bytes; content hash `807e4bd8a151440ecb5d9f3e0a7be5a821624193f40ecd0478072638c64b8f96` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-20_P12FoldDilation.md`](notes/WN-20_P12FoldDilation.md), revision 1; 7742 bytes; SHA-256 `e26f94890f4c804deda8aa66648645849bb0ede434e483faefdef2e0872b4e8d`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 3 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-GEO v6"; "SS-DYN"; "SS-L5D".
- **Editorial changes:** the author named as "the author" (2); workflow lines removed or made neutral (1); internal locations removed or replaced (1); internal coordination text condensed (2); Files section condensed (2).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-21

- **Source:** `P13L5DScaleGeometry.md`, 8 Nov 2026; 4358 bytes; content hash `75b7e1cfc7117392df2c03510c37e2f53a1e59f7d049550c843111ced6dc96e3` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-21_P13L5DScaleGeometry.md`](notes/WN-21_P13L5DScaleGeometry.md), revision 1; 7039 bytes; SHA-256 `b07160822e9ceaa2918114176be00c73691924df13c6c29ca59838ab30e80910`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 3 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-L5D"; "SS-GEO v6"; "SS-PIVOT v8"; "SS-DYN v8".
- **Editorial changes:** the author named as "the author" (1); workflow lines removed or made neutral (1); internal locations removed or replaced (2); internal coordination text condensed (3); Files section condensed (2).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-22

- **Source:** `P8CutoffBox.md`, 8 Nov 2026; 5397 bytes; content hash `b25ea2242cbcf23c23503d73cb22f08633f330f0f46444c6e68e45fd409e15ca` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-22_P8CutoffBox.md`](notes/WN-22_P8CutoffBox.md), revision 1; 7589 bytes; SHA-256 `3c18b832121c6387174b83472595d232ca6303b6bc01a0a1bb080048e07f07da`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 2 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN".
- **Editorial changes:** the author named as "the author" (1); workflow lines removed or made neutral (1); internal locations removed or replaced (1); internal coordination text condensed (2); Files section condensed (2).
- **Editorial correction notes inserted:** 1 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-23

- **Source:** `P9FarRegion.md`, 8 Nov 2026; 5823 bytes; content hash `aa66748c676e7bcb3753e810c4b5679c3e00efcf5a66b7412c772a77e920963b` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-23_P9FarRegion.md`](notes/WN-23_P9FarRegion.md), revision 1; 7350 bytes; SHA-256 `bf480b2528fd8a8f8534ebb521e918a6b3f34e612f3f7b613080fd0fbc9b3c5e`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 2 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN".
- **Editorial changes:** the author named as "the author" (1); workflow lines removed or made neutral (1); internal locations removed or replaced (1); internal coordination text condensed (2); Files section condensed (2).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-24

- **Source:** `P5CommonScale.md`, 8 Nov 2026; 5790 bytes; content hash `661e2642d36567836f79901f9848238707c31054ce906664d0dd4fc3953d383d` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-24_P5CommonScale.md`](notes/WN-24_P5CommonScale.md), revision 1; 10117 bytes; SHA-256 `1113e6cbf8b962117ab875890520c45593b3d7c684d57d08e33de08f1069b269`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 2 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN"; "SS-DYN v6/v8"; "Paper-20".
- **Editorial changes:** workflow lines removed or made neutral (1); internal locations removed or replaced (1); Files section condensed (2).
- **Editorial correction notes inserted:** 2 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-25

- **Source:** `P21MatterIntoGravity.md`, 9 Nov 2026; 7016 bytes; content hash `79ccbee0fd59221b6c9baa58df8fddff7e3e9fbdfa0996719ec484aa210b38ef` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-25_P21MatterIntoGravity.md`](notes/WN-25_P21MatterIntoGravity.md), revision 1; 8737 bytes; SHA-256 `aaaa29e93d9eb5a24f30985eb318483fcbc14cb822e3c401ff5c695a9fc17b14`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 4 (links to released notes, or "not included").
- **Editorial changes:** the author named as "the author" (1); other AI sessions described without names (1); internal locations removed or replaced (1); Files section condensed (1); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-26

- **Source:** `P24ScaleKinkWeight.md`, 9 Nov 2026; 6869 bytes; content hash `6552e119699ba50f1cbc9d48ce6c7f52d4c184bf5eac488f61a9a7bec1b983eb` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-26_P24ScaleKinkWeight.md`](notes/WN-26_P24ScaleKinkWeight.md), revision 1; 9045 bytes; SHA-256 `f8c8b520f8d8ef03df0a3a579daf29c1eec9108fcef30d878906ef3458b54f43`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 4 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN".
- **Editorial changes:** the author named as "the author" (1); internal locations removed or replaced (1); Files section condensed (1); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-27

- **Source:** `P19DiracMaxwellParent.md`, 9 Nov 2026; 8139 bytes; content hash `7536b48f3635d81d314ffca38672a6a68a2888d9883dbfb8861a2eb3d0050cfb` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-27_P19DiracMaxwellParent.md`](notes/WN-27_P19DiracMaxwellParent.md), revision 1; 9961 bytes; SHA-256 `0fa31bbae8927c0e65bd75b41517808180ff23d748ab57fcf315e58e208394c0`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 7 (links to released notes, or "not included").
- **Editorial changes:** the author named as "the author" (1); other AI sessions described without names (1); internal locations removed or replaced (1); Files section condensed (1); footer list of material not included updated (1).
- **Editorial correction notes inserted:** 1 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-28

- **Source:** `P20ChiralParent.md`, 9 Nov 2026; 7065 bytes; content hash `031cadde1039ab7ea8210f64be2fe1702f29a479eec39f934aa52a7c895d7b19` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-28_P20ChiralParent.md`](notes/WN-28_P20ChiralParent.md), revision 1; 11732 bytes; SHA-256 `a9df472f231ab85587e311b6826a5b28056ce4aa071f8ac00e0784b2930e7951`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 8 (links to released notes, or "not included").
- **Editorial changes:** the author named as "the author" (1); other AI sessions described without names (1); internal locations removed or replaced (1); Files section condensed (1); footer list of material not included updated (1).
- **Editorial correction notes inserted:** 6 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-29

- **Source:** `P20bReviewCorrections.md`, 9 Nov 2026; 5601 bytes; content hash `dea93d5cd67c2c112f549a7d61ad55bdd9249494dd799072342bb6c99db44d6d` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-29_P20bReviewCorrections.md`](notes/WN-29_P20bReviewCorrections.md), revision 1; 7322 bytes; SHA-256 `939304a880d9e924a2d68b4f4dd0fba500adc6f252248648a1c9439af41bb612`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 5 (links to released notes, or "not included").
- **Editorial changes:** other AI sessions described without names (1); workflow lines removed or made neutral (2); Files section condensed (1); footer list of material not included updated (1).
- **Editorial correction notes inserted:** 1 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-30

- **Source:** `P22SelfEnergyWard.md`, 9 Nov 2026; 6355 bytes; content hash `93f44d10b67b54696465ef20af3360a906c41fde959323697d9d40f6ae004fd1` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-30_P22SelfEnergyWard.md`](notes/WN-30_P22SelfEnergyWard.md), revision 1; 7657 bytes; SHA-256 `70042afd9b99cc9ccb6a51421aa15b84c0230019fa94dbb7ccc4a22ea15fde61`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 7 (links to released notes, or "not included").
- **Editorial changes:** the author named as "the author" (1); internal locations removed or replaced (1); Files section condensed (1); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-31

- **Source:** `P23NonAbelianHiggs.md`, 9 Nov 2026; 5476 bytes; content hash `8f1918a8d02fffd5ea8de751c046e883fbd05712c99056d742b86f674175802a` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-31_P23NonAbelianHiggs.md`](notes/WN-31_P23NonAbelianHiggs.md), revision 1; 6751 bytes; SHA-256 `0b8c941377d070965ba349d54d5b9830e6ef06026641a144de8a51cb1d640d93`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 6 (links to released notes, or "not included").
- **Editorial changes:** the author named as "the author" (1); internal locations removed or replaced (1); Files section condensed (1); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-32

- **Source:** `P26ChargeExtentOnKink.md`, 9 Nov 2026; 6485 bytes; content hash `f120196ede79e0063c1f19a1c1a760ac9f56eb4a8442972815f77ffbadb71453` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-32_P26ChargeExtentOnKink.md`](notes/WN-32_P26ChargeExtentOnKink.md), revision 1; 9003 bytes; SHA-256 `3b0f06bbf5d126578b891660aaf8a845da891bb8dc36f00271caa328fa2d8439`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **DOI citations added at first mention:** "SS-MAT v1".
- **Editorial changes:** internal locations removed or replaced (1); Files section condensed (1).
- **Editorial correction notes inserted:** 1 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-33

- **Source:** `P27PhotonWarpWeight.md`, 9 Nov 2026; 3752 bytes; content hash `0febe637835d64b138a31c16a6604c19a7ec857a53cdaa62fddc0b51bace98b5` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-33_P27PhotonWarpWeight.md`](notes/WN-33_P27PhotonWarpWeight.md), revision 1; 5222 bytes; SHA-256 `a0480c4bcffc0df51415ba20a5b02298bb28f60d09ff199543fb2f1b5767d83c`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 1 (links to released notes, or "not included").
- **Editorial changes:** internal coordination text condensed (1); Files section condensed (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-34

- **Source:** `P28ChargedDropletKinkSize.md`, 9 Nov 2026; 5268 bytes; content hash `aecfc753aa0af902c5c326c72fcde421192d1539fa6ca5789a9d96e593f11b43` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-34_P28ChargedDropletKinkSize.md`](notes/WN-34_P28ChargedDropletKinkSize.md), revision 1; 6804 bytes; SHA-256 `1e25075909d009eafb5046baa4ca709c3c870f8f3e463ebe7634b7c618620f31`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 2 (links to released notes, or "not included").
- **Editorial changes:** internal coordination text condensed (1); Files section condensed (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-35

- **Source:** `SS_SingleActionReduction_v1.md`, 9 Nov 2026; 15955 bytes; content hash `4f30dc0d9503f21c09bacd1c3a8c12604060421add8f8d8c33f2dc6d94ab643e` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-35_SS_SingleActionReduction_v1.md`](notes/WN-35_SS_SingleActionReduction_v1.md), revision 1; 19067 bytes; SHA-256 `1e355afd5eb5eed08aaa5dd50cb9a469f1e5b0cbade80c2c1c7f771737edc1ba`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 11 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN v8"; "SS-MAT"; "SS-MULTI".
- **Editorial changes:** workflow lines removed or made neutral (2); internal coordination text condensed (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-36

- **Source:** `SS_TwoReductionComparison_v1.md`, 9 Nov 2026; 13155 bytes; content hash `4490be8d53923cf27075ee61d7680438facbb9560189627acbef9df2be5d72bc` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-36_SS_TwoReductionComparison_v1.md`](notes/WN-36_SS_TwoReductionComparison_v1.md), revision 1; 16328 bytes; SHA-256 `718d6588faec7f8d3e2815b987279ee8e8459073668033a38447506a35cdf64d`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 13 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN v8".
- **Editorial changes:** workflow lines removed or made neutral (2); internal locations removed or replaced (1); internal coordination text condensed (2).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-37

- **Source:** `SS_KinkFermionGauge_ParentGate_v1.md`, 9 Nov 2026; 16494 bytes; content hash `72719436b2d9d0cde501e4aa37a716463a696ffdff64cc8713ece0ba97c8b82a` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-37_SS_KinkFermionGauge_ParentGate_v1.md`](notes/WN-37_SS_KinkFermionGauge_ParentGate_v1.md), revision 1; 19692 bytes; SHA-256 `0334537689b627b885a5a6254e30642ab12c26c4fcdf0481b5e208e525872e40`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 17 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN"; "SS-GEO".
- **Editorial changes:** other AI sessions described without names (2); workflow lines removed or made neutral (1); internal coordination text condensed (1); footer list of material not included updated (1).
- **Editorial correction notes inserted:** 1 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-38

- **Source:** `SS_FullFiniteAmplitude_ParentGate_v1.md`, 9 Nov 2026; 14989 bytes; content hash `2f142fa534badc8a6835ac83a3cf71d940d3f2f2dd2b6b0e0e590a1ae7da16a4` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-38_SS_FullFiniteAmplitude_ParentGate_v1.md`](notes/WN-38_SS_FullFiniteAmplitude_ParentGate_v1.md), revision 1; 17936 bytes; SHA-256 `671b26dd9035186d20266d8ba9072ce58968325e66e1665c45cc91f221a4a3b4`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 11 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN".
- **Editorial changes:** workflow lines removed or made neutral (2); internal coordination text condensed (3); Files section condensed (1); footer list of material not included updated (1).
- **Editorial correction notes inserted:** 1 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-39

- **Source:** `SS_OnShellMatch_Decision_v1.md`, 9 Nov 2026; 15147 bytes; content hash `1c055a996a104abed94237aad149c08f168354e55774cb3143bc503030bda07d` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-39_SS_OnShellMatch_Decision_v1.md`](notes/WN-39_SS_OnShellMatch_Decision_v1.md), revision 1; 18223 bytes; SHA-256 `354267247317e33fd99aca91e58d249a94ac20f2dfdc419208aed825f41d80c9`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 15 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN".
- **Editorial changes:** workflow lines removed or made neutral (3); internal locations removed or replaced (2); internal coordination text condensed (3); footer list of material not included updated (1).
- **Editorial correction notes inserted:** 1 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-40

- **Source:** `SS_ProfileSelection_Decision_v1.md`, 9 Nov 2026; 15671 bytes; content hash `9e6bbd9f6a1ff8e60de89f17526605f46376a13d19c4862dc3f52abe4d8ee7be` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-40_SS_ProfileSelection_Decision_v1.md`](notes/WN-40_SS_ProfileSelection_Decision_v1.md), revision 1; 17842 bytes; SHA-256 `b1496dbba596bd93af21440bf08e2f41643af0dd1c71bacfec12306299718b63`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 13 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN v8"; "SS-GEO".
- **Editorial changes:** workflow lines removed or made neutral (1); internal locations removed or replaced (1); internal coordination text condensed (1); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-41

- **Source:** `SS_Parent5D_Decision_v1.md`, 10 Nov 2026; 15422 bytes; content hash `b5a5ad0084ac80e9aa3f39c51ed590624babe99c39c2530966e465b3c70124d6` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-41_SS_Parent5D_Decision_v1.md`](notes/WN-41_SS_Parent5D_Decision_v1.md), revision 1; 17347 bytes; SHA-256 `6a1d9acacd9a4ca77f64cffe6de54f64f0e2153cc42e55eb804510217168dc11`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 11 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN"; "SS-MAT".
- **Editorial changes:** the author named as "the author" (1); other AI sessions described without names (1); workflow lines removed or made neutral (1); internal locations removed or replaced (1); internal coordination text condensed (1); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-42

- **Source:** `SS_5DParent_IntervalGate_v1r1.md`, 10 Nov 2026; 18387 bytes; content hash `114a45c1c44d8dff23bad3ffd5014ddc4751b29b4e2134e781154169ca7553d5` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-42_SS_5DParent_IntervalGate_v1r1.md`](notes/WN-42_SS_5DParent_IntervalGate_v1r1.md), revision 1; 20251 bytes; SHA-256 `a4ebfcf9d457579a1d47734d1e9865802fbfc962b4d3039ab8ef73939356163e`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 12 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN v8"; "SS-MAT".
- **Editorial changes:** workflow lines removed or made neutral (2); internal locations removed or replaced (1); internal coordination text condensed (3); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-43

- **Source:** `WS1_BOUNDARY_TENSION_FACTOR2_HOLD_20261110_v1.md`, 10 Nov 2026; 2510 bytes; content hash `338a895053feaacd7dcefd0c4285ccafc9388d3685e029102658914a93f505b1` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-43_WS1_BOUNDARY_TENSION_FACTOR2_HOLD_20261110_v1.md`](notes/WN-43_WS1_BOUNDARY_TENSION_FACTOR2_HOLD_20261110_v1.md), revision 1; 5049 bytes; SHA-256 `2bb50685b515c5471411fc9c539a57328d0be571160efb8fde0cb465425f1b01`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 1 (links to released notes, or "not included").
- **Editorial changes:** other AI sessions described without names (1); workflow lines removed or made neutral (1); internal coordination text condensed (4).
- **Editorial correction notes inserted:** 1 (each marked "Editorial note (public edition, 19 November 2026)" in the text; header "Later correction" line added or updated).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).

### WN-44

- **Source:** `WS1_BOUNDARY_TENSION_FACTOR2_RECONCILED_20261110_v1.md`, 10 Nov 2026; 2730 bytes; content hash `b752ebcef9d758e9be6a685e10aa75b8de9a5674d9672232a4840e0306e734a1` (Dropbox algorithm, as cited in Chapter 15).
- **Public edition:** [`notes/WN-44_WS1_BOUNDARY_TENSION_FACTOR2_RECONCILED_20261110_v1.md`](notes/WN-44_WS1_BOUNDARY_TENSION_FACTOR2_RECONCILED_20261110_v1.md), revision 1; 4258 bytes; SHA-256 `18efc7d2f80375cb699b1407b5b2d3aea5174a692e8a3b79da4f072ff49516ce`.
- **Added:** a provenance header and a closing "References and related notes" section.
- **File names and paths replaced:** 6 (links to released notes, or "not included").
- **DOI citations added at first mention:** "SS-DYN".
- **Editorial changes:** other AI sessions described without names (3); internal coordination text condensed (4); Files section condensed (1); footer list of material not included updated (1).
- **Mathematics, numbers, verdicts and conclusions:** unchanged (checked by comparing every number and mathematical symbol before and after editing).
