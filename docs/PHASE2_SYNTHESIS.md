# Phase 2 Synthesis and Framework Decision

**Date:** 2026-11-26  
**Status:** Completed targeted literature comparison; framework selected as working framework, not yet manuscript-frozen.

## 1. Main finding

The broad initial novelty claim is not tenable. Scientific philosophy already contains:
- accounts of scientific representation and surrogate reasoning (Giere, Hughes, Suárez, Contessa, Frigg–Nguyen);
- theories of models as mediators and epistemic artifacts (Morgan–Morrison, Knuuttila);
- an explicit account of rigorous mathematical relations transmitting empirical warrant across physical models (Gelfert 2009);
- an account of mature mathematical formalisms as inferential and interpretative resources (Gelfert 2011);
- an account of notations/formalisms as epistemic actions that shape mathematical practice (Gelfert 2022);
- purpose-relative model evaluation (Parker 2020).

We must not claim any of these ideas as new.

## 2. Framework decision

Adopt a **formalization-aware DDI framework** as the working analytical framework.

The DDI structure (Denotation, Demonstration, Interpretation) remains the organizing skeleton. The contribution is to specify how machine formalization and kernel checking enter the Demonstration component, while preserving the distinct obligations of formalization fidelity and model-to-target interpretation.

### Layer 1: Mature physical mathematical formalism
A physically interpreted notation system with local rules, conventions, and theoretical/methodological commitments (Gelfert 2011). Examples include operator formalism, Feynman diagrams, and Euclidean QFT structures.

### Layer 2: Formalization correspondence
A selective translation from the source physical formalism into a proof-assistant language. The mapping must preserve the relevant objects, operations, assumptions, domains, and theorem statements. DeDeo–Duede's representation/tracking criteria and FormalScience's semantic-drift analysis are prior constraints, not new contributions.

### Layer 3: Machine-checked demonstration
A kernel-accepted derivation:
$$
\Gamma \vdash_{\mathcal L} \varphi.
$$
This establishes formal derivability relative to the declared language, assumptions, imports, and trust base. It does not alone establish the physical interpretation of the symbols or the adequacy of the source formalism.

### Layer 4: Model interpretation and instantiation
To obtain a model-internal claim, the formal statement must be interpreted and all theorem hypotheses must be instantiated by the concrete model.

### Layer 5: Target-directed inference and purpose-sensitive evaluation
To infer a claim about a target, the model must support appropriate denotation, keying/imputation, and surrogate inference. The inference must be assessed for soundness and adequacy relative to the target, user, method, circumstances, and purpose.

Gelfert 2009 adds an important qualification: mathematically rigorous relations can transmit empirical warrant across models when an empirically supported source model is linked to a target model by a physically relevant relation. A proof assistant may certify the mathematical relation; it does not create empirical warrant from scratch or establish the physical relevance of the mapping.

## 3. Claim taxonomy revision

Retain three principal claim types:
- **C_F — formal derivability:** a proposition follows in the declared formal system.
- **C_M — model-internal claim:** the interpreted proposition holds in a specified model, with hypotheses instantiated.
- **C_T — target-directed claim:** a claim about a physical target is warranted through model-based inference and purpose-appropriate evidence.

Keep **C_E — explanatory understanding** as an orthogonal epistemic aim, not a mandatory fourth stage. A proof may establish a theorem without providing the relevant physical explanation.

Also allow **modal/exploratory model knowledge** where no actual target is intended (Knuuttila 2021). Target-world transfer is not compulsory for every scientific use of a model.

## 4. Candidate contribution

The paper's candidate contribution is:

**A formalization-aware analysis of the epistemic role of machine-checked demonstration within mature mathematical formalisms in theoretical physics, clarifying which warrants are strengthened by kernel checking and which remain dependent on interpretation, model construction, and target-directed inference.**

The novelty claim remains provisional. The paper must be positioned as an extension/application of existing frameworks, not as a new general theory of scientific representation or cross-model warrant.

## 5. Paper title and scope

Working title:

**Machine-Checked Proofs and Mature Mathematical Formalisms in Physics: The Epistemology of Formalized Osterwalder–Schrader Reconstruction**

Primary case: OSforGFF, OSreconstruction, and the Comparator audit surface. Gelfert's Hubbard–Heisenberg example is the comparison case for cross-model warrant. Feynman diagrams/operator formalism provide a bounded example of mature physical formalisms.

## 6. Why the OS case remains suitable

The OS formalizations expose distinct interfaces:
- a concrete Gaussian free field satisfying OS axioms;
- a separate conditional reconstruction theorem requiring an arity-dependent growth condition;
- a Comparator audit of the theorem statement and proof interface;
- a nontrivial boundary between Wightman distributions and full GNS/operator reconstruction.

The public packages inspected do not show an end-to-end instantiation of the exact reconstruction growth hypothesis from OSforGFF. This is an explicit technical boundary, not a physical error and not evidence that the two developments cannot be connected.

## 7. Acceptance status

Phase 2 passes its planned criteria:
- core representation and model-reasoning accounts compared;
- Gelfert 2009 and 2011 identified as direct antecedents;
- novelty claim narrowed;
- framework revised to formalization-aware DDI;
- C_E moved out of the serial warrant chain;
- target-world warrant made purpose-sensitive and non-mandatory for modal/exploratory model uses.

No new numerical computation or Lean build was required or performed.
