# OS Reconstruction: Epistemological Case Audit

**Date:** 2026-11-26  
**Status:** Source-critical analysis of public artifacts at fixed commits. No Lean build, proof replay, or new proof was performed by this project.

## 1. Executive conclusion

The three projects establish different things.

1. **OSforGFF** reports a kernel-checked construction of the massive Gaussian free field as a probability measure on tempered distributions and a proof that its generating functional satisfies the project's OS0–OS4 package for spacetime dimension D >= 2. The result is a concrete Euclidean free-field model with a specified covariance construction and stated analytic, regularity, invariance, reflection-positivity, clustering, and ergodicity properties.
2. **OSreconstruction** proves conditional mathematical reconstruction statements. Its forward theorem takes a Euclidean Schwinger family on the zero-diagonal Schwartz test space, the OS E0–E4 record, and a separate arity-dependent OS-II growth hypothesis. It concludes existence of a Wick-paired Wightman-function family. Its OS-II version additionally proves an output growth bound and uniqueness among Wick-paired families. The reverse theorem constructs Euclidean Schwinger functions from a Wightman-function family without the forward growth hypothesis.
3. **OSreconstruction-comparator** presents an independent Mathlib-only challenge specification and a solution discharged from the production package, then checks structural correspondence and proof replay with Comparator/NanoDa under the stated standard-axiom whitelist. It is an independent formal statement/checking interface, not an independent mathematical derivation by a second research group and not empirical validation.

The projects do **not** constitute one publicly demonstrated end-to-end proof that the specific OSforGFF object satisfies the exact OSreconstruction growth input. A separate companion project is described by OSreconstruction as containing examples of the corrected growth condition, including a massive free field and a Proca Wick square, but that companion is private. This is evidence reported by the package authors, not a source that we independently inspected. In addition, the public projects use different formal records, test-space conventions, dimensional conventions, and Lean/Mathlib pins.

The principal philosophical result is therefore not that machine proof fails. It is that machine proof provides a strong, local deductive warrant whose scope is exactly the formal proposition, assumptions, definitions, and trust base checked. The transition to a concrete model and then to a physical interpretation requires additional, separately stated relations.

## 2. Evidence and exact source pins

### 2.1 OSforGFF

- Repository: https://github.com/mrdouglasny/OSforGFF
- Commit: `fef84a82937dfd2bb7f672108a72da329d3ef0fd`
- Master theorem source: `OSforGFF/OS/Master.lean`
- Axiom definitions: `OSforGFF/OS/Axioms.lean`
- Project README reports Version 3.2 (August 2026), approximately 25,500 lines, zero `sorry`, and zero project axioms.
- README states that the massive GFF is constructed as a probability measure on S'(R^D), with dimension-generic theorem for spacetime dimension D >= 2 and concrete propagator instances for D=2,3,4,5. A corollary covers all D >= 2 through the proper-time propagator.
- Master theorem: `gaussianFreeField_satisfies_all_OS_axioms_generic`; all-dimensions corollary: `gaussianFreeField_satisfies_all_OS_axioms_of_dim`.
- The master record bundles OS0 analyticity, OS1 regularity, OS2 Euclidean invariance, OS3 reflection positivity, OS4 clustering, and OS4 ergodicity. The README's duplicate OS4 label is its convention: clustering and ergodicity are both recorded as OS4-related components.

**What this establishes:** conditional on the declared Lean foundations, imports, definitions, and theorem statement, the specified massive Gaussian free-field measure has the bundled properties in this formalization for the stated dimensions and propagator assumptions.

**What it does not establish by itself:** the OS-II arity-dependent growth condition used by the separate reconstruction package; a Wightman reconstruction theorem for this exact object; the full operator/GNS reconstruction; or empirical adequacy of the free-field model for a particular physical system.

**Important precision:** OSforGFF's OS1 is defined through an exponential bound on its generating functional, with a subsidiary two-point integrability/convergence condition in the p=2 case. It is not definitionally identical to the separate OSreconstruction package's `OSLinearGrowthCondition`.

### 2.2 OSreconstruction

