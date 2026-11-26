# Formalization-Aware DDI Framework (v0.2)

**Status:** Working framework selected after the phase-two literature comparison. Not yet frozen for the manuscript.

## 1. Organizing idea

Use Hughes's Denotation–Demonstration–Interpretation (DDI) structure as the organizing skeleton, but make explicit the role of machine formalization within Demonstration and the interfaces that remain outside kernel checking.

This is not a new general theory of scientific representation. It is an analysis of how machine-checked proof changes the epistemic status of demonstration within mature mathematical formalisms in theoretical physics.

## 2. Mature physical mathematical formalism

Let F_phys denote a mature mathematical formalism used in physics: a physically interpreted notation system with locally applicable rules, conventions, and theoretical/methodological commitments.

Examples include operator formalism, Feynman diagrams, and Euclidean field-theory structures. Following Gelfert (2011, 2022), such formalisms are not neutral containers: they provide inferential and interpretative resources and shape scientific practice.

A Lean formalization is a selective re-articulation of some part of F_phys. It need not encode the entire formalism or all of its tacit conventions.

## 3. Formalization correspondence

Let L be the proof-assistant language and let tau denote the formalization map from the relevant part of F_phys into L.

The formalization must preserve, for the claim at issue:
- mathematical objects and their types;
- operations and locally applicable rules;
- domains, boundary conditions, and side assumptions;
- the exact theorem statement and its quantifiers;
- the physical interpretation intended for the encoded objects.

This is a correspondence question. DeDeo and Duede's adequate-representation and tracking criteria, and FormalScience's semantic-drift analysis, are important prior constraints. They are not claimed as new contributions here.

## 4. Machine-checked Demonstration

For assumptions Gamma and proposition phi, a proof assistant checks:

$$
\Gamma \vdash_{\mathcal L} \varphi.
$$

This establishes formal derivability relative to the declared language, assumptions, definitions, imports, kernel, and trust base. It does not alone establish that the formalization faithfully captures the source physical formalism or that the formal symbols have the intended physical interpretation.

The machine-checking contribution is therefore local but significant: it strengthens the reliability and auditability of the formal derivation.

## 5. Model interpretation and instantiation

Let M be a specified mathematical/physical model. To obtain a model-internal claim from the formal theorem, one must establish:
1. correspondence between the formal statement and the intended model statement;
2. correct interpretation of formal objects and predicates in M;
3. satisfaction by M of every theorem hypothesis, including regularity, growth, domain, and boundary assumptions.

The resulting claim is model-internal:

$$
\mathcal M \models \varphi^*.
$$

This step is not automatic from kernel acceptance.

## 6. Target-directed inference and model evaluation

Let T be an intended physical target and P a scientific purpose. A claim about T requires an appropriate model-to-target relation and a justified inference from the model result to the target.

Relevant prior frameworks include:
- Suárez and Contessa on surrogate reasoning;
- Frigg and Nguyen's DEKI account, especially keying and imputation;
- Gelfert's account of cross-model warrant transfer;
- Parker's adequacy-for-purpose view.

A formal proof may certify a mathematical mapping between models. It does not by itself establish that the mapping preserves the physically relevant properties, that the source model is empirically supported, or that the target model is adequate for P.

Gelfert (2009) is decisive here: rigorous mathematical relations may transmit empirical warrant between models, but they do not create empirical warrant from scratch.

Model evaluation is purpose-sensitive. Parker's problem space includes target, user, methodology, circumstances, and goal. A theorem may be adequate for a mathematical or structural purpose without being sufficient for prediction or empirical application.

## 7. Modal and exploratory knowledge

Not every model use aims at a claim about an actual target. Following Knuuttila (2021), models can be epistemic artifacts used to explore possible mechanisms and modal structures.

Thus target-directed warrant is one possible endpoint, not a mandatory final stage for every formalized model.

## 8. Claim taxonomy

- **C_F — formal derivability:** Gamma entails phi in the declared formal system.
- **C_M — model-internal claim:** the interpreted proposition holds in a specified model, with all hypotheses instantiated.
- **C_T — target-directed claim:** a claim about an intended physical system is warranted through appropriate model-based inference and evidence.
- **C_E — explanatory understanding:** an orthogonal epistemic aim; a proof may establish a theorem without supplying the relevant physical explanation.

Modal/exploratory model knowledge may be epistemically valuable even when no C_T claim is intended.

## 9. Conditional audit schema

For a target-directed claim, the following components should be audited:

$$
V_F \land C_{form} \land A_M \land I_M \land R_{MT}(P) \land E_P
$$

where:
- V_F: formal proof validity under the declared trust base;
- C_form: adequate correspondence between the source physical formalism and the formalized statement;
- A_M: satisfaction of all theorem hypotheses by model M;
- I_M: correct physical interpretation of the formal objects and predicates;
- R_MT(P): an appropriate model-to-target relation for purpose P;
- E_P: evidence appropriate to the target and purpose.

This is a diagnostic schema, not a universal sufficient-condition theorem. Which components are required depends on the kind of claim being made.

## 10. Application to the OS case

The OS case distinguishes:
1. proof of OS properties for a concrete Euclidean free-field model;
2. a separate conditional OS-to-Wightman reconstruction theorem requiring an arity-dependent growth condition;
3. the instantiation of that exact growth condition by the concrete model;
4. physical interpretation and target-directed use of the reconstructed objects.

The public repositories inspected do not expose a single end-to-end theorem instantiating the exact reconstruction growth hypothesis from OSforGFF. OS1 regularity must not be identified with that condition without a proved bridge.

## 11. Scope discipline

The paper does not propose a universal theory of all AI-generated scientific knowledge, a new general representation theory, or a new theory of cross-model empirical warrant. Its contribution is a formalization-aware analysis of the Demonstration component and its interfaces in theoretical physics.
