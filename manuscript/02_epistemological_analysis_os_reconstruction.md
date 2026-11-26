# 2. Epistemological Analysis of Osterwalder–Schrader Reconstruction

## 2.1. The mathematical and physical setting

The Osterwalder–Schrader programme concerns the relation between Euclidean field-theoretic data and relativistic quantum field theory. In the Euclidean formulation, the central objects are Schwinger functions. Under appropriate conditions, these data can be related by analytic continuation to Wightman functions satisfying relativistic covariance, positivity, locality, and spectral properties. The original OS papers formulate axiomatic conditions for Euclidean Green functions and establish a reconstruction programme connecting Euclidean and relativistic descriptions (Osterwalder and Schrader 1973).

The sequel is essential to the precise statement of the reconstruction result. Osterwalder and Schrader (1975) explicitly extend and correct the earlier paper and introduce the additional linear growth condition usually denoted E0-prime. Thus, the forward reconstruction result cannot be represented accurately as a consequence of the OS axioms E0–E4 alone. The quantitative growth hypothesis is part of the mathematical content of the corrected theorem.

The Lean projects considered here formalize different parts of this programme. OSforGFF formalizes a concrete massive Gaussian free-field model and its OS properties. OSreconstruction formalizes conditional theorems relating Euclidean Schwinger data and Wightman-function distributions. The Comparator project checks an independently stated version of the reconstruction propositions against the production package. These are related contributions, but they are not a single formal development with an already demonstrated end-to-end instantiation.

## 2.2. OSforGFF: a concrete Euclidean model

OSforGFF constructs the massive Gaussian free field as a probability measure on the space of tempered distributions S'(R^D). Its README identifies the construction as dimension-generic for spacetime dimension D greater than or equal to two, with explicit propagator instances for D=2, 3, 4, and 5, and a general corollary based on the proper-time propagator. The principal theorem is

**gaussianFreeField_satisfies_all_OS_axioms_generic**.

The theorem states that the specified massive Gaussian free-field measure satisfies the bundled OS properties under the stated dimension, mass, and propagator assumptions. The bundle includes:

- OS0: analyticity of the generating functional;
- OS1: regularity;
- OS2: Euclidean invariance;
- OS3: reflection positivity;
- OS4: clustering;
- an additional ergodicity property recorded alongside OS4.

The repository reports that the master theorem and its dimension-specific instances are fully proved, with no sorry and no project-specific axioms, at the pinned revision. This report should be understood relative to the declared Lean environment and its foundational trust base. The present paper reuses the result and does not claim to have independently rebuilt or replayed the proof.

The epistemic content of this theorem is substantial. It is not merely a proof that an abstract list of properties is mutually consistent. The project constructs a particular probability measure and proves that its associated generating functional satisfies the formalized OS conditions. The result therefore establishes a strong model-internal mathematical claim about the specified massive Gaussian free-field construction.

The scope of that claim must nevertheless be stated precisely. OSforGFF defines OS1 through an exponential bound on the generating functional, with a subsidiary two-point integrability and convergence condition in the borderline case. This predicate is not definitionally identical to the arity-dependent OS-II growth condition used in OSreconstruction. Similar terminology does not establish equivalence between two formal predicates.

Nor does the theorem, by itself, establish the empirical adequacy of the free-field model for an interacting physical system. It establishes mathematical properties of the specified Euclidean model. Whether and how that model is used to represent a physical target is a further scientific question.

## 2.3. OSreconstruction: conditional reconstruction of Wightman functions

The OSreconstruction package formalizes the forward and reverse relations between Euclidean Schwinger-function data and relativistic Wightman-function distributions. Its dimensional convention differs from that of OSforGFF: here d is the positive spatial dimension and spacetime has dimension d+1. Consequently, four-dimensional spacetime corresponds to D=4 in OSforGFF and d=3 in OSreconstruction.

The Euclidean input is formulated on a zero-diagonal Schwartz test-function space. The package emphasizes that this is the appropriate test space for the Euclidean data in its OS-I/OS-II formulation; the Wightman distributions, by contrast, act on the full Schwartz space. This distinction is mathematically relevant because the passage from zero-diagonal Euclidean test functions to full-Schwartz Wightman distributions is part of the reconstruction problem itself.

### 2.3.1. The forward theorem

The public theorem **os_to_wightman** has the following schematic form:

\[
\mathrm{OS}(S)\land \mathrm{Growth}(S)
\Longrightarrow
\exists W\; \mathrm{WickPair}(S,W).
\]