- Repository: https://github.com/xiyin137/OSreconstruction
- Source commit: `cf0904e34a7c146a9f312f601e3707dca4a87697`
- Package: `os-reconstruction/`
- Specification: `OSReconstruction/Specification.lean`
- Wightman output record: `OSReconstruction/Specification/Wightman.lean`
- Public theorem interface: `OSReconstruction/Wightman/Reconstruction/Main.lean`
- Exact target contract: `verification/Contracts.lean`
- Comparator mathematical definitions: `verification/comparator/Definitions.lean`
- Lean toolchain: `leanprover/lean4:v4.35.0-rc4`
- Mathlib commit: `1f414401f69059aa7eead47b53ee40bd38455eeb`
- GaussianField dependency commit: `e28a381288f0c6cdd275f9fd84cfb1b20feea957`

The package treats d as a **positive spatial dimension**; spacetime has dimension d+1. The Euclidean input acts on zero-diagonal Schwartz test functions, while Wightman distributions act on full Schwartz space.

#### Forward E' -> R

The public theorem `os_to_wightman` has the shape:

```lean
theorem os_to_wightman (OS : OsterwalderSchraderAxioms d)
    (linear_growth : OSLinearGrowthCondition d OS) :
    ∃ Wfn : WightmanFunctions d,
      IsWickRotationPair OS.schwinger Wfn.W
```

Thus the conclusion is existence of a Wightman-function family Wick-paired with the Euclidean Schwinger family. The `WightmanFunctions` record carries the formalized distributional properties, including continuity/temperedness, normalization, translation and Lorentz covariance, analytic forward-tube/boundary-value data, positive spectral support, positive definiteness, Hermiticity, locality, and clustering.

The forward theorem is **conditional** on both the OS E0–E4 record and the separate `OSLinearGrowthCondition`.

#### OS II E' -> R'

The theorem `os_to_wightman_osii_original` takes the original-coordinate OS-II growth condition and concludes:
- existence of a Wick-paired Wightman family;
- the output coordinate-norm growth condition R0' (4.3);
- uniqueness among Wightman-function families satisfying the same Wick-pair relation.

The output is still a Wightman-function family. The package explicitly states that operator/GNS reconstruction is not an endpoint.

#### Reverse R -> E

The theorem `wightman_to_os` constructs Schwinger functions with continuity, linearity, and the Wick-pair relation; the specification contract also checks the corresponding OS axioms for the constructor. This reverse direction has no forward OS-II growth hypothesis. Therefore the two public directions do not, by themselves, yield an unconditional biconditional between arbitrary OS data and arbitrary Wightman data.

#### Exact growth hypothesis

In `Specification.lean`, `OSLinearGrowthCondition` abbreviates an arity-linear bound. It includes:
- normalization at arity zero;
- a fixed Sobolev/seminorm index parameter s;
- positive constants alpha and beta and a real exponent gamma;
- for every arity n and zero-diagonal test function f, a bound of the form

$$
\|S_n(f)\| \leq
\alpha\,\beta^n\,(n!)^\gamma\,
\|f\|_{n s,n s}.
$$

The seminorm uses Schwartz weights/derivative orders that grow linearly with n. This is a specific quantitative condition on the whole family of Schwinger distributions, not merely the qualitative assertion that each S_n is a tempered distribution.

The README explains that the earlier fixed-order condition forced s=0 at arity zero and excluded the intended massive free field in spatial dimension 3; the corrected arity-linear condition is used instead. This correction matters philosophically: the formal theorem's assumptions are not generic “regularity” but a precise, arity-dependent estimate.

#### Inhabitants and public boundary

The package README says neither the OS-axiom record nor the corrected growth record is inhabited **inside this distributable package**. It also identifies a private companion project, `math-commons/yang-mills`, which reportedly vendors the records and proves inhabitants for the massive free field and the Proca Wick square, using only the three standard Lean axioms. That project is private and was not independently inspected in this audit.

Consequently, the correct statement is not “no model satisfies the growth hypothesis.” The correct statement is: the public OSreconstruction package proves a conditional theorem; it does not itself expose a public inhabitant of its corrected input records. The authors report concrete inhabitants in a private companion development.

### 2.3 Comparator

