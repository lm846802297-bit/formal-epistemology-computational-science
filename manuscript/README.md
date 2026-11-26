# Manuscript Development

## Working title

*Machine-Checked Proofs and Formalization Interfaces in Mathematical Physics: The Epistemology of Osterwalder–Schrader Reconstruction*

## Complete manuscript

[Open the integrated manuscript](full_manuscript.md). Editable sections:

1. [Abstract](00_abstract.md)
2. [Introduction](01_introduction.md)
3. [The Osterwalder–Schrader Formalization Network](02_epistemological_analysis_os_reconstruction.md)
4. [Inter-Formalization Warrant and Scientific Knowledge](03_discussion.md)
5. [Conclusion](04_conclusion.md)

## Writing standard

The manuscript follows peer-reviewed research-article conventions in philosophy of science and philosophy of physics. It draws selectively on related papers rather than imitating one journal or author. Prose is argumentative and continuous; conceptual claims are situated in the literature; mathematical and repository claims are attributed to exact sources; novelty is bounded.

## Central argument

The revised paper asks when a machine-checked theorem in one formalization can support an inference in another formalization of the same physical theory. It distinguishes local proof warrant, source-formalism correspondence, inter-formalization warrant, model instantiation, and target-directed scientific inference. The term inter-formalization warrant is an analytical distinction, not a universal theory.

## Citation and source practice

- APA 7 author–date citations.
- Formalization projects cited as scholarly software artifacts with exact commit pins.
- Original OS papers and Glimm–Jaffe cited for the mathematical formulations.
- Repository-reported verification status is attributed to maintainers; this project does not claim an independent Lean rebuild or proof replay.
- Root BibTeX: **bibliography/references.bib**. The integrated manuscript and root BibTeX file contain the same 23 cited works.
- EJPS AI-use disclosure is in **docs/EJPS_AI_DISCLOSURE_FOR_AUTHOR_REVIEW.md** and requires author confirmation.

## Editorial status

The follow-up critical review of originality and interface scope is complete. DeDeo and Duede's library-lock-in analysis is acknowledged, and the Comparator is described as a record-level audit-to-production interface rather than a cross-project physical bridge. The next phase is author-led source verification and EJPS submission preparation; the manuscript is not yet submission-ready.


## Major revision

The current manuscript's central question concerns when a theorem proved in one formalization can warrant an inference in another. The term **inter-formalization warrant** is a bounded analytical label, not a new universal theory or technical proof-transfer mechanism. The Comparator case must be described precisely: its challenge definitions reproduce the production package's own audit definitions, while the bridges and theorem equivalences are checked across the import boundary. See **docs/MAJOR_REVISION_REVIEW.md**.
