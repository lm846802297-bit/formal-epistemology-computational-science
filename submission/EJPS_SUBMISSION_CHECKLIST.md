# EJPS submission checklist

**Target:** European Journal for Philosophy of Science  
**Stage:** Preparation only; no submission has been made.

## Author actions

- [ ] Personally verify all 23 sources in `AUTHOR_SOURCE_VERIFICATION_CHECKLIST.md`.
- [ ] Record exact page/section/theorem/source-file locations and correct the manuscript as required.
- [x] Author confirmed the AI-use statement, model/version, and scope on 2026-11-27.
- [x] Inserted the detailed AI-use disclosure after the methodological paragraph in the Introduction and added an AI Use Declaration before the references.
- [x] Inserted the same disclosure in the separate Title Page template.
- [ ] Fill all placeholders in `title-page-template.tex`: name, affiliation, email, ORCID if available, acknowledgements, funding, competing interests, and approved AI statement.
- [ ] Approve the final title, abstract, keywords, and full text.
- [ ] Confirm with the EJPS editorial office whether public GitHub software repositories may appear as software references under the journal's rule that references should be published or accepted; if not, move exact commit pins to a footnote or suitable code-availability statement without losing version traceability.
- [ ] Confirm no simultaneous submission.
- [ ] Select subscription publication after acceptance; do not select Open Choice/APC under the no-author-fee requirement.

## Prepared in this branch

- [x] Current EJPS double-blind and separate Title Page requirements checked.
- [x] Anonymous LaTeX source prepared with no author block and empty PDF-author metadata.
- [x] Separate Title Page template prepared with explicit placeholders.
- [x] 23-item source-verification checklist prepared; all items remain pending author action.
- [x] AI-use disclosure author-confirmed and inserted in the manuscript and Title Page; original-source verification remains a separate pending task.
- [x] Springer Nature `sn-apa` class option used in the blind source.

## Technical acceptance still pending

- [ ] Obtain the official Springer Nature template package.
- [ ] Place `sn-jnl.cls` and required template support files alongside the source.
- [ ] Compile locally with PDFLaTeX; preserve full build log.
- [ ] Resolve all LaTeX errors and material overfull boxes.
- [ ] Inspect every formula, citation, reference, and hyperlink in the compiled PDF.
- [ ] Inspect PDF metadata and confirm no author identity is embedded.
- [ ] Confirm the Title Page is separate and absent from the blind manuscript PDF.
- [ ] Flatten the final source files into a single upload directory; EJPS instructions prohibit subfolders in the uploaded LaTeX source package.

## Fixed acceptance criteria

The package is ready only when the 23 source checks are author-complete, AI disclosure is approved and inserted, Title Page placeholders are filled, the anonymous PDF has no identifying information, the official Springer template compiles locally, and the final PDF has been inspected.
