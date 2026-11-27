# Final Reference and Source Audit (major revision)

**Audit date:** 2026-11-27  
**Scope:** The 23 works cited in the current integrated manuscript and retained in the root BibTeX file. Metadata and source locations were checked against publisher, repository, and preprint records. This does not replace the submitting author's substantive reading and verification.

| Reference | Verification source | Result |
|---|---|---|
| Al Wardani et al. (2023), *Formal Reasoning Using Distributed Assertions* | Springer DOI 10.1007/978-3-031-43369-6_10 | Authors, FroCoS 2023, LNCS 14279, pages 176–194, DOI matched |
| Bobbin et al. (2024), *Formalizing Chemical Physics Using the Lean Theorem Prover* | RSC DOI 10.1039/D3DD00077J | Authors, title, Digital Discovery 3(2), pages 264–280, DOI matched |
| Cherkis et al. (2026), OSforGFF | Pinned repository formalization.yaml and commit fef84a82937dfd2bb7f672108a72da329d3ef0fd | Five listed authors include Sergey A. Cherkis; exact commit and project metadata matched |
| Contessa (2007), *Scientific Representation, Interpretation, and Surrogative Reasoning* | DOI 10.1086/519478 | Title, author, Philosophy of Science 74(1), pages 48–68 matched |
| DeDeo & Duede (2026), *A Correspondence Problem for Mathematical Proof* | arXiv:2603.13680v2; PhilArchive full text | Title, authors, and forthcoming status matched; Sections 3–4 substantively reviewed for library lock-in, shared models, and structural/causal/explanatory routes to correspondence |
| Douglas et al. (2026), *Formalization of QFT* | arXiv:2603.15770v1 | Authors, title, arXiv identifier and preprint status matched |
| Douglas, Yin, & Mei (2026), OSreconstruction-comparator | Pinned repository and formalization.yaml, commit 93cdb40e728ba27b7b1b55efc30d57f7b43de9aa | Authors, project identity, exact commit matched |
| Frigg & Nguyen (2018), *The Turn of the Valve* | Springer DOI 10.1007/s13194-017-0182-4 | Title, authors, European Journal for Philosophy of Science 8(2), pages 205–224 matched |
| Gelfert (2009), *Rigorous Results, Cross-Model Justification...* | DOI 10.1007/s11229-008-9431-6 | Title, author, Synthese 169(3), pages 497–519 matched |
| Gelfert (2011), *Mathematical Formalisms in Scientific Practice* | DOI 10.1016/j.shpsa.2010.11.035 | Title, author, Studies in History and Philosophy of Science Part A 42(2), pages 272–286 matched |
| Gelfert (2022), *Thinking with Notations* | Springer DOI 10.1007/978-3-030-97833-4_11 | Title, author, book and page metadata matched |
| Glimm & Jaffe (1987), *Quantum Physics* | Springer DOI 10.1007/978-1-4612-4728-9 | Second edition, authors, publisher, year, DOI matched |
| Guilloud et al. (2025), *Interoperability of Proof Systems with SC-TPTP* | Springer DOI 10.1007/978-3-031-99984-0_18; Springer author metadata | Seven authors, CADE 30, LNCS 15943, pages 325–340, DOI matched |
| Hughes (1997), *Models and Representation* | DOI 10.1086/392611 | Title, author, Philosophy of Science 64, pages S325–S336 matched |
| Imbert & Ardourel (2023), *Formal Verification, Scientific Code...* | DOI 10.1017/psa.2022.78 | Title, authors, Philosophy of Science 90(2), pages 376–394 matched |
| Knuuttila (2021), *Epistemic Artifacts and the Modal Dimension of Modeling* | DOI 10.1007/s13194-021-00374-5 | Title, author, European Journal for Philosophy of Science 11, article 65 matched |
| Meadows et al. (2026), *FormalScience* | ACL Anthology DOI 10.18653/v1/2026.acl-long.1057 | Title, authors, proceedings and pages 23059–23077 matched |
| Osterwalder & Schrader (1973), *Axioms for Euclidean Green's Functions* | Project Euclid / Springer DOI 10.1007/BF01645738 | Title, authors, Communications in Mathematical Physics 31(2), pages 83–112 matched |
| Osterwalder & Schrader (1975), *Axioms for Euclidean Green's Functions II* | Project Euclid DOI 10.1007/BF01608978 | Title, authors, Communications in Mathematical Physics 42(3), pages 281–305 matched |
| Parker (2020), *Model Evaluation: An Adequacy-for-Purpose View* | DOI 10.1086/708691 | Title, author, Philosophy of Science 87(3), pages 457–477 matched |
| Rabe (2017), *Morphism Axioms* | DOI 10.1016/j.tcs.2017.07.006 | Author, title, Theoretical Computer Science 691, pages 55–80, DOI matched |
| Suárez (2004), *An Inferential Conception of Scientific Representation* | DOI 10.1086/421415 | Title, author, Philosophy of Science 71(5), pages 767–779 matched |
| Yin et al. (2026), OSreconstruction in Lean | Pinned repository commit cf0904e34a7c146a9f312f601e3707dca4a87697 | Authors, package path, exact commit and project identity matched |

