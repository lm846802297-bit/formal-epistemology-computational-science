# Research Decisions

- **DEC-001 (2026-11-26):** Focus the first paper on machine-checked proofs in physics, not all AI-generated science.
- **DEC-002:** Do not claim novelty for semantic fidelity, theorem correspondence, or proof tracking; engage DeDeo & Duede (2026) and FormalScience (2026).
- **DEC-003:** Distinguish formal derivability, model-internal claims, target-directed claims, and explanatory understanding.
- **DEC-004:** Reuse OSforGFF, OSreconstruction, and Comparator as primary case; Bobbin et al. (2024) secondary. No new Lean library now.
- **DEC-005:** Use axial anomaly only as a bounded physics stress test after primary-source checking. Do not claim it is formalized in cited Lean projects.
- **DEC-006:** No numerical computation in phase 1 or phase 2.
- **DEC-007:** Keep novelty provisional; no “first”, “unprecedented”, “complete”, or universal necessary-and-sufficient claim without evidence.
- **DEC-008:** OS reconstruction is the primary case, with exact source commits.
- **DEC-009:** Do not assume public packages compose automatically. OS1 regularity is not the exact OSLinearGrowthCondition absent a proved bridge.
- **DEC-010:** Submit substantive changes on a review branch and merge only after PR review.
- **DEC-011 (2026-11-26):** The broad claim that rigorous mathematical relations can transfer empirical warrant is already explicit in Gelfert (2009); it is not our novelty.
- **DEC-012:** Mature mathematical formalisms and their embedded inferential/interpretative commitments are directly addressed by Gelfert (2011); do not claim this concept as new.
- **DEC-013:** Adopt a formalization-aware DDI framework as the working analytical framework. Machine checking strengthens Demonstration; formalization correspondence, interpretation, and model-to-target warrant remain separate.
- **DEC-014:** Keep C_E explanatory understanding orthogonal, not a required serial stage. Permit modal/exploratory model knowledge without an actual target.
- **DEC-015:** Make model evaluation purpose-sensitive, following Parker (2020).
- **DEC-016:** Use Gelfert's Hubbard–Heisenberg case as the cross-model warrant comparison; keep OS reconstruction as the primary formalization case.
- **DEC-017 (2026-11-26):** Reuse the existing OSforGFF, OSreconstruction, and Comparator research results directly as prior mathematical/formalization results. Do not fork or reimplement them merely for convenience.
- **DEC-018:** Our independent contribution is the source-critical and epistemological analysis of the exact statements, assumptions, theorem endpoints, interpretation, and warrant interfaces. Cite original authors and pin exact commits.
- **DEC-019:** Treat repository-reported Lean checks and Comparator results as evidence about the specified formal artifacts and environments. Do not claim we independently rebuilt or reverified them unless we actually do so.
- **DEC-020:** A future fork or code modification is justified only if a concrete research question requires a new formal theorem, counterexample, or reproducible independent check. Any such work must be isolated from upstream and submitted through a review branch/PR.

## Scope lock

The paper concerns the epistemic role of machine-checked demonstration within mature mathematical formalisms in theoretical physics. It is not a general AI ethics paper, broad simulation-epistemology survey, or new QFT formalization project.

- **DEC-021 (2026-11-26):** The OS case is analyzed from exact public theorem declarations and source records; no OS proofs are reimplemented.
- **DEC-022:** OSforGFF uses D as spacetime dimension (D>=2); OSreconstruction uses d as spatial dimension with spacetime d+1 (d>=1). Four-dimensional spacetime corresponds to D=4 and d=3.
- **DEC-023:** OSforGFF's OS1 generating-functional exponential bound is not definitionally the OSreconstruction arity-dependent OS-II growth condition.
- **DEC-024:** The OSreconstruction public package does not expose inhabitants of its OS/growth input records; its README reports a private companion with massive GFF and Proca Wick-square inhabitants. Treat this as author-reported, not independently inspected.
- **DEC-025:** Comparator is an independent Mathlib-only challenge/checking interface with fresh-kernel/NanoDa replay, not a second independent mathematical derivation by another research team.
- **DEC-026:** The public OSreconstruction endpoint is a Wightman-function distribution family, not full GNS/operator reconstruction.
- **DEC-027:** The 1975 OS paper explicitly extends and corrects the 1973 reconstruction claim; any account of the sufficient forward hypothesis must include the E0' growth condition.

