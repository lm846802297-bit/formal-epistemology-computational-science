# Formal Epistemology of Computational Science

**Working paper:** *Machine-Checked Proofs and Formalization Interfaces in Mathematical Physics: The Epistemology of Osterwalder–Schrader Reconstruction*

## Manuscript status

The major-revision manuscript is available in [manuscript/full_manuscript.md](manuscript/full_manuscript.md). It includes the abstract, Introduction, OS formalization-network analysis, Discussion, Conclusion, and 20 cited references.

- Main text: approximately 6,250 words, excluding abstract and references.
- Abstract: 213 words, with six keywords.
- The central argument now concerns **inter-formalization warrant**: the conditions under which a machine-checked result in one formal representation can be reused in another.
- The manuscript is not yet ready for submission; the revised originality argument and source analysis require one further critical review before journal formatting.

## Revised contribution

The paper distinguishes:
1. local proof warrant supplied by kernel checking;
2. correspondence between a source physical formalism and its formal encoding;
3. inter-formalization warrant supplied by verified interfaces between formal records;
4. instantiation of theorem hypotheses by a concrete model;
5. target-directed scientific inference.

The OS case provides both a positive example (Comparator's proved record and theorem bridges) and a public composition boundary (no end-to-end public instantiation from the pinned OSforGFF object to the OSreconstruction input record).

This is a bounded, case-based analytical contribution. It does not claim a new general theory of scientific representation, proof interoperability, or cross-model empirical warrant.

## Primary journal target

European Journal for Philosophy of Science (EJPS) remains the recommended first target, with the subscription publishing route (no APC). Journal requirements and the no-fee plan are documented in [Journal Selection and Submission Plan](docs/JOURNAL_SELECTION_AND_SUBMISSION_PLAN.md).

## Research method

Reuse OSforGFF, OSreconstruction, and Comparator as prior results at exact pinned commits. No fork, reimplementation, new Lean build, proof replay, or numerical calculation is claimed. Source inspection is distinguished from independent execution.

## Repository map

- [Complete manuscript](manuscript/full_manuscript.md)
- [Separate manuscript sections](manuscript/README.md)
- [Inter-formalization warrant framework](docs/FRAMEWORK.md)
- [OS reconstruction source audit](docs/OS_RECONSTRUCTION_EPISTEMOLOGICAL_AUDIT.md)
- [Novelty matrix](docs/NOVELTY_MATRIX.md)
- [Reference audit](docs/REFERENCE_AUDIT.md)
- [Journal selection and submission plan](docs/JOURNAL_SELECTION_AND_SUBMISSION_PLAN.md)
- [Research decisions](docs/DECISIONS.md)
- [Next bounded task](docs/NEXT_TASK.md)
- [BibTeX](bibliography/references.bib)
- [Source register](provenance/SOURCE_REGISTER.csv)
- [Exact Lean environment pins](provenance/OS_RECONSTRUCTION_ENVIRONMENT.yaml)
