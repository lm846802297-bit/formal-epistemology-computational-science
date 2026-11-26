# Formal Epistemology of Computational Science

**Working paper:** *Machine-Checked Proofs and Mature Mathematical Formalisms in Physics: The Epistemology of Formalized Osterwalder–Schrader Reconstruction*

**Question:** What epistemic role does machine-checked formalization play within mature mathematical formalisms in theoretical physics, and what does it add to the demonstration of model-internal results?

## Working thesis

Machine checking strengthens the reliability and auditability of formal derivations. It does not by itself establish correspondence with the source physical formalism, instantiate all theorem hypotheses in a concrete model, or warrant a target-directed physical inference.

The project uses a **formalization-aware DDI framework**: Denotation, Demonstration, Interpretation, with explicit treatment of source-formalism correspondence and kernel-checked proof within Demonstration.

## Manuscript status

The first integrated draft of the three core sections is available in the **manuscript/** directory:
- Introduction
- Epistemological Analysis of Osterwalder–Schrader Reconstruction
- Discussion

The draft is approximately 6,000 words and is not yet submission-ready. The abstract, conclusion, citation harmonization, and journal formatting remain editorial tasks.

## Research method

Reuse the existing OSforGFF, OSreconstruction, and Comparator results as prior mathematical/formalization work. Do not fork or reimplement these projects merely for convenience. Our independent contribution is the source-critical and epistemological analysis of exact theorem statements, assumptions, endpoints, interpretation, and warrant interfaces. Cite original authors and pin exact commits. Distinguish source inspection from independent execution; never claim a fresh Lean build or proof replay unless performed.

## Repository map

- [Manuscript guide](manuscript/README.md)
- [Research charter](docs/RESEARCH_CHARTER.md)
- [Phase-two model representation review](docs/MODEL_REPRESENTATION_REVIEW.md)
- [Phase-two synthesis and framework decision](docs/PHASE2_SYNTHESIS.md)
- [Working warrant framework](docs/FRAMEWORK.md)
- [OS reconstruction epistemological audit](docs/OS_RECONSTRUCTION_EPISTEMOLOGICAL_AUDIT.md)
- [OS reconstruction case study](docs/CASE_STUDY_OS_RECONSTRUCTION.md)
- [Literature review](docs/LITERATURE_REVIEW.md)
- [Novelty matrix](docs/NOVELTY_MATRIX.md)
- [Paper outline](docs/PAPER_OUTLINE.md)
- [Research decisions](docs/DECISIONS.md)
- [Next bounded task](docs/NEXT_TASK.md)
- [BibTeX](bibliography/references.bib)
- [Source register](provenance/SOURCE_REGISTER.csv)
- [Exact Lean environment pins](provenance/OS_RECONSTRUCTION_ENVIRONMENT.yaml)

## Phase-two conclusion

The general ideas of scientific representation, surrogate reasoning, mature mathematical formalisms, and cross-model transfer of empirical warrant are established in prior literature. In particular, Gelfert (2009, 2011) is a direct antecedent. The candidate contribution is narrower: analyze what machine-checked Demonstration adds within mature mathematical formalisms and what correspondence, instantiation, interpretation, and target-warrant obligations remain.

## Current status

The targeted literature comparison and OS source-critical epistemological audit are complete. The formalization-aware DDI framework is the working framework. Novelty remains carefully bounded; no priority claim is made.

The primary case is the public Lean formalization ecosystem for Osterwalder–Schrader axioms and reconstruction. Existing results are reused at exact commit pins. No new numerical computation or Lean build was performed in this research phase.

Substantive changes are submitted by pull request. No GitHub Actions workflow is required in this phase; validation is local/source-based.
