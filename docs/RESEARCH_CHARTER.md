# Research Charter

## Question
Under what conditions can a machine-checked theorem about a formalized physical theory warrant a claim about a physical system?

## Provisional thesis
Machine checking supplies conditional deductive warrant for a formal proposition, relative to a specified formal system, kernel, axioms, definitions, imports, and trust base. Transfer to a scientific claim requires distinct relations:

1. **Formal validity:** acceptance of the proof object by the declared system.
2. **Theorem correspondence:** adequate representation of the intended mathematical/scientific statement. If the claim concerns the original proof's reasoning, tracking its inferential steps is an additional requirement.
3. **Assumption instantiation:** the concrete model satisfies every theorem hypothesis, including growth, regularity, boundary, and domain conditions.
4. **Physical interpretation:** formal objects are correctly interpreted as fields, states, operators, observables, symmetries, and constraints.
5. **Model-to-target warrant:** the model is appropriate for target, purpose, and domain. This may be representational, inferential, idealized, or modal; literal isomorphism is not assumed.
6. **Empirical/domain evidence:** claims about actual physical systems require evidence appropriate to the system and regime.

These are diagnostic conditions, not a theorem that their conjunction is universally sufficient.

## Claim types
Let F be a formal system, A its assumptions, phi a formal proposition, M a mathematical/physical model, and W an intended physical target:
- C_F: A |-F phi.
- C_M: the interpreted proposition holds in M.
- C_W: the property is warranted for W in domain D.
- C_E: the derivation explains why the result holds.

C_E is not reducible to C_F: a proof may establish a theorem without preserving explanatory structure.

## Candidate contribution
A typed, physics-specific account of warrant transfer integrating proof correspondence, theorem-hypothesis instantiation, physical interpretation, and purpose-sensitive model-to-target relations. This is an integration and extension, not an invention of these individual distinctions.

## Case strategy
Primary: public OSforGFF, OSreconstruction, and OSreconstruction-comparator repositories at exact commits. Secondary: Bobbin et al. (2024). Bounded stress test: classical versus quantum axial Ward identities and anomaly, after primary-source checking. No claim that cited Lean projects formalize the anomaly.

## Out of scope
Universal epistemology of all AI science; comprehensive numerical-simulation epistemology; full Lean formalization of QFT/anomaly; re-deriving OS formalizations; duplicating DeDeo and Duede's proof-correspondence account.

## Phase-one acceptance
Closest prior work accurately classified; novelty distinguished from prior correspondence and semantic-drift work; claim types precise; OS case technically accurate; anomaly example physically checked. No numerical convergence analysis is applicable because no numerical computation is in scope.