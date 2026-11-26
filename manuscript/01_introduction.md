# 1. Introduction

## 1.1. Machine-checked proof and the epistemology of physics

Proof assistants are increasingly used to formalize mathematical results that enter scientific theories. In mathematical physics, this development is especially significant. Physical theories are not expressed only in ordinary prose or in isolated equations: they rely on mature mathematical formalisms whose symbols, operations, admissible transformations, and interpretative conventions have been developed through sustained scientific practice. Operator methods, distribution theory, Euclidean field theory, and diagrammatic techniques are examples of formalisms that function both as mathematical languages and as resources for scientific reasoning (Gelfert 2011, 2022).

A proof assistant such as Lean can check that a proposition follows from specified definitions and assumptions in a formal system. This is a substantial epistemic achievement. It makes the inferential content of a derivation explicit, exposes assumptions that might otherwise remain implicit, and allows the proof object to be checked by a small trusted kernel. The formal turn in mathematics has made clear that such systems can strengthen the reliability and auditability of deductive reasoning (Avigad 2024). Recent discussions of AI-assisted mathematical discovery likewise argue that transparent proof checking can provide a route from computationally opaque discovery procedures to warranted mathematical knowledge (Duede and Davey 2025).

The epistemological question in physics, however, is not exhausted by asking whether a formal proof is valid. A mathematical theorem is a theorem about the objects and assumptions specified in its formal statement. A scientific claim concerns a physical model, a theoretical structure, or an intended target system. Moving from the former to the latter requires an account of how the formal objects are related to the physical formalism, how the hypotheses apply to the model under consideration, and how the model is used to draw conclusions about the physical world.

This paper examines that transition. Its central question is:

> What does a machine-checked proof establish when the formal system being checked is itself a selective formalization of a mature mathematical formalism used in physics?

The question is deliberately narrower than a general epistemology of artificial intelligence or computational science. It concerns the epistemic role of machine-checked demonstration within mathematical physics, and the additional relations required when a result is interpreted as a claim about a physical model or its target.

## 1.2. Scientific models, mathematical formalisms, and proof

The philosophy of science has long distinguished the internal manipulation of a model from the use of that model to reason about a target. Hughes's DDI account separates denotation, demonstration, and interpretation: a model denotes a target, supports reasoning within the model, and is interpreted so that model results can inform claims about the target (Hughes 1997). Other accounts emphasize the pragmatic and purpose-sensitive character of representation (Giere 2004), the inferential capacities of models (Suárez 2004), and the role of interpretation in surrogate reasoning (Contessa 2007). The DEKI account makes the mapping from model properties to target properties explicit through denotation, exemplification, keying, and imputation (Frigg and Nguyen 2018).

These accounts show why a formally valid derivation need not, by itself, establish a true claim about a target. A model may support a valid inference while the inference is not sound for the intended target; the model may represent only selected aspects of a system; and the relation between a mathematical property and a physical property may require a substantive interpretation. Model evaluation is also purpose-relative: the adequacy of a model depends on its target, the methods by which it is used, the circumstances of use, and the scientific goal (Parker 2020).

A further complication arises because mathematical formalisms in physics are not neutral containers for equations. Gelfert describes mature mathematical formalisms as systems of notation and locally applicable rules that carry theoretical and methodological commitments while providing inferential and interpretative resources (Gelfert 2011). The formalism shapes what can be derived and how the derivation is understood. Translating part of such a formalism into a proof assistant is therefore not simply copying a proof into a different notation. It is a selective re-articulation of the mathematical structures, operations, domains, and assumptions that the formalization makes explicit.

The present paper brings these two discussions together. It asks how machine checking changes the epistemic status of the demonstration component in a model-based scientific practice. The aim is not to propose a new general theory of scientific representation. Rather, the DDI structure is used as an established analytical framework, while the formalization and machine checking of demonstration are examined as a specific development within mathematical physics.

## 1.3. What existing work has established

Several adjacent literatures already address important parts of this problem. Work on proof correspondence distinguishes the adequacy of a formal statement as a representation of an informal theorem from the extent to which a formal proof tracks the original reasoning (DeDeo and Duede 2026). Research on physics autoformalization identifies semantic drift that can arise when scientific statements are translated into formal languages (Meadows, Zhang, and Freitas 2026). The epistemology of formal verification in computational science also emphasizes that verification practices have heterogeneous roles and do not replace every other form of scientific assessment (Imbert and Ardourel 2023).

The philosophy of scientific models has addressed the relation between model reasoning and target-directed inference. Particularly relevant to the present case, Gelfert (2009) argues that mathematically rigorous relations can transmit empirical warrant between physical models. Gelfert (2011) further analyzes the role of mature mathematical formalisms in scientific practice. These results rule out any claim that the general ideas of model-based inference, mathematical warrant transfer, or mature mathematical formalisms are new contributions of this paper.

