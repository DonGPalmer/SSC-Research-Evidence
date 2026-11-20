# Evidence release checklist

These checks apply to each note proposed for release. For release v1.0.0, the outcome of each check is recorded in [tc/ch15/PREPARATION.md](../tc/ch15/PREPARATION.md) and in [releases/](../releases/).

- [ ] Verify the working file's identity, version and content hash against the author's provenance records.
- [ ] Confirm authorship, AI-assistance disclosure, third-party rights and the licence.
- [ ] Remove private identifiers, internal-only paths, personal information, credentials and licensed material.
- [ ] Never silently alter scientific content: equations, numbers, verdicts and conclusions stay as written, and known errors are flagged, not repaired.
- [ ] Flag later corrections, withdrawals and limits at the affected passage, naming the correcting note.
- [ ] Check mathematical expressions and character encoding against the exact working file; record any reading problem.
- [ ] State which scripts, inputs and outputs are not included; do not invent missing verification.
- [ ] Label each result's review status explicitly (see [REVIEW_STATUS.md](REVIEW_STATUS.md)).
- [ ] Confirm the link from evidence number to public file to Chapter 15 result, with both hashes, in the register.
- [ ] Obtain the author's explicit approval of the final inventory, hashes, warnings, licence and release description.
- [ ] Commit, create a fixed version tag and release, compare the repository's file hashes with the register, and optionally archive the release (for example on Zenodo).
- [ ] Update the Technical Companion's access statement to the actual release address; for a later correction, keep the earlier release and publish an erratum.

**Stop condition:** an unresolved permission, identity or serious scientific-status conflict blocks release of the affected note, not necessarily the whole release.
