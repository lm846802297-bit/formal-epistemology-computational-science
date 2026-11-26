# Paper Outline

**Title:** What Does a Machine-Checked Proof Establish in Physics? The Epistemology of Formalized Osterwalder-Schrader Reconstruction

**Target length:** approximately 7,000-9,000 words.

1. Introduction: machine checking in science; local guarantee; bounded contribution.
2. What machine checking establishes: proof objects, kernel, assumptions, imports, trust base; Duede & Davey.
3. Informal science to formal proposition: DeDeo & Duede; FormalScience; semantic drift and tracking.
4. Formal proposition to physical model: interpretation of fields, states, operators, observables, symmetries; idealization and epistemic artifacts.
5. Model to target: verification, validation, purpose-sensitive inference, empirical warrant.
6. Warrant architecture: C_F, C_M, C_W, C_E; two-track model; claim-sensitive transfer.
7. Case study: OSforGFF + OSreconstruction + Comparator; Bobbin et al.; bounded axial anomaly stress test.
8. Discussion.
9. Conclusion.

## Working abstract
This paper examines the epistemic scope of machine-checked proofs in mathematical physics through recent Lean formalizations of the Osterwalder-Schrader (OS) axioms and reconstruction theorem. It distinguishes formal validity, theorem-statement adequacy, instantiation of analytic growth assumptions, reconstruction of Wightman distributions, and empirical warrant for a physical target. The analysis compares a public formalization showing that a massive Gaussian free field satisfies the OS axioms with a separate package proving conditional OS-to-Wightman and reverse reconstruction theorems, together with a Comparator audit of theorem statements. These results are mathematically substantial, but their exact hypotheses and endpoints matter. In particular, the forward reconstruction theorem requires an arity-dependent growth condition not inhabited within that package, and the formalized endpoint is a family of Wightman distributions rather than a full GNS/operator reconstruction. The case shows that machine checking can establish strong conditional mathematical results while transfer to a concrete model and an empirical target depends on separately justified interfaces. The paper develops a claim-sensitive account of these interfaces and argues that mathematical reconstruction, physical interpretation, and empirical adequacy are distinct forms of warrant.