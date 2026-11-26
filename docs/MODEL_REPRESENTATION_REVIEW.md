# Scientific Model Representation and Model-Based Reasoning: Comparative Review

**Review date:** 2026-11-26  
**Status:** Targeted literature review; not an exhaustive systematic review.

## 1. Scope and distinctions

Three questions are often conflated:

1. **Representation:** In virtue of what does a model represent a target?
2. **Model-based inference:** How can operations or deductions performed on a model license conclusions about its target?
3. **Model evaluation:** What makes a model and its use adequate for a particular scientific purpose?

A fourth question becomes central for formalized physics:

4. **Formalization and proof:** What does a machine-checked derivation certify about the mathematical formalism and model, and what remains to be justified in applying the result?

The first three questions have substantial prior literatures. Our project must not claim them as new.

## 2. Major accounts of scientific representation

### 2.1 Pragmatic and similarity-based accounts: Giere

Giere, R. N. (2004), “How Models Are Used to Represent Reality,” Philosophy of Science 71(5), 742–752, DOI: 10.1086/425063.

Giere shifts attention from an abstract dyadic relation between language and world to the activity in which scientists use models to represent aspects of the world for particular purposes. Designated similarities are specified in selected respects and degrees.

**Contribution:** representation is pragmatic and purpose-sensitive; similarity is selected rather than global.

**Relevance to formal proof:** a proof can establish a mathematical property of a model, but it cannot decide which similarities matter for a scientific purpose or whether the model is suitable for that purpose.

### 2.2 DDI: Hughes

Hughes, R. I. G. (1997), “Models and Representation,” Philosophy of Science 64, Supplement, S325–S336, DOI: 10.1086/392611.

The DDI account distinguishes:
- **Denotation:** a model stands for a target.
- **Demonstration:** reasoning is carried out within the model.
- **Interpretation:** the model result is related back to the target.

**Contribution:** separates internal model reasoning from its interpretation as a claim about the target.

**Relevance to formal proof:** kernel checking can strengthen the Demonstration component. It does not, by itself, establish Denotation or the correctness of Interpretation.

### 2.3 Inferential conception: Suárez

Suárez, M. (2004), “An Inferential Conception of Scientific Representation,” Philosophy of Science 71(5), 767–779, DOI: 10.1086/421415.

Suárez characterizes scientific representation through directionality and the capacity to support surrogate reasoning. Such reasoning need not be deductive: scientific model use also includes inductive, analogical, and abductive inferences.

**Contribution:** representation is connected to the inferences that a model enables users to draw about its target.

**Relevance to formal proof:** Lean checks derivations in a formal deductive system. It does not certify the full range of inductive, analogical, or abductive reasoning used in scientific modeling.

### 2.4 Interpretational account: Contessa

Contessa, G. (2007), “Scientific Representation, Interpretation, and Surrogative Reasoning,” Philosophy of Science 74(1), 48–68, DOI: 10.1086/519478.

Contessa argues that an interpretation of a model in terms of a target grounds the possibility of valid surrogative inferences. Crucially, such inferences can be valid without necessarily being sound.

**Contribution:** distinguishes the validity of model-to-target inference from its truth-conduciveness or faithfulness.

**Relevance to formal proof:** a kernel-checked proof may establish validity inside the formal model. It does not show that the interpretation connecting the model to the physical target is sound.

### 2.5 DEKI: Frigg and Nguyen

Frigg, R. and Nguyen, J. (2018), “The Turn of the Valve: Representing with Material Models,” European Journal for Philosophy of Science 8, 205–224, DOI: 10.1007/s13194-017-0182-4.

The DEKI account analyses representation through four elements:
- **Denotation:** what the model stands for.
- **Exemplification:** which properties the model exhibits.
- **Keying:** how model properties are mapped to target properties.
- **Imputation:** which properties are attributed to the target.

The paper develops the account through material models; its use as a general analytic template for mathematical physics requires care.

**Contribution:** makes the mapping from model properties to target properties explicit.

**Relevance to formal proof:** a proof of property P in a mathematical model does not establish that P is correctly keyed to a property of the physical target, or that the target should be imputed to possess it.

