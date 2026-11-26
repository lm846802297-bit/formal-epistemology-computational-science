# OS Reconstruction: Epistemological Case Audit (revised)

**Date:** 2026-11-26  
**Status:** Source-critical analysis of public artifacts at fixed commits. No Lean build, proof replay, or new proof was performed by this project.

## 1. Executive conclusion

The three developments establish different results and expose different interfaces.

1. **OSforGFF** constructs a massive Gaussian free field as a probability measure on tempered distributions and proves a dimension-generic package of Glimm–Jaffe OS properties for spacetime dimension D >= 2. The formalization uses Schwartz test functions and the generating-functional/probability-measure formulation. Its OS1 is an exponential generating-functional bound with a subsidiary two-point integrability condition; the GFF proof uses p=2 and c=1/(2m^2). OS4 is represented through clustering and an ergodicity condition on a specified class of finite exponential functionals. The accompanying QFT paper explains how these predicates relate to the Glimm–Jaffe compact-support formulation and the original ergodicity condition.
2. **OSreconstruction** takes Schwinger distributions on the zero-diagonal Schwartz test space. Its forward theorem requires E0–E4 and an arity-dependent growth condition. The OS-II original-coordinate growth condition is converted by a proved theorem into the arity-linear record used by the public forward theorem. The OS-II result additionally establishes the output R0-prime bound and uniqueness among Wick-paired families. The reverse theorem has no forward growth hypothesis. The output is a Wightman-function distribution family, not a GNS/operator construction.
3. **Comparator** reproduces the package's own Mathlib-only audit definitions as a challenge, then proves equivalences between the challenge records and production records. The bridges preserve the Schwinger family, transfer growth records, and identify Wick-pairing and output-growth predicates. Comparator and NanoDa provide structural and proof-replay checks. This is a separate import/checking boundary and a formally proved record correspondence, not an independently authored specification or a second mathematical derivation by another research team.

The public artifacts do not expose an end-to-end theorem that instantiates the exact OSreconstruction zero-diagonal OS and growth input from the particular OSforGFF probability-measure construction at the pinned revision. The OSreconstruction README reports a private companion development with massive-free-field and Proca-Wick-square inhabitants of the corrected input records. This is author-reported evidence; the private code was not independently inspected, and the reported massive-free-field inhabitant is not thereby identified with the specific OSforGFF object.

## 2. Exact source pins

### OSforGFF
- Repository: https://github.com/mrdouglasny/OSforGFF
- Commit: fef84a82937dfd2bb7f672108a72da329d3ef0fd
- Authors in formalization.yaml: Sergey A. Cherkis, Michael R. Douglas, Sarah Hoback, Anna Mei, Ron Nissim.
- Master theorem: gaussianFreeField_satisfies_all_OS_axioms_generic.
- OS1: OS1_Regularity in OSforGFF/OS/Axioms.lean; GFF proof in OSforGFF/OS/OS1_Regularity.lean.
- OS4: clustering and ergodicity are separate predicates; ergodicity is proved from polynomial clustering.
- Formalization paper: Douglas, Hoback, Mei, and Nissim (2026), arXiv:2603.15770.
- The formalization paper says the Schwartz/tempered-distribution formulation implies the corresponding Glimm–Jaffe compact-support formulation. It also explains the restricted exponential-functional class and L2-to-L1 argument for ergodicity.

### OSreconstruction
- Repository: https://github.com/xiyin137/OSreconstruction
- Commit: cf0904e34a7c146a9f312f601e3707dca4a87697
- Package: os-reconstruction/
- Lean: 4.35.0-rc4; Mathlib commit 1f414401f69059aa7eead47b53ee40bd38455eeb.
- Euclidean data: zero-diagonal Schwartz test functions.
- Wightman data: full Schwartz distributions with covariance, spectral support, locality, positivity, Hermiticity, and clustering.
- Forward theorem: os_to_wightman assumes OsterwalderSchraderAxioms and OSLinearGrowthCondition.
- OS-II theorem: os_to_wightman_osii_original takes OSIIOriginalLinearGrowthCondition, converts it to the arity-linear record, and concludes Wick pairing, R0-prime, and uniqueness.
- Reverse theorem: Wightman data yield OS data via the explicit constructor without a growth hypothesis.
- GNS/operator reconstruction is outside the package endpoint.
- The README says the corrected OS/growth input records are not inhabited in the public package. It reports a private companion project that inhabits them for a massive free field and Proca Wick square.

### Comparator
- Repository: https://github.com/mrdouglasny/OSreconstruction-comparator
- Commit: 93cdb40e728ba27b7b1b55efc30d57f7b43de9aa.
- The challenge reproduces verbatim the package's Mathlib-only audit definitions from verification/comparator/Definitions.lean; it does not import the production package.
- OSBridge.lean constructs conversions in both directions between challenge and production OS records, preserves the Schwinger family definitionally, transfers arity-linear and original-coordinate growth records, and identifies Wick-pairing and output-growth predicates.
- Solution.lean proves eToR_iff, eToROSII_iff, and rToE_iff between challenge statements and production specifications.
- Comparator checks structural correspondence and proof replay through a fresh kernel and NanoDa under the stated three-foundational-axiom whitelist.
- The project describes itself as a thin wrapper with no mathematics of its own. Its independence is at the import/checking boundary, not in authorship or mathematical origin.

## 3. Interface analysis

| Interface | Public evidence | Status |
|---|---|---|
| OSforGFF predicates to Glimm–Jaffe source formulation | Formalization paper and repository definitions | Mathematical correspondence explained by authors |
| Comparator records to production OSreconstruction records | OSBridge.lean and Solution.lean | Explicitly formalized bidirectional record and theorem correspondence |
| OSforGFF model to OSreconstruction input record | No end-to-end public theorem at the pinned commits | Not established by inspected public artifacts |
| OSreconstruction growth input for massive free field | Private companion examples reported in README | Author-reported, not independently inspectable |
| Wightman distributions to GNS/operator theory | Explicitly outside package endpoint | Not established by this formalization |

## 4. Epistemological interpretation

The Comparator is a positive case of relative inter-formalization warrant: the interface itself is proved and checked, so the production theorem can be reused under a separate, Mathlib-only audit surface. Because the challenge definitions are copied from the same package's audit file, this does not independently validate the physical adequacy of the shared specification. The OSforGFF-to-OSreconstruction relation is a different case: the mathematical connection is plausible and relevant, and a private companion is reported, but the public artifacts do not expose the specific bridge needed to compose the pinned results.

The central issue is therefore not that any local proof fails. It is that the warrant of a composed result depends on the correspondence of the formal records, the transport of the exact hypotheses, and the preservation of the theorem's conclusion and witnesses.
