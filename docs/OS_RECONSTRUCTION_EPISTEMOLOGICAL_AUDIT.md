# OS Reconstruction: Epistemological Case Audit

**Updated:** 2026-11-27  
**Status:** Source-critical account of fixed public artifacts. The manuscript corrections are based on the 50-claim audit at `audit/submission-source-check-2026-11-27`, commit `b5c4ce03b1157e2af018ff857cf7b166ec1b3ee7`. No new Lean build, proof replay, or physical computation was performed.

## 1. Executive conclusion

The three developments establish different results and expose different interfaces.

1. **OSforGFF** constructs a massive Gaussian free field as a probability measure on tempered distributions and proves the Glimm–Jaffe probability-measure formulation of the OS properties for every spacetime dimension \(D\geq2\), when supplied with a propagator instance. Its canonical-propagator corollary supplies the proper-time propagator for every \(D\geq2\); separate results give closed-form covariances in \(D=2,3,4,5\). Its OS1 predicate is an exponential bound on the generating functional with a subsidiary two-point integrability condition. For the massive GFF, the proof uses \(p=2\) and \(c=1/(2m^2)\). OS4 includes clustering and a mean-square ergodicity predicate for a specified class of finite exponential functionals.
2. **OSreconstruction** takes Schwinger distributions on a zero-diagonal Schwartz test-function space and proves conditional reconstruction theorems. Its forward theorem requires the OS record and an arity-dependent growth condition. The original-coordinate OS-II condition is imposed for \(n>0\), with a separate normalization at \(n=0\), and is converted by a proved theorem into the arity-linear growth record. The stronger forward result supplies the output \(R'_0\) bound and uniqueness among Wightman families with the same Wick pairing. The reverse theorem constructs an OS record from a supplied Wightman family without a forward growth hypothesis. The public endpoint is a family of Wightman distributions, not a GNS/operator construction.
3. **Comparator** supplies a separately elaborated Mathlib-only challenge and proves bridges to the production records. Its mathematical declaration block reuses 460 lines from the production package's audit definitions. The whole source file is not reproduced verbatim: five Mathlib imports are consolidated into one, the header is revised, and three theorem obligations are appended. Bidirectional record adapters preserve the Schwinger family and growth records; the Wick-pairing and output-growth predicates are definitionally equivalent, while the original-coordinate seminorms are definitionally equal. Three theorem equivalences relate the challenge and production forward, OS-II, and reverse propositions.

The positive Comparator result is a **same-provenance, audit-to-production record interface**, not a bridge between independently authored physical formalisms or an independent validation of the shared physical specification. The cross-project OSforGFF-to-OSreconstruction question is separate. Across the three pinned public revisions examined, no declaration was found deriving both the required zero-diagonal Schwinger record and the arity-dependent growth witness from the particular OSforGFF probability measure. This is bounded negative evidence about those public revisions, not a claim that such a derivation is mathematically impossible or unavailable elsewhere.

## 2. Exact source pins and claims

### 2.1 OSforGFF and the QFT formalization paper

- Repository: https://github.com/mrdouglasny/OSforGFF
- Commit: `fef84a82937dfd2bb7f672108a72da329d3ef0fd`
- Software authors in `formalization.yaml`: Sergey A. Cherkis, Michael R. Douglas, Sarah Hoback, Anna Mei, and Ron Nissim.
- Generic theorem: `gaussianFreeField_satisfies_all_OS_axioms_generic`.
- Canonical-propagator corollary: `gaussianFreeField_satisfies_all_OS_axioms_of_dim`, for every \(D\geq2\).
- The generic theorem takes a propagator instance. The all-dimensions corollary supplies the canonical proper-time propagator; closed-form covariance results are also provided in dimensions 2, 3, 4, and 5.
- OS1 is the Glimm–Jaffe exponential generating-functional bound, with the two-point integrability condition when \(p=2\). The proof uses \(p=2\), \(c=1/(2m^2)\), and the free covariance kernel.
- OS4 separates clustering from ergodicity. The Lean predicate establishes mean-square convergence for finite exponential functionals. Douglas, Hoback, Mei, and Nissim (2026, Remark 3.2) explain the density argument in \(L^1(\mu)\), the \(L^2\)-to-\(L^1\) estimate on a probability space, and the role of time-translation invariance in extending the time-average result to general integrable observables.
- The related QFT paper, Douglas et al. (2026), treats the four-dimensional free scalar field and lists OS reconstruction as a subsequent milestone. The later all-\(D\geq2\) corollary is a result of the pinned OSforGFF library and is attributed to Cherkis et al. (2026), not to the four-dimensional paper.
- The paper's Remark 3.1 explains the Schwartz-space/compact-support relation. Glimm and Jaffe (1987, second edition, p. 91 n. 1) also discuss the Schwartz-space extension and the free-field measure on tempered distributions.
- The repository reports zero `sorry` declarations and no project-specific axioms for the pinned library theorem. The corresponding `#print axioms` guard lists the foundational dependencies `propext`, `Quot.sound`, and `Classical.choice`. This is a source-reported status of the pinned library, not a claim that the proof has no foundational axioms or that a new Lean run was performed here.

**OS4 source boundary:** the public preview of Glimm and Jaffe used in the source audit contains pp. 90–91, including the OS4 heading and p. 91 n. 1, but not the continuation containing the full OS4 quantifiers, norm, and time-average formula. The \(L^1(\mu)\) extension is therefore attributed to Douglas et al. (2026, Remark 3.2), not presented as a direct quotation from the inaccessible textbook continuation.

### 2.2 OSreconstruction

- Repository: https://github.com/xiyin137/OSreconstruction
- Commit: `cf0904e34a7c146a9f312f601e3707dca4a87697`
- Package: `os-reconstruction/`; Lean 4.35.0-rc4; Mathlib commit `1f414401f69059aa7eead47b53ee40bd38455eeb`.
- Euclidean input: a family of Schwinger distributions on the zero-diagonal Schwartz test-function space. Wightman output: distributions on the full Schwartz space.
- The forward theorem `os_to_wightman` takes `OsterwalderSchraderAxioms` and `OSLinearGrowthCondition`.
- The original-coordinate condition `OSIIOriginalLinearGrowthCondition` requires \(s>0\) and, for \(n>0\), the estimate
  \[
  \|S_n(f)\|\leq \alpha (n!)^\gamma\|f\|_{\mathrm{OSII},ns},
  \]
  together with a separate normalization at \(n=0\). The conversion to the arity-linear record uses
  \[
  \alpha'=\max\{1,\alpha\},\qquad
  \beta'=(d+2)^s,\qquad
  \gamma'=\gamma+2s.
  \]
- The stronger OS-II theorem establishes existence of a Wick-paired Wightman family, the output \(R'_0\) bound, and uniqueness among families satisfying the same Wick-pairing relation. This uniqueness is uniqueness of the distribution family, not a claim that all physical realizations are unique.
- The reverse constructor `wightman_to_os_axioms` produces an OS record from a supplied Wightman family. This conditional constructor is not a published concrete model that supplies both the forward OS record and the corrected growth witness.
- The README reports examples for the massive free field and Proca Wick square in a private companion revision (reported as `03bb758`). The private repository/revision was not publicly inspectable in this audit. The evidence establishes that the package authors report these witnesses; it does not independently verify the private proofs or identify the massive-free-field witness with the pinned OSforGFF measure.
- The package's public endpoint is a Wightman distribution family. The subsequent GNS Hilbert-space and operator-valued-field construction is outside its stated scope.

### 2.3 OSreconstruction Comparator

- Repository: https://github.com/mrdouglasny/OSreconstruction-comparator
- Commit: `93cdb40e728ba27b7b1b55efc30d57f7b43de9aa`.
- `RegistryChallenge.lean` reuses the 460-line mathematical declaration block corresponding to `verification/comparator/Definitions.lean`. The whole file is not copied verbatim: imports are consolidated, the header comment is revised, and three theorem obligations are appended.
- `OSBridge.lean` defines conversions in both directions between the challenge OS record and the production `OsterwalderSchraderAxioms` record. Round-trip identities are proved, and the Schwinger family is preserved definitionally.
- Growth records are transported in both directions. `wickPair_iff` and `outputGrowth_iff` are definitional equivalences; `originalSeminorm_eq` is a definitional equality.
- `Solution.lean` proves `eToR_iff`, `eToROSII_iff`, and `rToE_iff`, relating the challenge and production forward, OS-II, and reverse propositions. The reverse bridge also identifies the returned Schwinger family with the output of its specified constructor.
- Configured proof targets are `e_to_r`, `e_to_r_osii`, and `r_to_e`. The archived 2026-11-03 workflow run for the pinned commit records acceptance of the solution by NanoDa and the default Lean kernel. This audit read the historical workflow record; it did not rerun the proof.
- The challenge imports Mathlib but not the production package; the solution elaborates the audit definitions and adapters before using production theorems. Project metadata describes review as self-assessed and lists no external reviewers. The independence is at the import/elaboration/checking boundary, not in mathematical authorship or physical specification.

The challenge also states specific conventions: the forward tube imposes a condition on the first imaginary coordinate; locality is expressed through adjacent transpositions; reflection positivity uses a totalized coercion that sends test functions outside the zero-diagonal subspace to zero; and the growth condition remains a forward hypothesis rather than being recovered by the reverse construction. These details delimit the propositions that the Comparator checks.

## 3. Interface analysis

| Interface | Public evidence | Status |
|---|---|---|
| OSforGFF predicates to the Glimm–Jaffe presentation | Pinned repository definitions and Douglas et al. (2026), Remarks 3.1–3.2 | Correspondence explained by the authors; the OS4 textbook continuation remains for author verification |
| Comparator records to production OSreconstruction records | `OSBridge.lean`, `Solution.lean`, and archived workflow run | Explicit bidirectional record and theorem correspondence between separately elaborated records of common provenance |
| OSforGFF measure to OSreconstruction forward input | No end-to-end declaration in the three pinned public revisions | Not established by the inspected public artifacts |
| Concrete OSreconstruction forward OS/growth input for the massive free field | README report of a private companion project | Author-reported; private proof artifacts not independently inspected |
| Wightman distributions to GNS/operator theory | Explicitly outside the package endpoint | Not established by this formalization |

## 4. Epistemological interpretation

The Comparator is a limited positive case of record-level interface warrant: the audit-to-production correspondence is itself expressed and checked in Lean, so production results can be reused under the separately elaborated challenge records. Because the challenge reuses the production package's mathematical declarations, this does not independently validate the physical adequacy of the shared specification.

The OSforGFF-to-OSreconstruction relation is a distinct cross-project composition problem. The two packages use different mathematical records and test-function domains. OSforGFF's OS1 is a bound on the generating functional for a single test function; OSreconstruction's forward theorem requires a quantitative bound on an arity-indexed family of Schwinger distributions. Similar terminology about regularity or growth does not supply the map, predicate transfer, or growth witness needed for composition.

The negative finding is deliberately bounded. The source audit inspected the three pinned public revisions, including the 60 OSforGFF Lean files, 855 OSreconstruction Lean files, and 2 Comparator Lean files, together with imports, dependencies, and the forward input types. It found no declaration deriving the particular OSforGFF measure's zero-diagonal Schwinger record and growth witness. This does not show that such a derivation is mathematically impossible, or that no implementation exists outside those public revisions.

## 5. Author verification still required

1. Obtain and inspect the continuation of Glimm and Jaffe (1987), second edition, §6.1(i), to verify the OS4 quantifiers, norm, time-average formula, and the dense-class/\(L^1(\mu)\) extension.
2. Personally verify all 23 cited works and the 50 mapped claim/evidence records. The source audit is a guide to the exact passages and repository declarations; it does not replace author approval.
3. Confirm that the manuscript's bounded negative finding and same-provenance characterization of the Comparator match the intended philosophical argument.

No Lean kernel was rerun, no new proof replay was performed, and no numerical or physical computation was added during this source-audit integration.