### 2.6 Models as mediators and epistemic artifacts

Morrison, M. and Morgan, M. S. (1999), “Models as Mediating Instruments,” in Models as Mediators: Perspectives on Natural and Social Science, pp. 10–37, DOI: 10.1017/CBO9780511660108.003.

Morgan and Morrison emphasize the relative autonomy of models: models are not simply deduced from theory or copied from data. Their construction and manipulation make them instruments of investigation and exploration.

Knuuttila, T. (2021), “Epistemic Artifacts and the Modal Dimension of Modeling,” European Journal for Philosophy of Science 11, 65, DOI: 10.1007/s13194-021-00374-5.

Knuuttila argues that models as constructed artifacts can support modal and exploratory inquiry. Their epistemic value need not always depend on representing an actual target system.

**Contribution:** scientific knowledge can concern possible structures and mechanisms, not only actual target systems.

**Relevance to formal proof:** target-world transfer is not a mandatory endpoint for every formalized model. A theorem may provide mathematical or modal knowledge about a constructed model even when no actual target is intended.

## 3. Mathematical formalisms and cross-model reasoning

### 3.1 Gelfert (2009): a direct antecedent for warrant transfer

Gelfert, A. (2009), “Rigorous Results, Cross-Model Justification, and the Transfer of Empirical Warrant: The Case of Many-Body Models in Physics,” Synthese 169, 497–519, DOI: 10.1007/s11229-008-9431-6.

This is a particularly close antecedent. Gelfert argues that mathematically rigorous results and relations can transmit empirical warrant between models. His case study concerns the Hubbard and Heisenberg models and the Mott metal-insulator transition.

The argument distinguishes:
- the **generation** of empirical warrant, which depends on empirical success and other sources of support;
- the **transmission** of empirical warrant, which may occur through an appropriate mathematically rigorous relation between models.

A rigorous relation does not create empirical warrant from nothing. It can transmit warrant from an empirically successful model to another model when the relation is physically relevant.

**Consequence for our project:** do not claim that mathematical proof or rigorous model relations provide a new general theory of warrant transfer. The more precise question is what machine checking adds to the certification of the mathematical relation, and what physical conditions still govern its warrant-transmitting role.

### 3.2 Gelfert (2011): mature mathematical formalisms

Gelfert, A. (2011), “Mathematical Formalisms in Scientific Practice: From Denotation to Model-Based Representation,” Studies in History and Philosophy of Science Part A 42(2), 272–286, DOI: 10.1016/j.shpsa.2010.11.035.

Gelfert develops the concept of a **mature mathematical formalism**: a mathematically formulated and physically interpreted notational system with locally applicable rules, connected to theoretical and methodological commitments.

Such formalisms:
- constrain which mathematical operations are legitimate;
- carry theoretical, ontological, and methodological commitments;
- provide inferential and interpretative resources;
- may embody assumptions that are no longer obvious to proficient users.

The discussion includes physical formalisms such as operator methods and Feynman diagrams.

**Consequence for our project:** Lean formalization should be understood as a selective formal re-articulation of a mature physical formalism, not merely the transcription of equations. The formalization may expose some assumptions while omitting or changing other inferential and interpretative commitments.

### 3.3 Gelfert (2022): notations as epistemic actions

Gelfert, A. (2022), “Thinking with Notations: Epistemic Actions and Epistemic Activities in Mathematical Practice,” in Model and Mathematics: From the 19th to the 21st Century, pp. 333–362, DOI: 10.1007/978-3-030-97833-4_11.

Gelfert argues that notations and formalisms are not neutral containers for pre-existing concepts. They shape mathematical practice and function as inferential resources. Formalization can constrain admissible manipulations while increasing inferential depth and enabling new lines of inquiry.

**Consequence for our project:** proof-assistant formalization is not epistemically neutral. The formal language, libraries, definitions, and proof obligations can reshape how a mathematical-physics result is represented and derived.

### 3.4 Cartwright: models and the limits of theory

Cartwright, N. (1999), “Models and the Limits of Theory: Quantum Hamiltonians and the BCS Models of Superconductivity,” in Models as Mediators, pp. 241–281, DOI: 10.1017/CBO9780511660108.010.