More explicitly, the theorem takes an OS record satisfying the package's E0–E4 conditions and a separate **OSLinearGrowthCondition**. It concludes that there exists a Wightman-function family whose distributions are Wick-paired with the input Schwinger family.

The growth condition is quantitative and arity-dependent. In the package specification, it has the schematic form

\[
\|S_n(f)\|
\leq
\alpha\,\beta^n\,(n!)^\gamma\,
\|f\|_{ns,ns},
\]

where alpha is positive, beta is positive, gamma is real, and the Schwartz seminorm orders increase linearly with the arity n. The precise formal definition includes a normalization condition at arity zero and a bound for every arity and every zero-diagonal test function.

This is not merely the statement that each Schwinger function is continuous or tempered. It is a uniform family-level estimate with specified dependence on the number of arguments. It is therefore a substantive premise of the reconstruction theorem.

### 2.3.2. The OS-II theorem

The package also formalizes the stronger OS-II form of the forward theorem. With the original-coordinate growth condition, it concludes:

1. existence of a Wick-paired Wightman-function family;
2. an output coordinate-norm growth condition corresponding to R0-prime;
3. uniqueness among Wightman-function families satisfying the same Wick-pairing relation.

The uniqueness statement is relative to the specified Wick-pairing condition. It is not a claim that every possible physical interpretation or every possible operator realization has been uniquely determined by the formal theorem.

The output remains a family of Wightman distributions. The package explicitly states that full GNS reconstruction of a Hilbert space and operator-valued fields is outside its endpoint. The standard mathematical reconstruction programme may motivate such a further step, but it should not be attributed to this particular formalized package.

### 2.3.3. The reverse theorem

The reverse direction constructs Schwinger-function data from a Wightman-function family and proves the corresponding OS properties for the constructed Euclidean data. This reverse theorem does not assume the forward OS-II growth condition.

The asymmetry is important. The package's forward theorem is conditional on the Euclidean growth premise; the reverse construction does not recover that premise as a conclusion. The two directions therefore should not be summarized as an unconditional biconditional between arbitrary OS data and arbitrary Wightman data.

### 2.3.4. What the public package does and does not contain

The distributable OSreconstruction package states that the OS input record and the corrected growth-condition record are not inhabited within that package. Its README also reports that a private companion project contains examples, including the massive free field and the Proca Wick square, satisfying the corrected input conditions. Since that companion is private, its proof details are not independently inspectable in the present study.

The correct conclusion is consequently limited: the public package exposes and proves a conditional reconstruction theorem, while the authors report concrete inhabitants in a separate private development. It would be inaccurate to infer that no model satisfies the growth condition. It would be equally inaccurate to claim that the public OSforGFF artifact has already been formally connected to the exact growth input of the pinned OSreconstruction package.

## 2.4. Comparator: an additional formal checking interface

The OSreconstruction-comparator repository provides a Mathlib-only challenge specification and a corresponding solution. The challenge reproduces the relevant mathematical definitions and states the three reconstruction obligations without importing the production package. The solution discharges those obligations using the production development. The Comparator workflow checks the correspondence between the challenge and solution and reports proof replay using a fresh kernel and NanoDa, with the stated whitelist of Lean's foundational axioms.

This provides a valuable additional layer of formal scrutiny. It makes the target propositions available in a separate specification interface and checks that the production solution proves those propositions under the stated checking procedure. It should not, however, be described as a second independent mathematical derivation by another research team. The comparator repository describes itself as a thin wrapper containing no mathematics of its own.

The Comparator documentation also makes several formalization conventions explicit. These include an additional condition on the first imaginary coordinate in the forward tube, locality stated for adjacent transpositions, reflection positivity expressed through a totalized coercion onto zero-diagonal test functions, and the placement of growth as a forward hypothesis rather than a reverse conclusion. These conventions are part of the exact propositions being checked. A philosophical analysis should therefore discuss the formalized theorem as stated, not silently replace it with a broader textbook formulation.

## 2.5. The interface between the three projects

The relation between OSforGFF and OSreconstruction is not established simply by observing that both projects concern Osterwalder–Schrader axioms.

There are at least four distinct interfaces.

**First, the formal records differ.** OSforGFF packages its result through a probability measure and generating-functional formulation. OSreconstruction takes a family of Schwinger distributions on a zero-diagonal Schwartz test space. A formal map between these records is required before the output of one project can be used directly as the input of the other.

