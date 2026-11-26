# 3. Discussion: The Epistemic Role of Machine-Checked Demonstration in Physics

## 3.1. The local strength of machine checking

The OS case supports a positive but carefully delimited assessment of machine-checked proof. A proof assistant does not merely provide another informal endorsement of a derivation. It checks a proof object against a formal proposition in a specified environment. When the definitions, assumptions, imports, and foundational trust base are made explicit, the result is a highly auditable form of deductive warrant.

This warrant is local in a precise sense. If a Lean kernel accepts a proof of

\[
\Gamma \vdash_{\mathcal L} \varphi,
\]

then, relative to the soundness of the formal system and its declared trust base, the proposition \(\varphi\) follows from the assumptions \(\Gamma\) as represented in the language \(\mathcal L\). The acceptance does not independently establish that \(\Gamma\) expresses the intended physical assumptions, that \(\varphi\) captures the intended scientific conclusion, or that the formal objects have the intended physical interpretation.

This qualification does not weaken the mathematical result. It identifies what the proof-checking procedure is designed to warrant. The distinction is especially important when a proof assistant is used to formalize a mature physical formalism rather than a self-contained mathematical exercise.

The Comparator layer in the OS case illustrates a further benefit. An independently stated Mathlib-only challenge makes the target propositions explicit outside the production package, while the Comparator and NanoDa workflow provide an additional proof-checking and replay interface. This increases auditability of the formal theorem statements and their proofs. It does not convert the result into an empirical test, nor does it establish that the physical interpretation of the formalism is correct.

## 3.2. Formalization is a selective re-articulation of a mature formalism

A mature mathematical formalism in physics is more than a set of equations. It includes notational conventions, locally applicable rules, domain restrictions, interpretative practices, and theoretical commitments. Such formalisms guide what physicists can infer and how mathematical operations are understood in physical terms (Gelfert 2011, 2022).

Formalization in a proof assistant therefore involves a selection. Some structures and rules are made explicit as definitions and theorems; others may remain in explanatory prose, be represented through external assumptions, or be omitted from the formal development. This is not necessarily a flaw. Any formalization has a scope. The epistemic task is to identify that scope accurately.

The OS case provides a concrete example. OSforGFF formalizes a probability-measure and generating-functional construction. OSreconstruction formalizes Euclidean Schwinger data on a zero-diagonal Schwartz test space and a Wightman-function output on full Schwartz space. Both are connected to the OS programme, but their formal records are not identical. Their different dimension conventions and dependency environments also matter when one asks whether a theorem from one project can be used as an input to another.

The distinction between OSforGFF's OS1 regularity and OSreconstruction's arity-dependent OS-II growth condition is particularly instructive. Both concern regularity or growth, but they are different formal predicates with different mathematical roles. The fact that both are described using familiar OS terminology does not license an inference from one to the other. A formal bridge or an explicit proof of hypothesis instantiation is required.

Thus, formalization does not simply preserve a pre-existing scientific object in a neutral way. It gives a precise mathematical representation of selected parts of a physical formalism. The resulting proof is rigorous relative to that representation; the adequacy of the representation for the scientific claim remains a separate question.

## 3.3. From a theorem to a model-internal claim: hypothesis instantiation

The distinction between a conditional theorem and a concrete model instance is central to the epistemology of mathematical physics.

The forward OS reconstruction theorem has the form

\[
\mathrm{OS}(S)\land \mathrm{Growth}(S)
\Longrightarrow
\exists W\;\mathrm{WickPair}(S,W).
\]

A proof of this implication establishes a general conditional relation. To conclude that a particular model M has a reconstructed Wightman family, one must establish that the Schwinger data associated with M satisfy both antecedents in the exact formal sense used by the theorem.

This is a familiar mathematical distinction between proving an implication and proving its antecedent for a particular object. In a formalized scientific setting, however, it has an additional epistemic role: the antecedent may encode substantive physical and analytic commitments. A growth condition is not a decorative technical assumption. It controls whether the reconstruction theorem applies.

The public OSreconstruction package proves the conditional theorem but does not itself expose inhabitants of its OS and corrected growth input records. Its README reports that a private companion project contains examples for the massive free field and the Proca Wick square. The existence of that reported companion work should be acknowledged, but it does not make the bridge publicly inspectable in the artifacts analyzed here. Nor does the separate OSforGFF theorem automatically provide the exact growth record required by OSreconstruction.

The lesson is not that the reconstruction theorem is incomplete as a conditional theorem. The theorem proves exactly what it states. The lesson is that the epistemic transition from a general theorem to a claim about a concrete model requires an explicit instance of every hypothesis. Machine checking makes this requirement more visible, not less important.

## 3.4. From a model to a physical target: representation and surrogate inference

Even after a theorem has been instantiated in a concrete mathematical model, a further distinction remains between a model-internal result and a claim about a physical target.

The DDI account provides a useful vocabulary. Denotation concerns what the model represents; demonstration concerns the reasoning performed within it; interpretation concerns how the result is related to the target (Hughes 1997). The OS case shows how machine checking can strengthen demonstration while leaving denotation and interpretation as separate tasks.

Other accounts of scientific representation sharpen this point. Suárez (2004) emphasizes the inferential capacities through which models support surrogate reasoning. Contessa (2007) distinguishes the validity of such reasoning from its soundness for the target. The DEKI account makes explicit the mapping and attribution of properties from model to target (Frigg and Nguyen 2018). These approaches differ in their account of representation, but each makes clear that a model property does not become a target property merely because it has been derived correctly within the model.

