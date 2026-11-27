# Next Bounded Research Task

## Task

Complete the author-led source and claim audit, then proceed to EJPS submission formatting. The critical review of the major revision is complete; do not reopen the research scope absent a concrete error.

## Current manuscript

- `manuscript/full_manuscript.md` — integrated article with abstract, main text, conclusion, and references.
- Separate section files remain the editable sources in `manuscript/`.
- The revised central question concerns the conditions under which a machine-checked theorem in one formalization can support an inference in another.

## Fixed acceptance criteria

1. The author verifies all 23 cited works and the 50 mapped claim/evidence records. In particular, inspect the continuation of Glimm and Jaffe (1987), second edition, §6.1(i), to verify the OS4 quantifiers, norm, and time-average formula; also verify the OSforGFF Remark 3.2 attribution, Rabe's theorem and model-reduct direction, DAMF/SC-TPTP scope, and the Comparator source/bridge claims.
2. Inter-formalization warrant remains a bounded analytical label for warrant relative to formal records, not a new universal theory or technical proof-transfer mechanism. DeDeo and Duede's (2026) library-lock-in and shared-model analysis is acknowledged; no novelty is claimed for correspondence or library dependence generally.
3. Comparator is described as a record-level audit-to-production interface. Its independence is limited to the import/elaboration/checking boundary; the challenge definitions are copied from the production package's own audit definitions.
4. The positive Comparator bridge and the absent public OSforGFF-to-OSreconstruction instantiation remain clearly distinguished.
5. Cherkis et al. are cited for the OSforGFF repository artifact; Douglas et al. for the accompanying Formalization of QFT paper.
6. The private companion examples are not identified with the pinned OSforGFF object without an inspectable bridge.
7. All cited works match the manuscript reference list and BibTeX; APA 7 and EJPS requirements are satisfied.
8. EJPS AI-use disclosure is reviewed and approved by the submitting author; the manuscript is anonymized and accompanied by a separate title page.
9. Springer Nature LaTeX source compiles locally, and the anonymous PDF passes formula, reference, metadata, and double-blind checks.
10. Subscription publishing is selected; no APC/Open Choice option is selected.

## Outputs

- Final source/claim audit.
- EJPS-format LaTeX source, anonymous manuscript, separate title page, BibTeX and compiled PDF.
- Build environment and compilation log.
- Final submission checklist.

## Non-goals

No new Lean implementation, fork, numerical computation, broad literature sweep, or expansion of the research question.


## EJPS submission preparation status (2026-11-27)

Prepared under `submission/`: a 23-item author-led source checklist; an AI-use declaration draft; an anonymous Springer Nature `sn-apa` LaTeX source with no author block and empty PDF-author metadata; a separate Title Page template with placeholders; and submission/build-status checklists.

Still pending: author completion of all 23 source checks; author approval of the AI declaration; author completion of Title Page fields; insertion of the approved disclosure into the anonymous manuscript; acquisition of the official Springer template class; local PDFLaTeX compilation and visual/PDF metadata inspection.

Do not mark the manuscript submission-ready until these items are complete.


## Source-audit integration status (2026-11-27)

The 50-claim report on `audit/submission-source-check-2026-11-27` commit `b5c4ce03b1157e2af018ff857cf7b166ec1b3ee7` has been mapped to the current manuscript and incorporated into the integrated Markdown manuscript, its four editable section sources, and the anonymous LaTeX source. The support documents now distinguish author-explained OSforGFF correspondence from the Comparator's Lean record bridges, and the public absence finding is bounded to the three pinned revisions.

The one specifically unresolved primary-source check is the continuation of Glimm and Jaffe (1987), second edition, §6.1(i), for the full OS4 quantifiers, norm, and time-average formula. The author must also approve all 23 source paraphrases. No Lean kernel rerun or new proof replay was performed during the source-audit integration.