- **DEC-028 (2026-11-26):** Enter manuscript-development stage. Draft the Introduction, OS Reconstruction epistemological analysis, and Discussion using the completed literature review and source-critical audit.
- **DEC-029:** Do not expand the literature review or reimplement OS mathematics during the first manuscript draft. Use the existing public formalization results with exact commit attribution.
- **DEC-030:** The manuscript's contribution is the epistemological analysis of machine-checked Demonstration within mature mathematical formalisms, not a new general theory of scientific representation or cross-model empirical warrant.
- **DEC-031:** Distinguish explicitly between source inspection and independent Lean execution. No fresh build or proof replay is claimed in the manuscript.

- **DEC-032 (2026-11-26):** Manuscript prose must follow the conventions of peer-reviewed research articles in philosophy of science and philosophy of physics. Use argumentative continuous prose, author–year citations, selective headings, and restrained claims; exclude project-report language, progress narration, promotional phrasing, and unnecessary lists from the paper.

- **DEC-033 (2026-11-26):** The manuscript may draw on the writing conventions of any closely related peer-reviewed research paper, not only papers from a predetermined set of journals. Use Hughes (1997), Gelfert (2009, 2011), Imbert and Ardourel (2023), and DeDeo and Duede (2026) as complementary exemplars for conceptual precision, case-based argument, analysis of mathematical practice, and careful epistemic distinctions. Do not imitate distinctive wording or reproduce another paper's structure mechanically.

- **DEC-034 (2026-11-26):** Abstract and Conclusion are complete. The three core sections have undergone a whole-manuscript academic-style edit and are harmonized into `manuscript/full_manuscript.md`.
- **DEC-035:** The integrated manuscript is approximately 5,900 words excluding references; the abstract is approximately 204 words. The current draft is complete in structure but is not yet journal-formatted or submission-ready.
- **DEC-036:** The next phase is limited to final source/citation verification, target-journal selection, journal formatting, and copyediting. Do not expand the research question or add new technical work without a specific issue found in the review.

- **DEC-037 (2026-11-26):** Select the European Journal for Philosophy of Science as the primary target. Use its subscription publishing route to satisfy the no-author-APC requirement.
- **DEC-038:** Align in-text citations and references with EJPS's APA 7 author–date requirements; the abstract and six keywords already fit the journal's stated ranges.
- **DEC-039:** EJPS requires disclosure of LLM use in Methods or a suitable alternative section. Because ChatGPT was used for substantive literature discovery, argument organization, and drafting/revision, this use must be disclosed; it must not be mischaracterized as copy-editing only.
- **DEC-040:** Before submission, the author must personally verify all cited sources and formalization claims, revise the AI-assisted prose to reflect their own scholarly judgment, and take responsibility for the final manuscript.

- **DEC-041 (2026-11-26):** Major revision centers on the epistemic conditions for transferring machine-checked results across distinct formalizations of the same physical theory. Use the term **inter-formalization warrant** as a bounded analytical distinction, not a universal new theory.
- **DEC-042:** Distinguish local proof warrant, source-formalism correspondence, inter-formalization warrant, model instantiation, and target-directed warrant. These relations are not a mandatory linear pipeline.
- **DEC-043:** Comparator's Challenge reproduces the OSreconstruction package's own Mathlib-only audit definitions verbatim; its independence is at the import/checking boundary. OSBridge and Solution prove record and theorem equivalences, preserving the Schwinger family and growth predicates. Do not call it an independent mathematical derivation or independently authored specification.
- **DEC-044:** OSforGFF uses the Glimm–Jaffe probability-measure/generating-functional formulation. Its OS1 is the exponential generating-functional bound with a subsidiary two-point condition; for the GFF the proof uses p=2 and c=1/(2m^2). OS4 includes clustering and an ergodicity condition on a specified exponential-functional class. The QFT formalization paper explains its relation to Glimm–Jaffe's compact-support formulation and ergodicity condition.
- **DEC-045:** OSreconstruction distinguishes the arity-linear growth record from the original-coordinate OS-II E0-prime record; a proved conversion connects them. Preserve this distinction in the manuscript.
- **DEC-046:** Do not identify the private companion's massive-free-field inhabitant with the exact pinned OSforGFF object unless a public or independently inspectable bridge establishes that identity.
- **DEC-047:** Revise the working title to emphasize formalization interfaces; add Bobbin et al. (2024), Douglas et al. (2026) Formalization of QFT, and Glimm & Jaffe (1987) as primary sources.

- **DEC-048 (2026-11-26):** The manuscript title is revised to *Machine-Checked Proofs and Formalization Interfaces in Mathematical Physics: The Epistemology of Osterwalder–Schrader Reconstruction*.
- **DEC-049:** The complete manuscript now contains 20 cited references, a 213-word abstract, six keywords, and approximately 6,395 words of main text excluding abstract and references.
- **DEC-050:** One critical review of the new inter-formalization warrant argument is required before returning to EJPS LaTeX conversion.

