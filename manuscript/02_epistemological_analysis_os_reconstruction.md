# 2. Epistemological Analysis of Osterwalder–Schrader Reconstruction

## 2.1. The reconstruction programme and its formalization

The Osterwalder–Schrader programme concerns the relation between Euclidean field-theoretic data and relativistic quantum field theory. In the Euclidean formulation, the central objects are Schwinger functions. Under suitable conditions, these functions can be analytically continued to Wightman distributions satisfying the characteristic properties of relativistic quantum field theory, including covariance, spectral support, locality, and positivity. The original axiomatic formulation established conditions under which Euclidean Green functions determine a relativistic theory (Osterwalder and Schrader 1973). The 1975 sequel is indispensable for stating the forward theorem precisely: it extends and corrects the earlier result and introduces the additional linear growth condition E0-prime (Osterwalder and Schrader 1975). The reconstruction claim relevant here is therefore conditional on more than the qualitative OS conditions E0–E4.

The public Lean developments considered here formalize different parts of the reconstruction programme. OSforGFF (Douglas, Hoback, Mei, and Nissim 2026) constructs a concrete massive Gaussian free-field model and establishes its OS properties in the project’s formal setting. OSreconstruction (Yin, Douglas, and Mei 2026) formalizes conditional theorems relating Euclidean Schwinger data to Wightman-function distributions. OSreconstruction-comparator (Douglas, Yin, and Mei 2026) provides a separate mathematical specification and proof-checking interface for the reconstruction propositions. The epistemic significance of these developments depends on the exact statements they establish, rather than on the general fact that all three concern the OS framework.

## 2.2. OSforGFF and the status of the concrete Euclidean model

