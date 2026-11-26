# Formal Epistemology of Computational Science

**Working paper:** *Machine-Checked Proofs and Mature Mathematical Formalisms in Physics: The Epistemology of Formalized Osterwalder–Schrader Reconstruction*

**Research question:** What epistemic role does machine-checked formalization play within mature mathematical formalisms in theoretical physics, and what does it add to the demonstration of model-internal results?

## Manuscript status

The complete first manuscript draft is available in [manuscript/full_manuscript.md](manuscript/full_manuscript.md). It includes the abstract, Introduction, OS Reconstruction epistemological analysis, Discussion, Conclusion, and a human-readable reference list.

- Main text: approximately 5,900 words, excluding references.
- Abstract: 204 words, plus keywords.
- The manuscript has been harmonized for academic prose, author–year citations, mathematical notation, and exact source attribution.
- It remains a research draft, not a journal-formatted submission.

## Working thesis

Machine checking strengthens the deductive warrant and auditability of formal derivations. It does not by itself establish correspondence with the source physical formalism, instantiate all theorem hypotheses in a concrete model, or warrant a target-directed physical inference.

The project uses a formalization-aware application of the Denotation–Demonstration–Interpretation framework. Its contribution is a source-critical and epistemological analysis of existing mathematical-physics formalizations, not a new general theory of scientific representation or cross-model warrant transfer.

## Research method

Reuse OSforGFF, OSreconstruction, and Comparator as prior mathematical/formalization results at exact pinned commits. Do not fork or reimplement them merely for convenience. Distinguish source inspection from independent execution; no fresh Lean build or proof replay is claimed.

## Repository map

- [Complete manuscript](manuscript/full_manuscript.md)
- [Separate manuscript sections](manuscript/README.md)
- [Research charter](docs/RESEARCH_CHARTER.md)
- [Model representation review](docs/MODEL_REPRESENTATION_REVIEW.md)
- [Working warrant framework](docs/FRAMEWORK.md)
- [OS reconstruction epistemological audit](docs/OS_RECONSTRUCTION_EPISTEMOLOGICAL_AUDIT.md)
- [Literature review](docs/LITERATURE_REVIEW.md)
- [Novelty matrix](docs/NOVELTY_MATRIX.md)
- [Paper outline](docs/PAPER_OUTLINE.md)
- [Research decisions](docs/DECISIONS.md)
- [Next bounded task](docs/NEXT_TASK.md)
- [BibTeX](bibliography/references.bib)
- [Source register](provenance/SOURCE_REGISTER.csv)
- [Exact Lean environment pins](provenance/OS_RECONSTRUCTION_ENVIRONMENT.yaml)

## Research status

The targeted literature comparison, OS source-critical audit, abstract, conclusion, and first integrated manuscript have been completed. Remaining work is final citation/source verification and adaptation to a selected journal's requirements. No new numerical computation or Lean implementation is planned for this manuscript.