For the OS case, the mathematical reconstruction of Wightman-function distributions has a well-defined physical interpretation within axiomatic quantum field theory. But an application to a particular physical system requires specifying what the model is intended to represent and which aspects of the target are relevant. The massive Gaussian free field is an exact mathematical model of a free field under its assumptions. Its formal properties do not by themselves establish that a free-field description is empirically adequate for an interacting system.

This is also where purpose-relative model evaluation matters. A model may be adequate for a structural or mathematical purpose and inadequate for a quantitative prediction or an empirical description. Parker's adequacy-for-purpose account makes the target, user, methods, circumstances, and scientific goal relevant to the assessment (Parker 2020). The epistemic significance of a machine-checked theorem therefore depends partly on the purpose for which the theorem is used.

## 3.5. Mathematical rigor can transmit warrant, but it does not create empirical warrant

The distinction between generating and transmitting empirical warrant is particularly important. Gelfert (2009) argues that mathematically rigorous relations can transmit empirical warrant between physical models, illustrated by the relation between Hubbard and Heisenberg models in many-body physics. The mathematical relation may support a transfer of warrant from a model with empirical support to another model, provided that the relation is physically relevant and the conditions for the transfer are met.

The OS case is compatible with this account. A machine-checked proof could strengthen confidence in a mathematical map or implication used to relate two physical models. It could establish that the relation follows from specified assumptions. But it cannot create empirical support for the source model, establish that the relation preserves the physically relevant properties, or determine whether the target model is adequate for the intended purpose.

Machine checking therefore changes the quality of one component in a warrant-transfer argument. It can make the mathematical relation more reliable and inspectable. It does not replace the empirical and interpretative premises on which the transfer depends.

This point also prevents an overly restrictive conclusion. The fact that machine checking does not itself establish empirical adequacy does not make it scientifically peripheral. In mathematical physics, a rigorous relation between structures can be a central part of scientific reasoning. The proof assistant strengthens that relation's deductive status, while the physical significance of the relation remains a substantive scientific question.

## 3.6. Explanatory understanding is not identical to proof validity

A proof may establish that a proposition follows from a set of assumptions without explaining why the result is physically significant or why the underlying phenomenon occurs. The same distinction appears in ordinary mathematical practice: proof validity and explanatory value are related but not identical.

In the OS case, a formal proof of reflection positivity or a reconstruction theorem can establish the relevant mathematical property. Understanding why reflection positivity is physically important, how it contributes to the construction of a positive Hilbert-space structure, and what the reconstructed distributions mean within a physical theory requires additional mathematical and physical interpretation.

The present paper does not treat explanation as a mandatory final stage through which every formal theorem must pass. Some results provide structural or modal knowledge without being directed at a particular actual target. Models can function as epistemic artifacts for exploring possibilities and constraints, not only as representations of existing systems (Knuuttila 2021). A machine-checked theorem about such a model may be valuable even when no immediate empirical claim is intended.

The appropriate question is therefore not whether every proof must culminate in an empirical prediction. It is what kind of claim is being made and what form of warrant that claim requires.

## 3.7. The epistemic contribution of machine-checked demonstration

The analysis supports a differentiated conclusion.

For a formal claim, machine checking provides deductive warrant relative to a specified formal system and trust base. For a model-internal claim, the formal statement must correspond to the intended model statement and the model must satisfy every theorem hypothesis. For a target-directed claim, a further model-to-target inference must be justified in relation to the scientific purpose and relevant evidence. Explanatory understanding remains a related but distinct epistemic aim.

The OS case can be summarized as follows:

\[
\begin{aligned}
&\text{formal derivability}\\
&\quad\Downarrow\;\text{formalization correspondence and interpretation}\\
&\text{model-internal mathematical claim}\\
&\quad\Downarrow\;\text{target-directed inference and purpose-sensitive evaluation}\\
&\text{claim about a physical target}.
\end{aligned}
\]

The arrows do not represent automatic entailments. They mark additional relations that must be justified for the corresponding type of scientific claim.

The contribution of machine-checked proof is consequently neither unlimited nor merely cosmetic. It strengthens the demonstration component of scientific modeling by making formal assumptions and deductions explicit and mechanically checkable. Its limits arise not from a defect in proof checking, but from the fact that scientific knowledge involves more than deduction inside a formal language.

## 3.8. Scope and limitations of the case

The present argument is based on a source-critical analysis of public repositories at fixed revisions and on the mathematical statements exposed by those repositories. No fresh Lean build or proof replay was performed for this paper. The reported zero-admission and axiom-audit results are attributed to the project documentation and the specified checking procedures. The private companion development reported by OSreconstruction authors was not independently inspected.

The case is also deliberately narrow. It concerns a particular formalization ecosystem around the OS reconstruction programme and does not establish that every proof assistant, every physical formalism, or every scientific model has the same epistemic structure. The analysis is intended as a focused contribution to the philosophy of mathematical physics: it clarifies the local warrant provided by machine-checked demonstration and the distinct relations required to use that demonstration in scientific reasoning.

The main conclusion is therefore precise: a machine-checked theorem can be completely valid as a theorem of its formal system while the scientific knowledge warranted by it remains conditional on the formalization's correspondence to the source formalism, the instantiation of its hypotheses, and the interpretation and use of the resulting model. The reliability of the proof and the scope of the scientific claim are different questions, and a rigorous account of formalized physics must answer both.