OSforGFF constructs the massive Gaussian free field as a probability measure on the space of tempered distributions \(S'(\mathbb R^D)\). At the pinned repository revision, the project states a dimension-generic result for spacetime dimension \(D\geq 2\), together with explicit propagator instances in dimensions \(D=2,3,4,5\). Its principal theorem, gaussianFreeField_satisfies_all_OS_axioms_generic, establishes that the specified massive Gaussian free-field measure satisfies the collection of OS properties encoded by the project. These include analyticity of the generating functional, the project’s regularity condition, Euclidean invariance, reflection positivity, clustering, and an additional ergodicity property.

The mathematical content of this result is stronger than the verification of an abstract implication. A particular probability measure is constructed, and properties of its associated generating functional are established. The result therefore supports a model-internal claim about the specified massive Gaussian free-field construction. The repository reports that the relevant theorems contain no sorry and use no project-specific axioms at the pinned revision. Such statements are understood relative to the Lean environment and its foundational trust base; the present analysis does not claim to have independently rebuilt or replayed the proofs.

The scope of the theorem is determined by the definitions used in the formalization. In particular, the condition designated OS1 in OSforGFF is expressed as an exponential bound on the generating functional, together with an associated two-point integrability and convergence condition. This predicate is not definitionally identical to the arity-dependent OS-II growth condition required by OSreconstruction. The shared terminology of regularity and growth does not establish equivalence between these conditions. Any use of the OSforGFF result as an input to the OSreconstruction theorem therefore requires an explicit correspondence between the relevant formal records and a proof that the precise growth hypothesis is satisfied.

The theorem also has a specific physical scope. It establishes properties of a massive Gaussian free-field model under the assumptions encoded in the construction. It does not, solely by virtue of those properties, establish the empirical adequacy of a free-field description for an interacting system or for a particular experimental target. That distinction concerns the application of the model, not the validity of the theorem about the model.

## 2.3. OSreconstruction and the conditional character of the forward theorem

OSreconstruction formalizes forward and reverse relations between Euclidean Schwinger-function data and relativistic Wightman-function distributions. Its dimensional convention differs from that of OSforGFF: \(d\) denotes the positive spatial dimension, and spacetime has dimension \(d+1\). Thus, a four-dimensional spacetime comparison corresponds to \(D=4\) in OSforGFF and \(d=3\) in OSreconstruction.

The formal input is specified carefully. The Euclidean Schwinger functions act on a zero-diagonal Schwartz test-function space, whereas the Wightman distributions act on the full Schwartz space. The distinction is relevant to reconstruction because the passage from the Euclidean test-function domain to the full relativistic distributional domain is part of the mathematical content of the theorem. It is not merely a change in notation.

The public theorem os_to_wightman has the schematic form

\[
\mathrm{OS}(S)\land \mathrm{Growth}(S)
\Longrightarrow
\exists W\;\mathrm{WickPair}(S,W).
\]

The first antecedent is the project’s record of the OS conditions E0–E4. The second is a separate OSLinearGrowthCondition. In the formal specification, this condition is an arity-dependent estimate of the schematic form

\[
\|S_n(f)\|
\leq
\alpha\,\beta^n(n!)^\gamma
\|f\|_{ns,ns},
\]

where \(\alpha\) and \(\beta\) are positive, \(\gamma\) is real, and the orders of the Schwartz seminorms increase linearly with the arity \(n\). The full definition also includes normalization at arity zero and requires the estimate for every arity and every zero-diagonal test function. It is therefore a quantitative condition on the family of Schwinger distributions, rather than a generic assumption of continuity or temperedness.

The theorem concludes that there exists a Wightman-function family whose distributions are Wick-paired with the input Schwinger family. Its logical form is important: the result establishes a conditional reconstruction theorem. The existence of the Wightman family follows from the specified OS assumptions together with the exact growth condition. The proof does not establish that every Euclidean family satisfying E0–E4 alone admits the stated reconstruction.

The package also formalizes the OS-II version of the forward theorem. With the original-coordinate growth condition, the theorem yields a Wick-paired Wightman family, an output coordinate-norm growth estimate corresponding to R0-prime, and uniqueness among Wightman-function families satisfying the specified Wick-pairing relation. The uniqueness claim is consequently relative to that relation and the formalized class of Wightman families. It should not be enlarged into a claim that all possible physical interpretations or operator realizations have been uniquely determined.

The reverse theorem constructs Euclidean Schwinger data from a Wightman-function family and establishes the corresponding OS properties for the constructed data. Unlike the forward theorem, this direction does not require the OS-II growth hypothesis as an input. The asymmetry of the two directions matters: the formalized results do not amount to an unconditional biconditional between arbitrary OS data and arbitrary Wightman data.

The output of the public package is a family of Wightman distributions. The package explicitly does not claim to complete the subsequent GNS construction of a Hilbert space and operator-valued fields. Although that construction belongs to the broader mathematical context of the OS programme, it is outside the stated endpoint of this formalization. The distinction between distributional reconstruction and operator reconstruction must therefore be preserved when describing what the Lean development establishes.

The distributable OSreconstruction package does not itself expose inhabitants of its OS input record or its corrected growth-condition record. Its documentation reports that a private companion project contains examples, including the massive free field and the Proca Wick square, satisfying the relevant conditions. Since the companion project is not publicly inspectable, the present analysis records this as an author-reported result. It would be unwarranted to infer from the public package alone that no concrete model satisfies the growth condition; it would be equally unwarranted to claim that the pinned OSforGFF artifact has been formally connected to the exact input record of the pinned OSreconstruction package.

## 2.4. The Comparator and the scope of independent checking

The OSreconstruction-comparator repository provides a Mathlib-only challenge specification and a corresponding solution. The challenge states the relevant reconstruction propositions using definitions that can be read independently of the production package. The solution discharges the proof obligations using the production development. The repository reports structural comparison and proof replay through Comparator and NanoDa, with the stated whitelist of Lean’s foundational axioms.

This arrangement strengthens the auditability of the formal statements and their proofs. The independently stated challenge makes the target propositions explicit outside the production package, while the replay procedure provides an additional check of the proof artifacts under the specified formal environment. The Comparator should not, however, be characterized as a second independent mathematical derivation by a separate research group. The repository describes itself as a checking interface around the production development, rather than as an independent reconstruction of the mathematics. Nor does the procedure provide empirical validation of the physical theory.

The Comparator documentation also discloses conventions that delimit the exact propositions under examination. These include an additional condition on the first imaginary coordinate in the forward tube, locality formulated for adjacent transpositions, reflection positivity expressed through a totalized coercion onto zero-diagonal test functions, and the use of growth as a forward hypothesis rather than a conclusion of the reverse construction. Such conventions are part of the mathematical specification being checked. Accordingly, the epistemic assessment must concern the formalized propositions as stated, rather than a broader textbook formulation that may suppress these choices.

## 2.5. The relation between the formal developments

The three projects cannot be combined into a single proof chain merely because they concern the same reconstruction programme. Their relation involves several distinct mathematical interfaces.

First, the formal records differ. OSforGFF formulates its result through a probability measure and its generating functional. OSreconstruction takes a family of Schwinger distributions on a zero-diagonal Schwartz test-function space. To use the output of the former as the input of the latter, one needs a map between these records that preserves the relevant mathematical structure.

Second, the regularity assumptions differ. The OS1 condition in OSforGFF is not definitionally the same as the arity-dependent OS-II growth condition in OSreconstruction. Direct application of the reconstruction theorem therefore requires either a proof that the concrete model satisfies the latter condition or an explicit theorem relating the two formal predicates. The fact that both conditions concern growth does not supply such a proof.

Third, the dimensional conventions must be translated. OSforGFF uses \(D\) for spacetime dimension, whereas OSreconstruction uses \(d\) for spatial dimension and \(d+1\) for spacetime. The four-dimensional spacetime case is thus represented by \(D=4\) in the former project and \(d=3\) in the latter. Finally, the projects use different Lean and Mathlib revisions. Their respective theorems are established in their own pinned environments; direct composition is not supplied by the separate theorem statements.

The public artifacts inspected do not expose a single end-to-end theorem that takes the specific OSforGFF construction and proves that it satisfies the exact OSreconstruction growth input at the pinned revisions. This is a claim about the public interface examined here, not a claim that the required mathematical relation is impossible or that no such result exists in the private companion development reported by the authors. The distinction is important because the epistemological issue concerns the warrant actually made available by the formal artifacts, not the mathematical possibility of extending them.

## 2.6. Denotation, demonstration, and interpretation in the OS case

The DDI distinction provides a useful structure for assessing these results. At the level of denotation, OSforGFF specifies a mathematical probability model: the massive Gaussian free field on a space of tempered distributions, with covariance determined by the propagator construction. OSreconstruction, by contrast, takes Euclidean Schwinger-function data on a specified test-function space. The physical interpretation of these objects is supplied by the OS framework, but the formal relation between the two records requires an explicit map. A common physical designation does not establish formal equivalence.

At the level of demonstration, the Lean projects establish different mathematical claims. OSforGFF proves the bundled OS properties for its specified Gaussian free-field construction. OSreconstruction proves conditional reconstruction theorems from its exact OS and growth hypotheses. The Comparator adds a separate statement and proof-checking interface for the reconstruction propositions. Machine checking contributes most directly at this level: it makes the mathematical demonstration explicit, subjects proof objects to kernel checking, and permits the assumptions and theorem endpoints to be examined. Its contribution is substantial, but its object is the formal proposition as encoded.

At the level of interpretation, the mathematical structures are understood through the physical relation between Euclidean Schwinger functions, reflection positivity, analytic continuation, and relativistic Wightman distributions. The formalized reconstruction result has a clear place within axiomatic quantum field theory. Nevertheless, the distributional endpoint should not be conflated with the subsequent construction of a Hilbert space and operator-valued fields, which the public package does not claim to complete.

The distinction becomes sharper when a model is used to make a target-directed claim. The OS properties of the massive Gaussian free field establish mathematical facts about that model. Whether the model is used as an exact representation of a free theory, as an idealization, or as a component of an approximation to a more complex system depends on the scientific purpose and the relevant model-to-target relation. The machine-checked theorem does not determine that purpose or establish empirical adequacy for an interacting system.

## 2.7. The epistemic content of the formalized results

The OS case supports three different kinds of claim. The first is a claim about a formal derivation: a proposition follows from specified assumptions in a specified formal system. The second is a model-internal claim: the interpreted mathematical proposition holds of a concrete model, provided that the model satisfies every hypothesis in the formal theorem. The third is a target-directed scientific claim: a property of the model warrants an inference about a physical system for a specified purpose. These claims are related, but they are not interchangeable.

The formal artifacts establish strong results at the first level and, in the case of OSforGFF, a concrete model-internal result at the second. The forward OSreconstruction theorem establishes a conditional mathematical relation, but its application to a particular model requires an instance of the exact growth hypothesis. A target-directed claim requires a further account of the model’s representational role and the evidence appropriate to the intended application. This structure does not diminish the mathematical achievements of the formalizations. It specifies the different kinds of knowledge to which those achievements can contribute.