**Second, the growth predicates differ.** OSforGFF's OS1 regularity condition is not definitionally the same as OSreconstruction's arity-dependent OS-II growth condition. A proof connecting them, or an independently verified inhabitant of the latter for the former model, is needed for direct composition.

**Third, the dimension conventions differ.** OSforGFF uses D for spacetime dimension, while OSreconstruction uses d for spatial dimension and d+1 for spacetime. A four-dimensional comparison therefore uses D=4 and d=3.

**Fourth, the Lean environments differ.** The inspected OSforGFF revision uses Lean 4.33.0-rc1, whereas the inspected OSreconstruction package uses Lean 4.35.0-rc4, with different Mathlib and GaussianField dependency pins. Their theorems are established in their respective environments; direct import or composition is not supplied merely by the separate proof results.

The public artifacts inspected do not expose one end-to-end theorem that takes the specific OSforGFF construction and proves that it inhabits the exact OSreconstruction growth-condition record at the pinned revisions. This is a statement about the public interface inspected, not a claim that such a mathematical relation is impossible or that the authors' private companion work does not establish it.

## 2.6. The epistemic structure of the case

The OS case can now be analyzed through the DDI distinction between denotation, demonstration, and interpretation.

### Denotation

OSforGFF specifies a mathematical probability model: the massive Gaussian free field on a space of tempered distributions, with a covariance determined by the chosen propagator construction. OSreconstruction specifies a Euclidean Schwinger-function family on a particular test-function space. These mathematical objects have intended physical interpretations within Euclidean field theory, but the relation between two formal records must be established by an appropriate map. A shared physical label does not itself prove formal equivalence.

### Demonstration

The Lean developments provide machine-checked demonstrations of their respective claims. OSforGFF proves the bundled OS properties for its specified Gaussian free-field construction. OSreconstruction proves conditional reconstruction theorems from its exact OS and growth hypotheses. The Comparator adds an independent statement/checking interface for the three reconstruction propositions.

This is where machine checking contributes most directly. It makes the mathematical demonstration explicit, checks the proof objects relative to the declared formal systems, and allows assumptions and theorem endpoints to be audited. It does not remove the need to examine what has been formalized.

### Interpretation

The physical interpretation connects Euclidean Schwinger data, reflection positivity, analytic continuation, and relativistic Wightman distributions. The OS framework provides the mathematical and physical context for understanding why these structures matter. Yet the formalized reconstruction endpoint considered here is a Wightman-function distribution family. The construction of the corresponding Hilbert space and operator-valued fields is not part of the package's stated endpoint.

### Target-directed warrant

A theorem about the massive Gaussian free field establishes a mathematical property of that model. To use it as a claim about a physical target, one must specify the target, the purpose of the model, and the relevant model-to-target relation. A free-field model may be used as an exact representation of a free theory, as an idealization, or as a component of a larger approximation. The machine-checked OS properties alone do not determine which use is justified, nor do they establish empirical adequacy for an interacting system.

## 2.7. Claim-to-evidence summary

| Claim | Evidence in the formal artifacts | Additional warrant required |
|---|---|---|
| The specified massive GFF satisfies the OS properties bundled by OSforGFF | Master theorem and dimension-generic corollary at the pinned OSforGFF commit | Correspondence of the formal record to the intended source formalism |
| OS data plus the corrected growth premise yield a Wick-paired Wightman family | **os_to_wightman** at the pinned OSreconstruction commit | Instantiation of the exact OS and growth hypotheses by a concrete model |
| The OS-II form adds an output growth bound and uniqueness among Wick-paired families | **os_to_wightman_osii_original** | Interpretation of the distributional endpoint; no operator/GNS claim follows from this package alone |
| Wightman data generate Euclidean data satisfying the specified OS record | Reverse constructor and **r_to_e_specification** | Assessment of the intended physical interpretation and scope |
| The production theorems match the comparator challenge and pass the specified replay | Comparator challenge, solution, metadata, and reported replay | This is formal checking, not empirical validation or a second independent derivation |
| The concrete OSforGFF model satisfies the exact OSreconstruction growth input | Not shown as an end-to-end public theorem in the inspected artifacts | A public bridge or inspectable inhabitant proof is needed |

The table makes the epistemic structure explicit. The formal artifacts establish strong mathematical results. The remaining questions are not defects in those results; they concern the relations required to use them as claims about a model or a physical target.