This chapter provides a physics-specific reminder that models and their interpretative assumptions cannot simply be read off from a fundamental theory. It is useful as a comparison for the role of mathematical structures and model construction in theoretical physics.

### 3.5 Hartmann: formal derivation and physical understanding

Hartmann, S. (1999), “Models and Stories in Hadron Physics,” in Models as Mediators, pp. 326–346, DOI: 10.1017/CBO9780511660108.012.

Hartmann discusses the role of physical stories and interpretation in legitimating models in hadron physics. This supports treating explanatory understanding as distinct from formal derivability.

## 4. Model evaluation and purpose

Parker, W. S. (2020), “Model Evaluation: An Adequacy-for-Purpose View,” Philosophy of Science 87(3), 457–477, DOI: 10.1086/708691.

Parker argues that model adequacy should be assessed relative to a target, user, methodology, circumstances, and goal. Representational accuracy alone is not a complete evaluation.

**Consequence for our project:** a formal theorem may be adequate evidence for a mathematical or structural purpose, but insufficient for a predictive or empirical purpose. The relevant question is always: what scientific purpose is the result intended to serve?

## 5. Comparative matrix

| Account | Main relation | What it contributes | What machine checking does not establish |
|---|---|---|---|
| Giere | Model–target similarity for a purpose | Selected respects and degrees of similarity | Which similarities matter for the task |
| Hughes DDI | Denotation–demonstration–interpretation | Separates internal reasoning from target interpretation | Denotation and sound interpretation |
| Suárez | Inferential capacity | Model-supported surrogate reasoning | Soundness of target inference; non-deductive inference |
| Contessa | Interpretation and valid surrogative inference | Validity need not imply soundness | Physical truth of the model-to-target mapping |
| Frigg–Nguyen DEKI | Denotation, exemplification, keying, imputation | Explicit property mapping | Keying and imputation to the target |
| Morgan–Morrison | Model as autonomous mediator | Construction, manipulation, exploration | The full practice of model construction and use |
| Gelfert 2009 | Rigorous cross-model relations | Transmission of empirical warrant | Empirical support of source model and physical relevance of relation |
| Gelfert 2011/2022 | Mature formalisms and notational practice | Embedded rules, commitments, inferential resources | Whether the Lean encoding captures the full source formalism |
| Knuuttila | Model as epistemic artifact | Modal and exploratory knowledge | Whether an actual target exists or is intended |
| Parker | Adequacy for purpose | Target, user, method, circumstances, goal | Whether a checked theorem serves the intended scientific purpose |

## 6. Synthesis

The literature already explains:
- how models represent targets;
- how models support surrogate reasoning;
- how rigorous mathematical relations can transmit empirical warrant;
- how mature mathematical formalisms constrain scientific inference;
- why model adequacy is purpose-sensitive;
- why models can support modal and exploratory knowledge without an actual target.

The candidate contribution is therefore narrower:

**How does machine-checkable formalization alter the epistemic role of demonstration within mature mathematical formalisms in theoretical physics, and what additional correspondence, interpretation, and model-evaluation warrants remain necessary?**

This is not a claim to invent a new general theory of representation or warrant transfer. It is a formalization-aware analysis of existing model-based reasoning, tested against concrete mathematical-physics formalizations.

## 7. Primary case and comparison cases

- **Primary case:** the public Lean formalizations of OS axioms and OS reconstruction, with exact commits and theorem interfaces recorded in CASE_STUDY_OS_RECONSTRUCTION.md.
- **Cross-model warrant comparison:** Gelfert's Hubbard–Heisenberg case.
- **Mature-formalism comparison:** operator formalism and Feynman diagrams, following Gelfert.
- **Secondary formalization comparison:** Bobbin et al. (2024), formalizing chemical physics in Lean.
- **Bounded physics example:** the axial Ward identity and quantum anomaly, used only after primary-source convention checks.

## 8. Review limitations

This is a targeted comparison, not a systematic review. It does not establish a priority claim. Further targeted checking is needed for work specifically combining proof assistants, mature mathematical formalisms, and model-based warrant in theoretical physics.
