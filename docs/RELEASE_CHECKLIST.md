# Governed evidence-intake and release checklist

A public catalogue may exist before its underlying sources. The following checks apply **for each proposed WN source**:

- [ ] Verify original file identity, version and content hash against live SSC provenance records.
- [ ] Confirm authorship, AI-assistance disclosure, third-party rights, and permitted publication terms.
- [ ] Review for private IDs, internal-only paths, personal information, credentials and licensed material.
- [ ] Preserve original note and include a clearly identified corrected edition if necessary; never silently alter scientific content.
- [ ] Document status (derived/conditional/open/contradicted/superseded/withdrawn), limitations and citations to external literature.
- [ ] Check mathematical expressions and character encoding; document uncertainty where original text is damaged.
- [ ] Include calculation scripts, inputs, outputs, environment and a reproducibility statement **where available**; do not invent missing verification.
- [ ] Independently review each published result or label it explicitly unreviewed and exploratory.
- [ ] Confirm WN identifier ↔ public source file ↔ TC U-result link, with checksum and reviewer notes.
- [ ] Obtain explicit author approval for public release and the applicable license; consider publisher requirements.
- [ ] Publish immutable GitHub tag/release, compare repository hashes, and optionally archive that release on Zenodo.
- [ ] Update the TC reference to the actual release/commit/DOI; retain the prior release and publish an erratum if corrected.

**Stop condition:** An unresolved permission, identity or serious scientific-status conflict blocks release of the affected file, not necessarily the entire archive.