- Repository: https://github.com/mrdouglasny/OSreconstruction-comparator
- Commit: `93cdb40e728ba27b7b1b55efc30d57f7b43de9aa`
- `formalization.yaml` pins the substantive source repository to the exact OSreconstruction commit above.
- The comparator repository says it contains no mathematics of its own. Its Challenge is a Mathlib-only specification, reproducing the package's definitions and exposing three proof obligations; its Solution discharges those obligations using the package.
- The README says Comparator checks structural correspondence of shared constants and replays proofs with a fresh kernel and NanoDa, under a whitelist of Lean's three core axioms: `propext`, `Classical.choice`, and `Quot.sound`.
- The comparator is not a second independent proof development by a separate research team. It is an independently stated challenge/solution interface around the production package and a separate proof-checking/replay mechanism.

Four scope conventions are explicitly disclosed:
1. The formalized forward tube has an extra condition on the imaginary part of the first coordinate, making it a proper subset of the literal n-point forward tube for n>0.
2. Locality is stated for adjacent transpositions.
3. Reflection positivity is stated through a totalized coercion onto zero-diagonal test functions.
4. Growth is a forward hypothesis, not a reverse conclusion.

These are not incidental implementation details: they specify the exact mathematical content that the Comparator is checking.

## 3. Original mathematical context

The primary sources are:
- Osterwalder & Schrader (1973), “Axioms for Euclidean Green's Functions,” Communications in Mathematical Physics 31, 83–112, DOI 10.1007/BF01645738. The paper states necessary and sufficient conditions for Euclidean Green's functions to define a unique Wightman field theory and develops E->R and R->E.
- Osterwalder & Schrader (1975), “Axioms for Euclidean Green's Functions II,” Communications in Mathematical Physics 42, 281–305, DOI 10.1007/BF01608978. The authors explicitly say that the sequel extends and corrects the previous paper; it introduces the linear growth condition E0' and the corrected E'->R' reconstruction result.

The 1975 correction is central. The philosophical case must not present the 1973 E0–E4 list alone as the sufficient reconstruction input. The formalized OS-II growth condition is the additional quantitative premise that makes the corrected forward theorem applicable.

## 4. The interface map

| Interface | What is available | What remains distinct |
|---|---|---|
| OSforGFF definitions -> OSforGFF master theorem | Public Lean theorem bundles OS0–OS4 properties for the specified massive GFF | The result is within OSforGFF's probability-measure/generating-functional formulation |
| OSforGFF OS record -> OSreconstruction OS record | Both concern Euclidean Schwinger data and OS-type conditions | Formal records, test spaces, definitions, dimension conventions, and Lean/Mathlib versions differ |
| OSreconstruction OS record -> forward reconstruction | Public theorem proves E'->R under OS axioms plus corrected arity-linear growth | Concrete inhabitance of both inputs is outside the public package |
| Concrete GFF -> corrected growth input | Private companion project is reported to prove the massive free-field inhabitant | No public end-to-end theorem from the pinned OSforGFF artifact into the pinned OSreconstruction input was inspected |
| OSreconstruction theorem -> Comparator challenge | Comparator states the target independently in a Mathlib-only challenge and proves it from the package | Comparator is not empirical validation and not a second independent derivation |
| Wightman functions -> physical QFT | Formal output record contains distributional Wightman properties | Operator/GNS construction and application to a specific physical target are outside this package |

Dimension conventions must be normalized before any attempted composition: OSforGFF uses D for spacetime dimension with D>=2; OSreconstruction uses d for spatial dimension with spacetime dimension d+1 and d>=1. In particular, the familiar four-dimensional spacetime comparison is OSforGFF D=4 against OSreconstruction spatial d=3.

The two principal packages also use different Lean/Mathlib versions. A direct import/composition is not established by their separate theorem statements.

## 5. What machine checking contributes

The contribution is substantial and specific:

1. **Deductive closure:** each declared theorem follows from its formal assumptions in the specified Lean environment.
2. **Assumption visibility:** the forward growth premise is explicit and cannot be silently replaced by a vague appeal to “regularity.”
3. **Statement precision:** quantifiers, test spaces, arity dependence, domains, and theorem endpoints are encoded.
4. **Regression protection:** the Comparator checks that the public theorem statements match the independently stated challenge and that the solution passes the specified replay checks.
5. **Auditability:** exact source revisions, dependencies, and proof artifacts can be inspected.

