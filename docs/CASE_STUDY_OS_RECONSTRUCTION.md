# Case Study: Machine-Checked Osterwalder-Schrader Reconstruction

The full source-critical analysis is in [OS_RECONSTRUCTION_EPISTEMOLOGICAL_AUDIT.md](OS_RECONSTRUCTION_EPISTEMOLOGICAL_AUDIT.md). This file is the concise source-pin and scope summary.

## A. OSforGFF

Repository: https://github.com/mrdouglasny/OSforGFF  
Commit: `fef84a82937dfd2bb7f672108a72da329d3ef0fd` (2026-08-31).

- Lean: `v4.33.0-rc1`; Mathlib: `79d0395a1825a6264ad5d269e35e60537518955e`.
- GaussianField: `ddb7102eb0515e420944b731ac66f8b4c29a9341`; BochnerMinlos: `58405ecd328cf8383a1c0b53d37605fe61a0b3f6`.
- Constructs the massive Gaussian free field as a probability measure on S'(R^D); D is spacetime dimension, D>=2. A generic theorem and all-D corollary are supplied, with explicit propagator instances for D=2,3,4,5.
- Master theorem: `gaussianFreeField_satisfies_all_OS_axioms_generic`; all-D corollary: `gaussianFreeField_satisfies_all_OS_axioms_of_dim`.
- README reports Version 3.2, ~25,500 lines, zero sorry and zero project axioms. The Lean foundations remain part of the trust base.
- Bundles OS0 analyticity, OS1 regularity, OS2 Euclidean invariance, OS3 reflection positivity, OS4 clustering, and OS4 ergodicity.
- Crucial: OSforGFF OS1 is an exponential generating-functional bound plus a subsidiary two-point integrability condition. It is not definitionally the separate OS-II arity-dependent `OSLinearGrowthCondition`.

## B. OSreconstruction

Repository: https://github.com/xiyin137/OSreconstruction  
Source commit: `cf0904e34a7c146a9f312f601e3707dca4a87697`; package `os-reconstruction/`.

- Lean: `leanprover/lean4:v4.35.0-rc4`; Mathlib: `1f414401f69059aa7eead47b53ee40bd38455eeb`; GaussianField: `e28a381288f0c6cdd275f9fd84cfb1b20feea957`.
- Here d is positive spatial dimension; spacetime has dimension d+1. Euclidean data act on zero-diagonal Schwartz tests; Wightman distributions act on full Schwartz space.
- `os_to_wightman`: OS E0–E4 plus arity-dependent `OSLinearGrowthCondition` imply existence of a Wick-paired Wightman-function family.
- `os_to_wightman_osii_original`: OS-II E0' input implies existence, output R0' growth, and uniqueness among Wick-paired families.
- `wightman_to_os`: reverse construction has no forward growth hypothesis. The two directions do not form an unconditional biconditional.
- `WightmanFunctions` is a distributional Wightman record. Operator/GNS reconstruction is explicitly outside the package.
- The growth condition is a precise arity-dependent Sobolev/seminorm estimate, not a synonym for OSforGFF's OS1.

### Growth-condition inhabitants

The distributable package README says the OS and corrected growth input records are not inhabited *inside this package*. It also reports that a private companion project `math-commons/yang-mills` proves inhabitants for the massive free field and Proca Wick square. That companion is private and was not independently inspected. Therefore do not say no examples exist; say the public package does not expose them, while the authors report private companion inhabitants.

## C. Comparator

Repository: https://github.com/mrdouglasny/OSreconstruction-comparator  
Commit: `93cdb40e728ba27b7b1b55efc30d57f7b43de9aa`.

- Thin wrapper; contains no independent mathematics of its own.
- Mathlib-only Challenge reproduces the definitions and states three proof obligations; Solution discharges them from the production package.
- Comparator checks structural correspondence and replays proofs with a fresh kernel and NanoDa, under the whitelist `propext`, `Classical.choice`, `Quot.sound`.
- This is an independent specification/checking interface, not an independent mathematical derivation by a second research team and not empirical validation.
- Disclosed conventions: extra first-coordinate forward-tube condition; locality for adjacent transpositions; reflection positivity via totalized coercion onto zero-diagonal tests; growth is a forward hypothesis, not a reverse conclusion.

## D. Composition boundary

OSforGFF uses D for spacetime dimension; OSreconstruction uses d for spatial dimension and d+1 for spacetime. Four-dimensional spacetime corresponds to OSforGFF D=4 and OSreconstruction d=3.

The public repositories do not expose a single end-to-end theorem that instantiates the exact OSreconstruction growth input from the pinned OSforGFF artifact. The private companion reportedly contains concrete inhabitants, but is not independently inspectable. The projects also use different Lean/Mathlib revisions and distinct formal records/test-space interfaces.

No Lake build or proof replay was run by this project. Existing results are reused at exact commits.