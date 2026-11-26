# Case Study: Machine-Checked Osterwalder-Schrader Reconstruction

Evidence snapshot: 2026-11-26. Three repositories must be distinguished.

## A. OSforGFF
https://github.com/mrdouglasny/OSforGFF
- Commit: `fef84a82937dfd2bb7f672108a72da329d3ef0fd` (2026-08-31).
- Lean `v4.33.0-rc1`; Mathlib `79d0395a1825a6264ad5d269e35e60537518955e`.
- GaussianField `ddb7102eb0515e420944b731ac66f8b4c29a9341`; BochnerMinlos `58405ecd328cf8383a1c0b53d37605fe61a0b3f6`.
- Constructs massive Gaussian free field on S'(R^d), dimension-generic d>=2, with instances d=2,3,4,5; proves OS0 analyticity, OS1 regularity, OS2 Euclidean invariance, OS3 reflection positivity, OS4 clustering/ergodicity.
- README reports ~25,500 Lean lines, zero sorry, zero custom axioms. AXIOM_AUDIT says headline results depend on Lean's three core axioms: propext, Classical.choice, Quot.sound.
- OS1 regularity is not automatically the specific `OSLinearGrowthCondition` required by the separate reconstruction package.

## B. OSreconstruction
https://github.com/xiyin137/OSreconstruction
- Source commit `cf0904e34a7c146a9f312f601e3707dca4a87697` (2026-11-03), package `os-reconstruction/`.
- Lean `v4.35.0-rc4`; Mathlib `1f414401f69059aa7eead47b53ee40bd38455eeb`; GaussianField `e28a381288f0c6cdd275f9fd84cfb1b20feea957`.
- Package reports zero sorry and zero project-specific axioms; standard Lean foundations remain.
- Euclidean data act on zero-diagonal Schwartz tests; Wightman distributions act on full Schwartz space.
- E'->R: OS axioms E0-E4 plus arity-dependent linear growth yield Wick-paired Wightman distributions.
- E'->R': OS II form also yields output coordinate-norm growth and uniqueness among Wick-paired Wightman families.
- R->E: Wightman family yields Schwinger functions satisfying E0-E4; reverse theorem does not assert forward growth.
- Forward theorem requires both OS axioms and `OSLinearGrowthCondition`. README says neither input is inhabited within this package. It reports a private companion with examples, not independently inspectable here. Operator/GNS reconstruction is explicitly not an endpoint.

## C. Comparator
https://github.com/mrdouglasny/OSreconstruction-comparator
- Commit `93cdb40e728ba27b7b1b55efc30d57f7b43de9aa`.
- Mathlib-only challenge and solution proved from package; describes Comparator and fresh-kernel/NanoDa replay. This audits the challenge/solution interface, not an independent derivation by another research team and not empirical validation.
- Scope conventions: extra forward-tube condition; adjacent-transposition locality; reflection positivity via totalized coercion onto zero-diagonal tests; growth as forward hypothesis, not reverse conclusion.

## D. Composition boundary
OSforGFF constructs a Euclidean free field and proves OS properties. OSreconstruction proves a conditional theorem from OS axioms plus exact arity-dependent growth to Wightman distributions. Public repositories inspected do not expose a single end-to-end theorem instantiating that exact condition from OSforGFF. Do not identify OS1 regularity with the exact growth condition without a proved bridge. Do not claim no such composition exists; the inspected public interface does not show it. The projects use different Lean/Mathlib revisions.

No Lake build was rerun. Commits, manifests, toolchains, repository axiom audits, and Comparator artifacts were inspected and recorded. Existing results are reused rather than recomputed. A separate `cherkis/OSreconstruction` repository is a different development and must not be conflated with `xiyin137/OSreconstruction`.