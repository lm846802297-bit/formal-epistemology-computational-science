# 2. The Osterwalder–Schrader Formalization Network

## 2.1. The mathematical setting

The Osterwalder–Schrader programme establishes conditions under which Euclidean field-theoretic data can be related to relativistic quantum field theory. Its Euclidean objects are Schwinger functions; the reconstructed relativistic objects are Wightman functions or distributions. The original OS papers formulate axioms for Euclidean Green functions and develop the corresponding reconstruction theorem (Osterwalder & Schrader, 1973, 1975). Osterwalder and Schrader (1975, pp. 282, 287–288) identify a gap in the 1973 forward proof and leave open there whether E0–E4 alone suffice. Their Section IV reconstruction theorem assumes E0′ together with E1–E4 and yields the output bound R0′.

The mathematical setting is not unique. Glimm and Jaffe (1987) formulate the Euclidean theory in terms of a probability measure on field configurations and its generating functional. The original OS formulation, by contrast, is expressed in terms of Schwinger functions as distributions on an appropriate test-function space. Douglas, Hoback, et al. (2026) choose the Glimm–Jaffe formulation for their Lean formalization because it makes the construction of a Euclidean field theory a problem about a functional measure, a mathematical structure well supported by Mathlib. They explicitly note that this is a variant of the original OS axioms and explain the relationship between their use of Schwartz functions and the compactly supported test functions in the Glimm–Jaffe presentation. Glimm and Jaffe (1987, p. 91, n. 1) also discuss the Schwartz-space extension and the free-field measure on tempered distributions. The three formalization projects considered below should therefore be understood as related representations of the OS programme, not as interchangeable encodings of a single record.

## 2.2. OSforGFF: the probability-measure formulation

At commit fef84a82937dfd2bb7f672108a72da329d3ef0fd, OSforGFF (Cherkis et al., 2026) constructs the massive Gaussian free field as a probability measure on the space of tempered distributions S'(R^D), where D ≥ 2 is the spacetime dimension. The generic theorem takes a propagator instance. The corollary gaussianFreeField_satisfies_all_OS_axioms_of_dim supplies the canonical proper-time propagator for every D ≥ 2; separate results exhibit closed-form covariances in D = 2, 3, 4, and 5. The principal theorem, gaussianFreeField_satisfies_all_OS_axioms_generic, proves that the constructed measure satisfies the project's bundled Glimm–Jaffe OS properties. The repository reports zero sorry declarations and no project-specific axioms for the pinned library theorem; these claims are understood relative to its Lean environment and foundational dependencies.

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

These choices are not merely notational. The OSforGFF documentation and the accompanying paper explain how the formalized conditions relate to the Glimm–Jaffe presentation. In particular, the use of Schwartz test functions and tempered distributions is stated to imply the corresponding compactly supported test-function formulation, since D(R^D) is contained in S(R^D) and S'(R^D) is contained in D'(R^D). The Lean predicate gives mean-square convergence for finite exponential functionals. Following Douglas et al. (2026, Remark 3.2), the finite-exponential result is read as a route to the L1(μ) ergodicity statement: density in L1(μ), the L2-to-L1 implication on a probability space, and invariance of μ under time translations extend the time-average result to general integrable observables. These are substantive correspondence claims, but the extension to general L1(μ) observables is attributed to the formalization paper's Remark 3.2 rather than presented as a direct quotation from the accessible pages of Glimm and Jaffe.

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

The package also formalizes the original-coordinate version of the OS-II growth condition. Its OSIIOriginalLinearGrowthCondition requires a positive Sobolev index s and, for n > 0, the estimate

\[
\|S_n(f)\|
\leq
\alpha (n!)^\gamma
\|f\|_{\mathrm{OSII},ns},
\]

where the final seminorm is the original-coordinate seminorm on the zero-diagonal test space. A separate normalization is imposed at n = 0. The public arity-linear condition instead uses the maximum of the relevant Schwartz seminorms with weight and derivative orders bounded by ns, and allows the coefficient \(\alpha\beta^n(n!)^\gamma\). The theorem os_to_wightman_osii_original converts the original-coordinate record into the arity-linear record with the explicit parameter choice

\[
\alpha' = \max\{1,\alpha\},\qquad
\beta'=(d+2)^s,\qquad
\gamma'=\gamma+2s.
\]

It then concludes three results: existence of a Wick-paired Wightman family, the output growth estimate R0-prime, and uniqueness among Wightman families satisfying the same Wick-pairing relation. The conversion is a proved quantitative interface, not an identification by terminology. The package explicitly distinguishes this corrected arity-dependent condition from an earlier fixed-order growth predicate that it does not treat as an equivalent reconstruction input.

The reverse theorem constructs Euclidean Schwinger data from a Wightman-function family and proves the corresponding OS properties for that constructor. It does not assume the forward growth condition. The two directions therefore do not form an unconditional biconditional between arbitrary OS data and arbitrary Wightman data. The public endpoint is a family of Wightman distributions satisfying the formalized Wightman-function axioms, including covariance, spectral support, locality, positivity, Hermiticity, and clustering. The package explicitly places the subsequent GNS construction of a Hilbert space and operator-valued fields outside its scope.