The machine check does not by itself establish:
- that the formal records are the uniquely correct formalization of the original OS papers;
- that the OSforGFF object inhabits the exact growth record of the separate package, unless the explicit bridge/inhabitant is inspected;
- that the formalized conventions are equivalent to every textbook convention;
- that Wightman functions have been extended to a Hilbert space and operator-valued fields by this package;
- that the free field is an adequate model of a particular interacting physical system or experiment.

## 6. Formalization-aware DDI analysis

### Denotation

OSforGFF denotes a specific mathematical probability model: the massive Gaussian free field measure on a tempered-distribution configuration space, with a covariance fixed by the chosen propagator. OSreconstruction's input denotes a family of Euclidean Schwinger distributions on the zero-diagonal test space. The correspondence between these two records is not automatic merely because both are called “OS data.”

### Demonstration

OSforGFF machine-checks the construction and OS-property theorem. OSreconstruction machine-checks conditional reconstruction from its exact axioms and growth hypothesis. Comparator checks the three declared theorem statements against a Mathlib-only challenge and performs the specified proof replay.

This is where machine verification adds its strongest local warrant.

### Interpretation

The physical interpretation uses the OS framework: Euclidean correlation functions, reflection positivity, analytic continuation, and Wightman distributions. The meaning of the mathematical objects and the adequacy of the model for a target remain tied to the original physical theory and its interpretative practice.

### Target-directed warrant

The free GFF is an exact mathematical model of a free scalar field under its assumptions. Its formal OS properties do not establish empirical adequacy for an interacting theory, a lattice approximation, or a specific observed system. Such claims require separate model construction, approximation/limit arguments, and empirical or theoretical support appropriate to the purpose.

## 7. Core philosophical argument

The case supports a precise claim:

**A machine-checked reconstruction theorem establishes a conditional mathematical relation between specified Euclidean and Wightman data. It does not, solely by being machine-checked, establish that a concrete Euclidean model satisfies every reconstruction hypothesis, that the formal objects exhaust the intended physical formalism, or that the resulting theory adequately describes a physical target.**

This does not diminish the mathematical achievement. It identifies its epistemic scope. Machine checking strengthens Demonstration; the Denotation and Interpretation obligations remain separately assessable.

## 8. Corrections to earlier project notes

The following clarifications supersede imprecise earlier wording:

1. Do not say that OSreconstruction has no known concrete inhabitants of the corrected growth condition. Its README reports a private companion project with massive GFF and Proca Wick-square inhabitants. Say instead that the public package itself does not expose these inhabitants and that the private companion was not independently inspected.
2. Do not call the Comparator a wholly independent proof by another research team. It is an independent Mathlib-only challenge and a Comparator/NanoDa replay wrapper around the production package.
3. Do not describe OSforGFF's OS1 regularity as the OSreconstruction growth hypothesis. They are distinct formal predicates.
4. Do not say OSforGFF D=4 directly matches OSreconstruction d=4. The latter uses spatial dimension d and spacetime dimension d+1; four-dimensional spacetime corresponds to d=3.
5. Do not describe the public package as constructing the full Hilbert-space/operator QFT. Its stated endpoint is Wightman-function distributions.
6. Do not treat the 1973 E0–E4 list as the corrected sufficient reconstruction input without the 1975 E0' growth condition.

## 9. Audit status

- Exact repository commits inspected: yes.
- Key Lean specification, theorem interface, Wightman record, Comparator definitions, and Comparator metadata inspected: yes.
- Original 1973/1975 paper metadata and abstracts checked against publisher/Project Euclid records: yes.
- Fresh Lean build or proof replay by this project: no.
- Numerical calculation: none.
- Upstream fork or source modification: none.
- Remaining material uncertainty: the private companion's concrete growth-condition inhabitants and a public, exact bridge from OSforGFF's formal record to OSreconstruction's input record are not independently inspectable in the public artifacts reviewed.