The more specific question considered here is what machine checking adds to the demonstration performed within such a formalism, and what it leaves untouched. A checked proof may strengthen confidence that a specified mathematical consequence follows from specified assumptions. It does not, solely by being checked, establish that the formalization preserves all scientifically relevant features of the source formalism, that a concrete model satisfies every hypothesis, or that the model is adequate for a particular physical purpose. These are distinct epistemic tasks.

## 1.4. The Osterwalder–Schrader case

The paper develops this analysis through recent Lean formalizations related to the Osterwalder–Schrader (OS) framework. The case is useful because it contains three distinct public artifacts.

First, OSforGFF constructs the massive Gaussian free field as a probability measure on a space of tempered distributions and formalizes the satisfaction of the project's OS0–OS4 properties. Its master theorem is stated for spacetime dimension D greater than or equal to two, with a dimension-generic construction and explicit propagator instances (OSforGFF, commit fef84a82937dfd2bb7f672108a72da329d3ef0fd).

Second, OSreconstruction formalizes conditional reconstruction results between Euclidean Schwinger-function data and relativistic Wightman-function distributions. Its forward theorem requires the OS E0–E4 assumptions together with a separate arity-dependent growth condition. The OS-II version adds an output growth bound and uniqueness among Wick-paired Wightman families. The package's stated endpoint is a family of Wightman distributions, not a full GNS construction of a Hilbert space and operator-valued fields (OSreconstruction, commit cf0904e34a7c146a9f312f601e3707dca4a87697).

Third, OSreconstruction-comparator provides a Mathlib-only challenge specification and a solution discharged from the production package, together with Comparator and NanoDa checking. It supplies an additional formal statement and proof-checking interface. It is not a second independent mathematical derivation by another research team, and it does not provide empirical validation (OSreconstruction-comparator, commit 93cdb40e728ba27b7b1b55efc30d57f7b43de9aa).

The three projects do not, in their inspected public interfaces, form one end-to-end formal proof that the particular OSforGFF model satisfies the exact growth input required by the separate OSreconstruction package. This is not a claim that no such inhabitant exists: the OSreconstruction README reports examples in a private companion development, which is not independently inspectable here. The point is that the public artifacts expose distinct theorem statements, assumptions, formal records, and dependency environments. Their relation must therefore be analyzed rather than presumed.

The original OS programme also matters. The 1973 paper introduced the axiomatic relation between Euclidean Green functions and Wightman theories; the 1975 sequel explicitly extended and corrected the earlier reconstruction result by introducing an additional growth condition. Any account of the forward reconstruction theorem must include this correction (Osterwalder and Schrader 1973, 1975).

## 1.5. Approach and contribution

The method is a source-critical conceptual case study. It examines the exact theorem statements, assumptions, output structures, and repository records of the three public formalization projects at fixed commits, and relates them to the original OS papers and the philosophy of scientific representation. No new Lean implementation, numerical calculation, or independent proof replay is undertaken. Claims about machine checking are attributed to the specified artifacts and their authors' reported verification procedures.

The paper makes three connected claims.

First, machine checking strengthens the epistemic status of mathematical demonstration by making the formal assumptions and inferential steps explicit and subjecting the proof object to kernel checking. The warrant is conditional on the formal system, its definitions, imports, axioms, and trust base.

Second, this strengthened demonstration does not automatically transfer to a claim about a concrete physical model. Such a transfer requires correspondence between the source physical formalism and its encoding, correct interpretation of the formal objects, and instantiation of every theorem hypothesis by the model under consideration.

Third, even a warranted model-internal result does not by itself establish the empirical adequacy of the model for a target system. Target-directed claims require a further account of the model-to-target relation and of the purpose for which the model is used. In some scientific contexts, however, a model may also provide mathematical or modal knowledge without being used to describe a particular actual target (Knuuttila 2021).

The contribution is thus a formalization-aware analysis of the demonstration component in mathematical physics, not a new general theory of scientific representation or cross-model empirical warrant. The OS case makes the relevant interfaces concrete: a model satisfying OS properties, a conditional reconstruction theorem with a quantitative growth premise, a separate proof-checking interface, and the physical interpretation of the resulting Wightman-function data.

The paper proceeds as follows. Section 2 analyzes the OS formalizations and distinguishes what each artifact establishes. Section 3 discusses the epistemic contribution and limits of machine-checked demonstration within mature mathematical formalisms, using the case to clarify the relations between formal derivability, model-internal knowledge, and target-directed scientific claims.
