# Formalization Interfaces and Inter-Formalization Warrant

**Status:** Working analytical framework for the major manuscript revision. This is a case-based distinction, not a universal theory of scientific knowledge.

## 1. Central question

Under what conditions can a machine-checked theorem in one formalization support an inference in another formalization of the same physical theory?

The paper distinguishes the local deductive warrant of a checked theorem from the warrant required to transfer that result across formal representations. The latter is called **inter-formalization warrant**.

## 2. Five epistemic relations

1. **Local proof warrant.** A kernel checks that a proposition follows from definitions and assumptions in a specified formal system.
2. **Source-formalism correspondence.** The formal encoding adequately represents the mathematical objects, predicates, domains, and assumptions relevant to the source physical formalism.
3. **Inter-formalization warrant.** A verified interface relates the records and propositions of two formalizations, preserving the mathematical content needed for the inference.
4. **Model instantiation.** A concrete model is shown to satisfy every hypothesis of the theorem in the receiving formalization.
5. **Target-directed warrant.** Where a claim about a physical target is intended, the model-to-target inference is justified relative to the scientific purpose and relevant evidence.

These relations are distinguishable, not a mandatory linear sequence for every scientific claim. In particular, model-internal or modal knowledge need not culminate in a claim about an actual target.

## 3. Interface conditions

For a source formalization with theorem `Γ₁ ⊢ φ₁` and a receiving formalization with target theorem `Γ₂ ⊢ φ₂`, an interface adequate for theorem reuse must make explicit:

- **Object correspondence:** which source and receiving structures represent the same mathematical objects or related objects.
- **Predicate correspondence:** how the relevant definitions, assumptions, and properties are translated; whether the relation is equality, equivalence, implication, or a weaker map.
- **Hypothesis transport:** why the receiving assumptions suffice to establish the translated source hypotheses.
- **Conclusion and witness preservation:** why the source conclusion, including any reconstructed family or other witness, corresponds to the receiving conclusion.
- **Proof transport and checking:** how the source derivation is made available in the receiving system and what checking procedure validates the bridge and transported result.

The exact obligations depend on the intended inference. An isomorphism is not always required; a one-way implication or structure-preserving map may suffice. What matters is that the direction and strength of the correspondence are explicit and proved at the level required by the claim.

A schematic proof obligation is:

[
Gamma_1 dash_{mathcal L_1} arphi_1,
qquad
Gamma_2 dash_{mathcal L_2} 	au(Gamma_1),
qquad
Gamma_2 dash_{mathcal L_2} igl(	au(arphi_1)ightarrowarphi_2igr),
]

together with a proof-preserving interpretation (	au) between the relevant formal languages. This is an audit schema, not a universal sufficient-condition theorem for scientific knowledge.

## 4. Application to the OS formalization network

### OSforGFF

- Formalizes a massive Gaussian free field as a probability measure on (S'(mathbb R^D)).
- Uses the Glimm–Jaffe probability-measure and generating-functional formulation.
- Its OS1 is an exponential bound on the generating functional, with a subsidiary two-point condition; for the GFF the proof uses (p=2) and (c=1/(2m^2)).
- OS4 includes clustering and an ergodicity condition on a specified class of finite exponential functionals.
- The accompanying QFT paper explains the relationship of the Schwartz-space predicates to the Glimm–Jaffe compact-support formulation and explains the ergodicity argument. These are source-to-formalism correspondence claims; they should not be confused with a formal bridge into OSreconstruction.

### OSreconstruction

- Takes Schwinger distributions on the zero-diagonal Schwartz test-function space.
- Its forward theorem requires E0–E4 and an arity-dependent growth condition.
- The OS-II original-coordinate growth condition is converted by a proved theorem into the arity-linear record used by the public forward theorem.
- The output is a Wightman-function distribution family; GNS/operator reconstruction is outside the package endpoint.

### Comparator

- The Mathlib-only challenge reproduces verbatim the package's own audit definitions and adds three theorem obligations; it is independent at the import/checking boundary, not in authorship or mathematical origin.
- The bridge code converts the challenge OS record to and from the production record, preserves the Schwinger family, transfers the growth records, and identifies the Wick-pairing and output-growth predicates.
- The solution proves equivalences between the challenge propositions and production specifications; Comparator and NanoDa provide additional structural and proof replay checks.
- This is a positive, formally checked instance of inter-formalization warrant, not a second independent derivation.

### OSforGFF to OSreconstruction

The public pinned artifacts do not expose an end-to-end theorem that takes the specific OSforGFF probability-measure construction and instantiates the exact zero-diagonal OS record and arity-dependent growth condition required by OSreconstruction. The projects use different formal records and test-function domains. OSreconstruction reports relevant inhabitants in a private companion development, but that does not establish identity with the pinned OSforGFF object or provide a publicly inspectable bridge.

## 5. Relation to existing philosophy

- **Hughes (1997):** DDI remains a useful organizing distinction, but machine-checked proof is only one formalized component of Demonstration.
- **Gelfert (2011, 2022):** mature mathematical formalisms are heterogeneous inferential and interpretative resources; the framework should not reduce them to a single representational mapping.
- **DeDeo and Duede (2026):** adequate representation and tracking constrain correspondence between informal proofs and formal derivations. The present case adds the distinct issue of correspondence between formal representations.
- **Rabe (2017):** theory morphisms are compositional translations that preserve judgments and induce model reduction. The paper does not claim this formal mechanism as new; it asks about its epistemic adequacy when applied to physical formalisms.
- **Al Wardani et al. (2023):** DAMF addresses provenance, trust, and exchange of formal assertions across heterogeneous proof systems.
- **Guilloud et al. (2025):** SC-TPTP addresses proof-certificate exchange and reconstruction across ATPs and ITPs, including Lean.
- **Bobbin et al. (2024):** interoperable scientific structures and proof reuse are established; the present paper analyzes the epistemic conditions for warrant transfer across formal records.
- **Gelfert (2009):** empirical warrant can transfer between physical models through rigorous mathematical relations. Inter-formalization warrant concerns a prior formal interface and does not itself supply empirical warrant.
- **Meadows et al. (2026):** semantic drift in autoformalization is an established problem; it motivates attention to source-formalism correspondence but is not the paper's novelty.

## 6. Bounded contribution

The paper offers a source-critical, case-based analysis of inter-formalization warrant in mathematical physics. It does not claim a new general theory of scientific representation, a new theorem about OS reconstruction, a new account of proof interoperability, or a new theory of cross-model empirical warrant.
