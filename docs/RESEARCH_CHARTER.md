# Research Charter (updated 2026-11-26)

## Research question

What epistemic role does machine-checked formalization play within mature mathematical formalisms in theoretical physics, and what does it add to the demonstration of model-internal results?

## Provisional thesis

Machine checking strengthens the reliability and auditability of formal derivations. Its epistemic contribution is local to the declared formal system, assumptions, definitions, imports, kernel, and trust base. Scientific warrant also depends on correspondence between the source physical formalism and its formal encoding, concrete instantiation of theorem hypotheses, physical interpretation, and (when a target-directed claim is intended) a purpose-appropriate model-to-target inference.

## Framework

Use a **formalization-aware DDI framework**:
- Denotation: the model's representational relation to its intended target.
- Demonstration: derivation within the model; formalization fidelity and machine checking specify this component.
- Interpretation: use of model results to draw claims about the target.

The DDI structure is supplemented by mature mathematical formalism (Gelfert), surrogate reasoning and DEKI, cross-model warrant transfer (Gelfert 2009), and adequacy-for-purpose (Parker).

This is not a new general theory of representation. It is a formalization-aware analysis of the role of machine-checked demonstration in mathematical physics.

## Claim types

- C_F: formal derivability in the declared system.
- C_M: interpreted model-internal claim with all hypotheses instantiated.
- C_T: target-directed claim warranted through model-based inference and evidence.
- C_E: explanatory understanding, orthogonal to the serial warrant path.
- Modal/exploratory model knowledge is permitted without an actual target.

## Primary case

Public Lean formalizations of OSforGFF, OSreconstruction, and the Comparator audit surface, at exact commits recorded in provenance/OS_RECONSTRUCTION_ENVIRONMENT.yaml.

## Comparison cases

- Gelfert's Hubbard–Heisenberg relation and Mott transition for cross-model empirical-warrant transfer.
- Operator formalism/Feynman diagrams as mature physical formalisms.
- Bobbin et al. (2024) as a secondary formalization of scientific derivations.
- Axial Ward identity/anomaly as a bounded physics stress test only after primary-source convention checking.

## Out of scope

A universal theory of AI-generated science; a new general account of scientific representation; a new general theory of cross-model empirical warrant; a full Lean implementation of QFT or the anomaly; a broad survey of all model-based reasoning.

## Phase-two result

The broad initial novelty claim has been narrowed. Gelfert (2009, 2011) are direct antecedents. The candidate contribution concerns the epistemic role of machine-checked Demonstration within mature mathematical formalisms and its interfaces with formalization correspondence, model instantiation, interpretation, and target-directed inference.