The public OSreconstruction package includes a conditional constructor that produces an OS record from a supplied Wightman family. What it does not expose is a standalone concrete model in the public package that supplies both the forward OS record and the corrected growth witness. Its README reports that a private companion project contains examples for the massive free field and the Proca Wick square. This is evidence that the authors report such examples; the private proof artifacts are not independently inspectable here. The reported massive-free-field inhabitant is not thereby identified with the particular probability-measure object constructed by OSforGFF at the pinned revision. Establishing that identity or an appropriate correspondence is precisely an inter-formalization task.

## 2.4. Comparator: an explicit bridge between formal records

The OSreconstruction-comparator project (Douglas, Yin, et al., 2026), pinned at commit 93cdb40e728ba27b7b1b55efc30d57f7b43de9aa, provides a Mathlib-only challenge and a solution for the three reconstruction propositions. Its notion of independence is specific. The challenge does not import the production package. RegistryChallenge.lean reuses the package's mathematical declarations: the 460-line mathematical block corresponds to the declarations in verification/comparator/Definitions.lean, while the generator consolidates the five Mathlib imports into one, revises the header comment, and appends three theorem obligations. Thus the mathematical declarations are reused unchanged, but the entire source file is not reproduced verbatim. The challenge is a separately elaborated checking surface, not an independently authored mathematical specification or a second derivation by a separate research team.

The bridge files provide the important mathematical content. OSBridge.lean constructs conversions in both directions between the challenge's OS record and the production OsterwalderSchraderAxioms record. The Schwinger family is preserved definitionally, and the two conversions satisfy round-trip identities. The adapters transport the growth records in both directions. The Wick-pairing and output-growth predicates are definitionally equivalent, while the original-coordinate seminorms are definitionally equal. Solution.lean then proves the equivalences eToR_iff, eToROSII_iff, and rToE_iff between the challenge statements and the production specifications for the forward theorem, the OS-II theorem, and the reverse constructor. The reverse bridge also identifies the Schwinger family with the output of its specified constructor. These equivalences preserve the underlying distribution families.

The configured proof targets are e_to_r, e_to_r_osii, and r_to_e; the three equivalence lemmas eToR_iff, eToROSII_iff, and rToE_iff provide the adapters used by their solutions. The Comparator checks that the challenge and solution share structurally corresponding declarations, that the proof dependencies remain within the stated whitelist of Lean's foundational axioms, and that the proofs can be replayed through a fresh kernel and NanoDa. The archived workflow run for the pinned commit records acceptance of the solution by both NanoDa and the default Lean kernel. The project itself describes the repository as a thin wrapper containing no new mathematics. Its epistemic contribution is consequently not an independent mathematical discovery. It is a separately checked interface that makes the relation between a public theorem specification and the production formalization explicit and auditable. The challenge definitions reuse the source project's mathematical declarations, while the record adapters and theorem equivalences provide the bridge to the production records. The distinction between these roles is important: the challenge is separate at the import and checking boundary, but not independent in authorship or mathematical origin.

The Comparator documentation also states several restrictions that delimit the propositions being checked. The forward tube includes an additional condition on the first imaginary coordinate; locality is formulated for adjacent transpositions rather than stated directly in its full permutation form; and reflection positivity is implemented through a totalized coercion that maps a test function failing the zero-diagonal condition to zero. The growth condition remains a forward hypothesis and is not recovered by the reverse construction. These are not erased by proof replay: the Comparator certifies the stated propositions with these conventions. Its formalization metadata labels the review status self-assessed and lists no external reviewers, while reporting review among the project authors. The checking boundary is therefore separate from the production imports, but it should not be described as an independent external audit.

## 2.5. What is and is not connected in the public formalization network

The projects exhibit different kinds of correspondence evidence. For OSforGFF, the authors explain how the probability-measure predicates relate to the Glimm–Jaffe axioms, including the Schwartz-space/test-function relation and the dense finite-exponential class used in the ergodicity argument. For the Comparator, the bidirectional record adapters and the three theorem equivalences are themselves expressed by Lean declarations. The Comparator challenge reuses the production package's mathematical declarations but elaborates them across a separate import and checking boundary. This is a proved audit-to-production interface between separately elaborated records of common provenance, not a second, independently authored physical formalization. It shows how a formal interface can itself become an object of mathematical proof, while delimiting the level at which that proof warrants reuse.

Across the three pinned public revisions examined here—OSforGFF, OSreconstruction, and the Comparator—we found no declaration deriving, from the particular OSforGFF probability measure, both the required zero-diagonal Schwinger record and the arity-dependent growth witness used by the OSreconstruction forward theorem. Establishing such a composition would require a map from the probability measure and generating functional to the relevant Schwinger distributions, a proof that the OS predicates transfer to the zero-diagonal formulation, and an inhabitant of the precise growth record. This is a bounded source-inspection finding about these public revisions; it does not show that such a derivation is mathematically impossible or unavailable in another or private development. The private companion report is not an inspectable substitute for this specific public bridge.

The significance of the case does not depend on treating the missing public interface as a defect in either mathematical project. Each project proves the propositions it states. The issue is whether, and under what conditions, their results can be composed to support a further scientific claim. This is a question about the warrant of the interfaces between formalizations, not about the validity of the local proofs.
