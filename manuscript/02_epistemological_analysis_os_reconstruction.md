# 2. The Osterwalder–Schrader Formalization Network

## 2.1. The mathematical setting

The Osterwalder–Schrader programme establishes conditions under which Euclidean field-theoretic data can be related to relativistic quantum field theory. Its Euclidean objects are Schwinger functions; the reconstructed relativistic objects are Wightman functions or distributions. The original OS papers formulate axioms for Euclidean Green functions and develop the corresponding reconstruction theorem (Osterwalder & Schrader, 1973, 1975). The 1975 paper explicitly extends and corrects the 1973 result by introducing the linear growth condition E0-prime. This correction is essential to the forward reconstruction theorem: the qualitative OS conditions E0–E4 alone do not supply the full hypothesis required by the corrected result.

The mathematical setting is not unique. Glimm and Jaffe (1987) formulate the Euclidean theory in terms of a probability measure on field configurations and its generating functional. The original OS formulation, by contrast, is expressed in terms of Schwinger functions as distributions on an appropriate test-function space. Douglas et al. (2026) choose the Glimm–Jaffe formulation for their Lean formalization because it makes the construction of a Euclidean field theory a problem about a functional measure, a mathematical structure well supported by Mathlib. They explicitly note that this is a variant of the original OS axioms and explain the relationship between their use of Schwartz functions and the compactly supported test functions in the Glimm–Jaffe presentation. The three formalization projects considered below should therefore be understood as related representations of the OS programme, not as interchangeable encodings of a single record.

## 2.2. OSforGFF: the probability-measure formulation

At commit fef84a82937dfd2bb7f672108a72da329d3ef0fd, OSforGFF (Cherkis et al., 2026) constructs the massive Gaussian free field as a probability measure on the space of tempered distributions S'(R^D), where D ≥ 2 is the spacetime dimension. The generic construction uses a covariance specified through a propagator typeclass, with explicit covariance instances in dimensions D=2,3,4,5. The principal theorem, gaussianFreeField_satisfies_all_OS_axioms_generic, proves that the constructed measure satisfies the project's bundled Glimm–Jaffe OS properties. The repository reports zero sorry declarations and no project-specific axioms for the pinned library theorem; these claims are understood relative to its Lean environment and foundational dependencies.

The axioms are predicates on the probability measure and its generating functional. OS0 states analyticity of the generating functional in finite collections of complex test-function parameters. OS1 is a regularity condition: there exist p in [1,2] and c>0 such that

\[
|Z_\mu(f)| \leq
\exp\left[
c\left(
\int_{\mathbb R^D}|f(x)|\,dx+
\int_{\mathbb R^D}|f(x)|^p\,dx
\right)
\right],
\]

together with a subsidiary local-integrability condition on the two-point function when p=2. For the massive Gaussian free field, the formal proof chooses p=2 and c=1/(2m^2), and proves the required two-point condition by identifying the mollified two-point function with the covariance kernel away from coincidence. OS2 expresses invariance under the Euclidean group. OS3 is reflection positivity in a complex generating-functional formulation, with time reflection and complex conjugation. OS4 is represented through clustering and ergodicity; the latter is formulated for a specified class of finite exponential functionals and established using a polynomial-clustering estimate.

These choices are not merely notational. The OSforGFF documentation and the accompanying paper explain how the formalized conditions relate to the Glimm–Jaffe presentation. In particular, the use of Schwartz test functions and tempered distributions is stated to imply the corresponding compactly supported test-function formulation, since D(R^D) is contained in S(R^D) and S'(R^D) is contained in D'(R^D). The authors also explain that their ergodicity condition is imposed on a dense class of finite exponential functionals and uses L2 convergence; they argue that density in L1 and the implication from L2 to L1 on a probability space recover the Glimm–Jaffe condition. These are substantive correspondence claims between the formal predicates and the source axioms. They are part of the mathematical interpretation of the formalization and should not be replaced by the bare observation that Lean accepts the proof.

The OS1 condition is particularly relevant to the comparison with OSreconstruction. It is the Glimm–Jaffe exponential regularity bound on the generating functional, with an additional two-point integrability condition. It is not the same predicate as the arity-dependent E0-prime growth condition required by the forward OSreconstruction theorem. The former controls the generating functional in terms of L1 and Lp norms of a single test function; the latter is a quantitative estimate on the family of n-point Schwinger distributions, with Schwartz seminorm orders increasing linearly with n. The shared language of regularity or growth does not establish a mathematical implication between them.

## 2.3. OSreconstruction: zero-diagonal Euclidean data and conditional reconstruction

At commit cf0904e34a7c146a9f312f601e3707dca4a87697, OSreconstruction (Yin et al., 2026) formalizes reconstruction for every positive spatial dimension d, with spacetime dimension d+1. Its Euclidean input is a family of Schwinger functions acting on the zero-diagonal Schwartz test-function space. Its Wightman distributions act on the full Schwartz space. The zero-diagonal domain is mathematically significant: it accommodates the coincidence singularities of Euclidean Schwinger functions without presupposing that they define distributions on the full Schwartz space.

The formal record OsterwalderSchraderAxioms includes temperedness, linearity and reality on the zero-diagonal test space; translation and connected Euclidean rotation invariance; reflection positivity on Borchers sequences supported in the ordered positive-time region; permutation symmetry; and the cluster property. The forward theorem os_to_wightman additionally assumes an OSLinearGrowthCondition. Schematically, the condition takes the form

\[
\|S_n(f)\|
\leq
\alpha\,\beta^n(n!)^\gamma
\|f\|_{ns,ns},
\]

