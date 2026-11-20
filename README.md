# SSC-Research-Evidence

Unpublished working notes from the Scale Space research programme, released so that readers can check the evidence cited in *The Forgotten Coordinate: Technical Companion*.

**A citation shows where a result came from. It does not show that the result is correct.**

## What is here

| Path | Contents |
|---|---|
| `tc/ch15/README.md` | Evidence register for Technical Companion Chapter 15 (results U1–U18): what each note is, its role, its review status and its hashes |
| `tc/ch15/PREPARATION.md` | How each public edition was prepared from the cited working file, with both hashes |
| `tc/ch15/notes/` | Public editions of the 44 cited notes, WN-01 to WN-44 |
| `docs/` | Citation guide, review-status vocabulary, licensing policy and release checklist |
| `releases/` | A record of each tagged release |

Each note keeps its original file name after its evidence number, for example `WN-08_P18RegulatedLoop.md`.

## Status of the notes

- They are public editions of working records. Internal folder paths and workflow lines were removed, published papers are cited by version DOI, and later corrections are flagged where they apply. The mathematics, numbers and conclusions are as they were when cited, errors included. `tc/ch15/PREPARATION.md` lists the changes.
- The notes were prepared with AI assistance, including ChatGPT (OpenAI) and Claude (Anthropic), under the direction of Donald G. Palmer. None has had external scientific review, and AI-assisted reviews are not external peer review.
- Some are drafts, some record decisions not to adopt a proposal, and some have been partly corrected or withdrawn by later notes. The register gives each note's role and says where a later note corrects it.
- Many notes refer to calculation scripts, output files, archives or other working notes that are not part of this release.

## How to cite

Cite the note's evidence number and the tagged release, for example:

> Palmer, D. G., *SSC-Research-Evidence*, release v1.0.0, note WN-08.

[docs/CITATION_GUIDE.md](docs/CITATION_GUIDE.md) gives the full rules, and `CITATION.cff` gives the repository's citation data.

## Checking a copy

The register gives each public edition's SHA-256, which `sha256sum FILE` checks. It also gives the content hash of the working file that Chapter 15 cites, which identifies the source of each edition.

A matching hash shows the file is the released edition. It says nothing about whether the content is right.

## Author

Donald G. Palmer, independent researcher (ORCID [0000-0003-4335-5533](https://orcid.org/0000-0003-4335-5533)).

## Licence

The author's research notes and documentation in this repository are licensed under the Creative Commons Attribution 4.0 International licence (CC BY 4.0); see [LICENSE](LICENSE). Third-party material is not included and keeps its own terms. The book manuscripts are not part of this repository. [docs/PUBLICATION_AND_LICENSES.md](docs/PUBLICATION_AND_LICENSES.md) sets out the scope.

## Contributing

Questions, identified errors and suggested checks are welcome; see [CONTRIBUTING.md](CONTRIBUTING.md).
