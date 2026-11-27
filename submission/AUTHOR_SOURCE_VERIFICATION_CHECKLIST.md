# Author-led source verification checklist

**Manuscript:** *Machine-Checked Proofs and Formalization Interfaces in Mathematical Physics: The Epistemology of Osterwalder–Schrader Reconstruction*  
**Branch:** `research/initial-literature-review`  
**Status:** All 23 entries are pending the submitting author's personal verification. The 50-claim source audit is recorded in `docs/PRE_SUBMISSION_SOURCE_AUDIT_INTEGRATION.md`; prior metadata checks and assistant source inspections do not count as author completion.

For each item, read the original source or inspect the exact pinned repository revision; verify the manuscript paraphrase; record the exact page, section, theorem, or source-file location; correct any inaccurate statement or reference; and only then mark the item complete.

| No. | Source | Manuscript location | Specific claims to verify | Exact source locator | Author status |
|---:|---|---|---|---|---|
| 1 | Al Wardani, Chaudhuri & Miller (2023) | Introduction; §3.2 | DAMF's assertion exchange, provenance records, and configurable trust in assertion creators/tools; distinguish formal assertion transfer from scientific interpretation. | DOI 10.1007/978-3-031-43369-6_10 | [ ] Pending author check |
| 2 | Bobbin et al. (2024) | Introduction; §§3.2, 3.5 | Shared structures for thermodynamics/kinematics; interoperable proofs for gas laws and equations of motion; distinction between mathematical verification and empirical adequacy. | DOI 10.1039/D3DD00077J | [ ] Pending author check |
| 3 | Cherkis et al. (2026), OSforGFF | Abstract; Introduction; §§2.2, 2.5; Conclusion | Pinned repository authorship; dimension-generic massive GFF construction; theorem gaussianFreeField_satisfies_all_OS_axioms_generic; OS0–OS4; OS1 p=2 and c=1/(2m^2); two-point condition; OS4 clustering/ergodicity; reported sorry/axiom status. | Commit fef84a82937dfd2bb7f672108a72da329d3ef0fd; inspect formalization.yaml, Axioms.lean, OS1_Regularity.lean, OS4 files, Master.lean. | [ ] Pending author check |
| 4 | Contessa (2007) | §3.4 | Surrogative reasoning and inference from model properties to target claims; verify that the text's summary captures Contessa's own account. | DOI 10.1086/519478 | [ ] Pending author check |
| 5 | DeDeo & Duede (2026) | Introduction; §§3.1, 3.5 | Representation vs tracking; §3 library lock-in/shared models; §4 structural, causal, explanatory routes to correspondence; ensure our distinction is complementary and does not claim novelty for correspondence/library dependence. | arXiv:2603.13680v2; Philosophy of Science forthcoming. | [ ] Pending author check |
| 6 | Douglas, Hoback, Mei & Nissim (2026), Formalization of QFT | Introduction; §§2.1–2.2; §3.1 | Glimm–Jaffe probability-measure formulation; variant relation to original OS axioms; Schwartz vs compact support; ergodicity/density argument; OS reconstruction as a later milestone. | arXiv:2603.15770v1 | [ ] Pending author check |
| 7 | Douglas, Yin & Mei (2026), Comparator | Abstract; Introduction; §§2.4–2.5; §§3.2–3.3; Conclusion | 460-line mathematical declaration block reused from production Definitions.lean; imports/header/three obligations differ; separate import/elaboration boundary; bidirectional record adapters and round-trip identities; Schwinger-family/growth/Wick-pairing preservation; eToR_iff, eToROSII_iff, rToE_iff; configured targets e_to_r, e_to_r_osii, r_to_e; historical NanoDa/default-kernel run; self-assessed review status. | Commit 93cdb40e728ba27b7b1b55efc30d57f7b43de9aa; inspect generator, RegistryChallenge.lean, RegistrySolution.lean, OSBridge/WightmanBridge/ReverseBridge and archived CI logs. | [ ] Pending author check |
| 8 | Frigg & Nguyen (2018) | §3.4 | DEKI terminology (denotation, exemplification, keying, imputation) and the role of mappings in attributing model properties to targets. | DOI 10.1007/s13194-017-0182-4 | [ ] Pending author check |
| 9 | Gelfert (2009) | Introduction; §3.3 | Hubbard–Heisenberg example and the transfer of empirical warrant through mathematically rigorous cross-model relations. | DOI 10.1007/s11229-008-9431-6 | [ ] Pending author check |
| 10 | Gelfert (2011) | Introduction; §3.1 | Limitations of DDI/matching-model accounts; mature mathematical formalisms as heterogeneous inferential and interpretative resources; avoid overstating the author's thesis. | DOI 10.1016/j.shpsa.2010.11.035 | [ ] Pending author check |
| 11 | Gelfert (2022) | Introduction | Epistemic actions and activities involving notations; verify the brief characterization and its relevance to the paragraph. | DOI 10.1007/978-3-030-97833-4_11 | [ ] Pending author check |
| 12 | Glimm & Jaffe (1987) | §§2.1–2.2 | Probability-measure and generating-functional formulation; p. 91 n. 1 on Schwartz extension and the free-field measure on tempered distributions. **Author must obtain and read the continuation of §6.1(i) containing OS4, and verify its exact quantifiers, norm, time-average formula, and the dense-class/L1 extension.** The public preview used in the source audit did not include these continuation pages. | 2nd ed.; §6.1(i), pp. 90–91 and continuation; DOI 10.1007/978-1-4612-4728-9 | [ ] Pending author check |
| 13 | Guilloud et al. (2025) | Introduction; §3.2 | SC-TPTP's transfer/reconstruction of derivations across automated and interactive theorem provers, including Lean; verify exact supported systems and what is reconstructed. | DOI 10.1007/978-3-031-99984-0_18 | [ ] Pending author check |
| 14 | Hughes (1997) | Introduction; §3.1 | DDI's denotation, demonstration, and interpretation; check that the summary is faithful to Hughes rather than later DDI revisions. | DOI 10.1086/392611 | [ ] Pending author check |
| 15 | Imbert & Ardourel (2023) | Introduction | Epistemological heterogeneity of computational science and context-dependent epistemic roles of verification. | DOI 10.1017/psa.2022.78 | [ ] Pending author check |
| 16 | Knuuttila (2021) | §3.4 | Models as epistemic artifacts and modal/exploratory knowledge without an actual target; verify the exact scope. | DOI 10.1007/s13194-021-00374-5 | [ ] Pending author check |
| 17 | Meadows, Zhang & Freitas (2026) | Introduction; §3.5 | FormalScience's human-in-the-loop autoformalization; semantic drift, notational collapse, and abstraction elevation; check exact definitions/examples. | DOI 10.18653/v1/2026.acl-long.1057 | [ ] Pending author check |
| 18 | Osterwalder & Schrader (1973) | §2.1 | Original Euclidean Green-function axioms and the scope of the original reconstruction result; read with the 1975 correction and do not attribute E0-prime to 1973. | DOI 10.1007/BF01645738 | [ ] Pending author check |
| 19 | Osterwalder & Schrader (1975) | §§2.1, 2.3 | Corrected reconstruction theorem and E0-prime linear growth condition; verify exactly which forward-theorem hypotheses are required and how the 1973 claim is corrected. | DOI 10.1007/BF01608978 | [ ] Pending author check |
| 20 | Parker (2020) | §3.4 | Adequacy-for-purpose account; distinguish mathematical/structural suitability from quantitative/empirical adequacy. | DOI 10.1086/708691 | [ ] Pending author check |
| 21 | Rabe (2017) | Introduction; §3.2 | Theory morphisms, compositional translations, judgment preservation, and induced model reduction; verify the precise theorem/terminology. | DOI 10.1016/j.tcs.2017.07.006 | [ ] Pending author check |
| 22 | Suárez (2004) | §3.4 | Inferential conception of scientific representation and its role in model-to-target inference. | DOI 10.1086/421415 | [ ] Pending author check |
| 23 | Yin, Douglas & Mei (2026), OSreconstruction | Abstract; §§2.1, 2.3–2.5; §§3.2–3.3; Conclusion | Zero-diagonal Schwartz space; OsterwalderSchraderAxioms; OSLinearGrowthCondition; original-coordinate OS-II growth conversion; forward endpoint as Wightman distributions; reverse theorem's lack of forward growth assumption; private companion claims. | Commit cf0904e34a7c146a9f312f601e3707dca4a87697; inspect theorem declarations and README. | [ ] Pending author check |