where alpha and beta are positive, gamma is real, and the Schwartz seminorm orders grow linearly with the arity n. The exact Lean definition uses a supremum over the relevant weight and derivative indices and includes a normalization condition at arity zero. The theorem concludes the existence of a Wightman-function family whose distributions are Wick-paired with the input Schwinger family.

The package also formalizes the original-coordinate version of the OS-II growth condition. Its OSIIOriginalLinearGrowthCondition requires a positive Sobolev index s and the estimate

\[
\|S_n(f)\|
\leq
\alpha (n!)^\gamma
\|f\|_{\mathrm{OSII},ns},
\]

where the final seminorm is the original-coordinate seminorm on the zero-diagonal test space. The public arity-linear condition instead uses the maximum of the relevant Schwartz seminorms with weight and derivative orders bounded by ns, and allows the coefficient \(\alpha\beta^n(n!)^\gamma\). The theorem os_to_wightman_osii_original converts the original-coordinate record into the arity-linear record with the explicit parameter choice

\[
\alpha' = \max\{1,\alpha\},\qquad
\beta'=(d+2)^s,\qquad
\gamma'=\gamma+2s.
\]

It then concludes three results: existence of a Wick-paired Wightman family, the output growth estimate R0-prime, and uniqueness among Wightman families satisfying the same Wick-pairing relation. The conversion is a proved quantitative interface, not an identification by terminology. The package explicitly distinguishes this corrected arity-dependent condition from an earlier fixed-order growth predicate that it does not treat as an equivalent reconstruction input.

The reverse theorem constructs Euclidean Schwinger data from a Wightman-function family and proves the corresponding OS properties for that constructor. It does not assume the forward growth condition. The two directions therefore do not form an unconditional biconditional between arbitrary OS data and arbitrary Wightman data. The public endpoint is a family of Wightman distributions satisfying the formalized Wightman-function axioms, including covariance, spectral support, locality, positivity, Hermiticity, and clustering. The package explicitly places the subsequent GNS construction of a Hilbert space and operator-valued fields outside its scope.

The distributable OSreconstruction package does not itself expose inhabitants of its OS input record and corrected growth-condition record. Its README reports that a private companion project contains examples for the massive free field and the Proca Wick square. The report is attributed to the package authors; the private development is not independently inspectable here. Moreover, the existence of a massive free-field inhabitant in that companion project does not, by itself, identify it with the particular probability-measure object constructed by OSforGFF at the pinned revision. Establishing that identity or an appropriate correspondence is precisely an inter-formalization task.

## 2.4. Comparator: an explicit bridge between formal records

The OSreconstruction-comparator project (Douglas, Yin, et al., 2026), pinned at commit 93cdb40e728ba27b7b1b55efc30d57f7b43de9aa, provides a Mathlib-only challenge and a solution for the three reconstruction propositions. Its notion of independence is specific. The challenge does not import the production package; it reproduces verbatim the package's own Mathlib-only audit definitions from verification/comparator/Definitions.lean and appends the three theorem obligations. It is therefore an independently elaborated checking surface, not an independently authored mathematical specification or a second derivation by a separate research team.

The bridge files provide the important mathematical content. OSBridge.lean constructs conversions in both directions between the challenge's OS record and the production OsterwalderSchraderAxioms record. The Schwinger family is preserved definitionally. The bridge also identifies the challenge and production growth records, relates the Wick-pairing predicates, and establishes equality of the relevant output-growth predicates and original-coordinate seminorms. Solution.lean then proves equivalences between the challenge statements and the production specifications for the forward theorem, the OS-II theorem, and the reverse constructor. These equivalences preserve the underlying distribution families.

The Comparator checks that the challenge and solution share structurally corresponding declarations, that the proof dependencies remain within the stated whitelist of Lean's foundational axioms, and that the proofs can be replayed through a fresh kernel and NanoDa. The project itself describes the repository as a thin wrapper containing no new mathematics. Its epistemic contribution is consequently not an independent mathematical discovery. It is a separately checked interface that makes the relation between a public theorem specification and the production formalization explicit and auditable. The challenge definitions are copied from the source project's own audit file, while the record adapters and theorem equivalences provide the bridge to the production records. The distinction between these roles is important: the challenge is independent at the level of imports and checking boundary, but not independent in authorship or mathematical origin.

## 2.5. What is and is not connected in the public formalization network

The three projects thus exhibit two different kinds of correspondence. Within the OSforGFF project, the authors explain how the probability-measure predicates relate to the Glimm–Jaffe axioms, including the use of Schwartz rather than compactly supported test functions and the restricted class used in the ergodicity statement. Within OSreconstruction and its Comparator, explicit Lean bridges identify independently elaborated records and preserve the Schwinger family, growth assumptions, and theorem conclusions. These are positive examples of correspondence work; they show that a formalization interface can itself become an object of mathematical proof.

The public artifacts do not, however, expose a single theorem that takes the specific OSforGFF construction and establishes that its associated Schwinger data inhabit the exact zero-diagonal OS record and arity-dependent growth condition required by OSreconstruction. Such a composition would require at least a map from the probability measure and generating functional to the relevant Schwinger distributions, a proof that the OS predicates transfer to the zero-diagonal formulation, and an inhabitant of the precise growth record. The different test-function domains and formal records cannot be identified merely because both projects concern the massive free field and the OS programme. The QFT formalization paper itself describes OS reconstruction as a subsequent milestone for the OSforGFF development. The private companion reported by OSreconstruction authors provides relevant additional evidence, but it does not make the specific public OSforGFF-to-OSreconstruction bridge inspectable.

The significance of the case does not depend on treating the missing public interface as a defect in either mathematical project. Each project proves the propositions it states. The issue is whether, and under what conditions, their results can be composed to support a further scientific claim. This is a question about the warrant of the interfaces between formalizations, not about the validity of the local proofs.