## Source-critical corrections

- OSforGFF software authorship is taken from the pinned formalization.yaml: Sergey A. Cherkis, Michael R. Douglas, Sarah Hoback, Anna Mei, and Ron Nissim. This differs from the author list of the related Douglas et al. QFT preprint.
- The Comparator challenge reproduces the OSreconstruction package's own Mathlib-only audit definitions; its independence is at the import/checking boundary, not authorship or mathematical origin.
- The Comparator bridge files establish record conversions, preserve the Schwinger family, transfer growth records, and identify Wick-pairing/output-growth predicates.
- The private companion's reported massive-free-field and Proca-Wick-square inhabitants are attributed to the OSreconstruction README; the private code was not independently inspected.
- The two OSreconstruction growth records are distinguished: the arity-linear condition and the original-coordinate OS-II E0-prime condition are connected by a proved conversion.
- The OSforGFF OS1 predicate is described as the Glimm–Jaffe generating-functional bound with the subsidiary two-point condition, not as the OSreconstruction arity-dependent growth hypothesis.
- Rabe's theory morphisms, DAMF, and SC-TPTP are treated as prior formal mechanisms for proof-preserving translation, assertion transfer, and proof-system interoperability. The manuscript does not claim these mechanisms as new.
- DeDeo and Duede (2026) already analyze library lock-in, shared-model hybridization across modelling traditions, and structural, causal, and explanatory routes to correspondence. The manuscript therefore makes no novelty claim for library dependence or correspondence in general; it narrows its contribution to the interface conditions for transferring results between source and receiving formal records in mathematical physics.

## Remaining author verification

The submitting author must read the cited works and confirm that each source supports the precise interpretation attributed to it. Metadata verification alone does not establish that a paraphrase is faithful. Repository claims should be checked against the pinned commits before submission.


## Substantive claim audit integrated (2026-11-27)

The source-critical audit is preserved on branch `audit/submission-source-check-2026-11-27`, commit `b5c4ce03b1157e2af018ff857cf7b166ec1b3ee7`. Its HTML report and CSV evidence table contain 50 claim records covering the 23 cited works. The audit was prepared against manuscript commit `61d565a204b3ff0f76e0c9522651263617abb2a0` (integrated manuscript blob `f080288c9196e9aefe7ee3d6b6d53074f430d11b`). The current PR branch was eight commits ahead at `9ccaece3bfbe0fb76db1a27a14cb614d18a1251c`; the current integrated manuscript blob before this integration was `467e1b0cce41fa0c0a99f0d33b2f2de99641def2`. The audit was mapped to current text rather than applied by stale line number.

Audit artifact Git blob IDs: HTML `4edf3d756b940f017fd844e4231bbd6599252329`; CSV `363e9e332c1a132536d1da9fcbd714bc5aad545f`.

The source pins are OSforGFF `fef84a82937dfd2bb7f672108a72da329d3ef0fd`, OSreconstruction `cf0904e34a7c146a9f312f601e3707dca4a87697`, and Comparator `93cdb40e728ba27b7b1b55efc30d57f7b43de9aa`. Integrated corrections cover Rabe's judgment-preservation terminology and model-reduct direction; DAMF/SC-TPTP scope; E0′ limited to the Section IV forward theorem; the QFT paper's four-dimensional scope versus the OSforGFF all-(D\geq2) corollary; Glimm–Jaffe p. 91 n. 1; Douglas et al. Remark 3.2 attribution for the L1(μ) ergodicity extension; Comparator's 460-line mathematical declaration block, three theorem targets and historical CI; and corrected attributions for Gelfert, Hughes, Suárez, Contessa, and Frigg–Nguyen.

No Lean kernel was rerun. Comparator statements were checked by source comparison, and historical CI logs were inspected. No new Lean build or proof replay is claimed.

**Author verification still required:** the continuation of Glimm and Jaffe (1987), second edition, §6.1(i), containing the full OS4 quantifiers, norm, and time-average statement was not available in the public preview. The author should inspect those pages directly. All 23 source entries remain subject to final author reading and approval.


## Editorial presentation of software sources

The manuscript cites OSforGFF, OSreconstruction, and the Comparator by project name and repository URL, without placing commit hashes or source-integrity checks in the article's prose or reference entries. Exact revisions, file-level comparisons, and proof-checking records remain preserved in the source-audit documentation for reproducibility. This keeps the philosophical article focused on its mathematical and epistemological claims while retaining technical provenance outside the manuscript.