## Author completion record

- Author name: ______________________________
- Date source audit completed: ______________________________
- Source items requiring correction: ______________________________
- Manuscript changes made after source audit: ______________________________
- Final author approval: [ ] Approved [ ] Not yet approved

**Acceptance rule:** the source audit is complete only when all 23 entries have been personally checked by the submitting author and resulting corrections have been incorporated. Metadata matching alone is not sufficient.


## Reference-list policy point for author decision

The manuscript cites three public GitHub software artifacts (OSforGFF, OSreconstruction, and OSreconstruction-comparator) as version-pinned research materials. EJPS instructions say the reference list should include works cited in the text and published or accepted for publication. The author should confirm with the editorial office that software repositories are acceptable as software references. If the journal requires a narrower interpretation, preserve exact commit hashes and repository URLs in a footnote or suitable data/code-availability statement, while retaining the associated scholarly papers in the reference list where applicable. Do not remove the version information needed to reproduce the source analysis.


## Additional source-audit author check

The 50-claim audit found no support for treating the OSforGFF OS1 exponential generating-functional bound as the OSreconstruction arity-dependent growth witness. The manuscript now distinguishes these predicates and limits the public absence claim to the three pinned revisions. The author should confirm that this wording matches the intended philosophical argument; it does not assert mathematical impossibility.
