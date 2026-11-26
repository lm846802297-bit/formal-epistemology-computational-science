# Formal Epistemology of Computational Science

**Working paper:** *What Does a Machine-Checked Proof Establish in Physics? The Epistemology of Formalized Osterwalder-Schrader Reconstruction*

**Question:** Under what conditions can a machine-checked theorem about a formalized physical theory warrant a claim about a physical system?

## Provisional thesis
A proof assistant supplies conditional deductive warrant for a proposition in a specified formal system, relative to its assumptions and trust base. It does not by itself establish that the proposition captures the intended physical statement, that a concrete model satisfies every theorem hypothesis, or that the model's conclusions apply to a physical target.

We distinguish **C_F** (formal claim), **C_M** (model-internal claim), **C_W** (target-world claim), and **C_E** (explanatory claim). The primary case is public Lean formalizations of the Osterwalder-Schrader axioms and reconstruction theorem. Lean chemical-physics formalization is a secondary comparison. The axial Ward identity/anomaly is a bounded physics stress test, not a claim of existing Lean formalization.

## Repository map
- [Research charter](docs/RESEARCH_CHARTER.md)
- [Literature review](docs/LITERATURE_REVIEW.md)
- [Warrant framework](docs/FRAMEWORK.md)
- [OS reconstruction case study](docs/CASE_STUDY_OS_RECONSTRUCTION.md)
- [Novelty matrix](docs/NOVELTY_MATRIX.md)
- [Paper outline](docs/PAPER_OUTLINE.md)
- [Research decisions](docs/DECISIONS.md)
- [Next task](docs/NEXT_TASK.md)
- [BibTeX](bibliography/references.bib)
- [Source register](provenance/SOURCE_REGISTER.csv)
- [Exact Lean environment pins](provenance/OS_RECONSTRUCTION_ENVIRONMENT.yaml)

## Status
Initial literature review and framework design. Novelty remains provisional; no priority claim is made. No new numerical computation or Lean build was performed. Existing public results are reused at exact commit pins.

## Acceptance criteria
1. Closest prior work accurately classified by publication status.
2. No novelty claim for semantic translation, proof correspondence, proof tracking, or model validation in isolation.
3. Four claim types precise and non-redundant.
4. Warrant-transfer account is conditional and claim-sensitive.
5. OS case accurately records hypotheses, endpoints, toolchains, and composition boundaries.
6. Axial anomaly example checked against primary physics sources before final use.

Substantive changes are submitted by pull request. No GitHub Actions workflow is required in this phase; validation is local.