- **DEC-051 (2026-11-26):** The major revision explicitly situates the argument against Rabe (2017) on theory morphisms, Al Wardani et al. (2023) on DAMF, and Guilloud et al. (2025) on SC-TPTP. These establish formal proof-preservation, assertion transfer, and proof-system interoperability; the paper must not claim those mechanisms as new.
- **DEC-052:** The paper's contribution is limited to the epistemological analysis of how formal interfaces between representations of physical mathematical formalisms interact with source-formalism correspondence, theorem-hypothesis instantiation, and scientific interpretation.

- **DEC-053 (2026-11-26):** Rabe (2017), Al Wardani et al. (2023), and Guilloud et al. (2025) are added to the literature comparison. The manuscript explicitly distinguishes theory morphisms, distributed assertion transfer, and SC-TPTP proof interoperability from its scientific-epistemic analysis.
- **DEC-054:** The integrated manuscript contains 23 cited references, a 211-word abstract, six keywords, and approximately 6,395 words of main text excluding abstract and references.

- **DEC-055 (2026-11-26):** Section 2 now states both OSreconstruction growth records and the proved parameter conversion from the original-coordinate OS-II condition to the arity-linear condition: alpha' = max(1, alpha), beta' = (d+2)^s, gamma' = gamma + 2s.
- **DEC-056:** The integrated manuscript contains 23 cited references, a 211-word abstract, six keywords, and approximately 6,395 words of main text excluding abstract and references.

- **DEC-057 (2026-11-26):** Comparator analysis now names eToR_iff, eToROSII_iff, and rToE_iff, and records the disclosed forward-tube, adjacent-locality, totalized-reflection-positivity, and growth-as-hypothesis conventions.
- **DEC-058:** Comparator review status is self-assessed with no external reviewers listed; it must not be described as an independent external audit.
- **DEC-059:** The integrated manuscript contains approximately 6,538 words of main text, 211 abstract words, six keywords, and 23 cited references.

- **DEC-060 (2026-11-26):** The Comparator's positive result is described as relative interface warrant: record and theorem correspondence is proved, but the copied challenge definitions do not independently validate the source specification's physical adequacy.
- **DEC-061:** The integrated manuscript contains 23 cited references, a 219-word abstract, six keywords, and approximately 6,693 words of main text excluding abstract and references.

- **DEC-041 (2026-11-26):** Reframe the paper around inter-formalization warrant: when a machine-checked theorem in one formalization can support an inference in another formalization of the same physical theory.
- **DEC-042:** Treat inter-formalization warrant as a bounded analytical label for the warrant supplied by an adequately established formal-record correspondence; do not claim a new universal theory or proof-transfer mechanism.
- **DEC-043:** Comparator is positive evidence of relative interface warrant: the challenge definitions reproduce the production package's own audit definitions, while explicit bridges and theorem equivalences are checked across a separate import/elaboration boundary. This does not independently validate source-formalism adequacy.
- **DEC-044:** The absence of a public OSforGFF-to-OSreconstruction instantiation is a public-interface boundary, not evidence that the mathematical connection is impossible or absent from private companion work.
- **DEC-045:** The major-revision review passed the predetermined conceptual and source-structure criteria. Proceed to author-led source verification and EJPS formatting; do not expand research scope without a concrete error.


- **DEC-062 (2026-11-27):** DeDeo and Duede (2026), especially Sections 3–4, already address library lock-in, shared-model hybridization across modelling traditions, and structural, causal, and explanatory routes to correspondence. Do not claim novelty for library dependence or correspondence in general.
- **DEC-063:** The paper's narrower question concerns source/receiving formal-record interfaces: object and predicate mapping, hypothesis transport, and conclusion/witness preservation when a machine-checked result is reused across mathematical-physics formalisms.
- **DEC-064:** Describe Comparator as a record-level audit-to-production interface. Its challenge reproduces the OSreconstruction package's own audit definitions; it is not a bridge between independently authored physical formalisms, a second derivation, or independent validation of the shared specification.
- **DEC-065:** Distinguish the Comparator's positive record-level result from the cross-project OSforGFF-to-OSreconstruction instantiation boundary. Do not treat them as symmetric cases.
- **DEC-066 (2026-11-27):** The DeDeo & Duede comparison, Comparator scope, Douglas citation disambiguation, public-package terminology, and BibTeX cleanup are completed. No OS mathematics or numerical calculations are changed.
- **DEC-067 (2026-11-27):** Following the bounded originality/interface revision, the integrated manuscript contains 206 abstract words, six keywords, 7,061 main-text words excluding abstract and references, and 23 cited references. The root BibTeX file contains the same 23 cited works.
