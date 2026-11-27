# Literature Review (updated 2026-11-26)

This repository now separates the first-pass review of formal proof and computational science from the phase-two review of scientific representation and model-based reasoning.

## 1. Machine-checked proof and mathematical knowledge

- **Duede & Davey (2025),** “A Priori Knowledge in an Era of Computational Opacity: The Role of Artificial Intelligence in Mathematical Discovery,” Philosophy of Science 92(5), 1394–1404, DOI 10.1017/psa.2025.10160. They argue that a transparent proof-checker can support a priori mathematical knowledge even when a proof-generating system is opaque. They explicitly leave open the extension to scientific knowledge beyond mathematics.
- **DeDeo & Duede (2026),** “A Correspondence Problem for Mathematical Proof,” Philosophy of Science, forthcoming; arXiv:2603.13680v2. They distinguish adequate representation of the theorem from tracking the original proof's inferential steps.
- **Meadows, Zhang & Freitas (2026),** “FormalScience,” ACL 2026, 23059–23077, DOI 10.18653/v1/2026.acl-long.1057. They develop human-in-the-loop physics autoformalization and study semantic alignment and semantic drift.
- **Imbert & Ardourel (2023),** “Formal Verification, Scientific Code, and the Epistemological Heterogeneity of Computational Science,” Philosophy of Science 90(2), 376–394, DOI 10.1017/psa.2022.78.

## 2. Formalization of scientific theories

- **Bobbin et al. (2024),** “Formalizing Chemical Physics Using the Lean Theorem Prover,” Digital Discovery 3, 264–280, DOI 10.1039/D3DD00077J.
- **Douglas et al. (2026),** “Formalization of QFT,” arXiv:2603.15770v1.
- Public OS formalization artifacts are analyzed at exact commits in CASE_STUDY_OS_RECONSTRUCTION.md.

## 3. Scientific representation and model-based reasoning

The detailed comparative review is in [MODEL_REPRESENTATION_REVIEW.md](MODEL_REPRESENTATION_REVIEW.md). The most relevant primary sources are:

- **Hughes (1997),** “Models and Representation,” Philosophy of Science 64, Supplement, S325–S336, DOI 10.1086/392611. DDI: Denotation, Demonstration, Interpretation.
- **Giere (2004),** “How Models Are Used to Represent Reality,” Philosophy of Science 71(5), 742–752, DOI 10.1086/425063. Pragmatic, purpose-sensitive similarity.
- **Suárez (2004),** “An Inferential Conception of Scientific Representation,” Philosophy of Science 71(5), 767–779, DOI 10.1086/421415. Directionality and surrogate inference.
- **Contessa (2007),** “Scientific Representation, Interpretation, and Surrogative Reasoning,” Philosophy of Science 74(1), 48–68, DOI 10.1086/519478. Valid surrogate inference need not be sound.
- **Frigg & Nguyen (2018),** “The Turn of the Valve: Representing with Material Models,” European Journal for Philosophy of Science 8, 205–224, DOI 10.1007/s13194-017-0182-4. DEKI: denotation, exemplification, keying, imputation.
- **Morrison & Morgan (1999),** “Models as Mediating Instruments,” DOI 10.1017/CBO9780511660108.003. Models as relatively autonomous instruments of investigation.
- **Knuuttila (2021),** “Epistemic Artifacts and the Modal Dimension of Modeling,” European Journal for Philosophy of Science 11, 65, DOI 10.1007/s13194-021-00374-5.
- **Parker (2020),** “Model Evaluation: An Adequacy-for-Purpose View,” Philosophy of Science 87(3), 457–477, DOI 10.1086/708691.

## 4. Direct antecedents for mathematical formalism and warrant transfer

Two Gelfert papers materially change the novelty assessment:

- **Gelfert (2009),** “Rigorous Results, Cross-Model Justification, and the Transfer of Empirical Warrant,” Synthese 169, 497–519, DOI 10.1007/s11229-008-9431-6. This explicitly argues that mathematically rigorous relations can transmit empirical warrant between models, illustrated by Hubbard–Heisenberg models and the Mott transition. We cannot claim this general idea as new.
- **Gelfert (2011),** “Mathematical Formalisms in Scientific Practice: From Denotation to Model-Based Representation,” Studies in History and Philosophy of Science Part A 42(2), 272–286, DOI 10.1016/j.shpsa.2010.11.035. This develops mature mathematical formalisms as physically interpreted systems of locally applicable rules and inferential/interpretative resources. It is a direct antecedent for our focus on formalized physical mathematics.
- **Gelfert (2022),** “Thinking with Notations: Epistemic Actions and Epistemic Activities in Mathematical Practice,” DOI 10.1007/978-3-030-97833-4_11. Notations and formalisms shape mathematical practice rather than merely expressing pre-existing concepts.
- **Cartwright (1999),** “Models and the Limits of Theory: Quantum Hamiltonians and the BCS Models of Superconductivity,” DOI 10.1017/CBO9780511660108.010.
- **Hartmann (1999),** “Models and Stories in Hadron Physics,” DOI 10.1017/CBO9780511660108.012.

## 5. Revised synthesis

The literature already contains general accounts of scientific representation, surrogate inference, mature mathematical formalisms, and cross-model empirical-warrant transfer. The candidate contribution is narrower: a formalization-aware analysis of the epistemic role of machine-checked Demonstration within mature mathematical formalisms in theoretical physics, including the distinct correspondence, instantiation, interpretation, and target-warrant obligations.

This is a targeted review, not a systematic review or a basis for a priority claim.
