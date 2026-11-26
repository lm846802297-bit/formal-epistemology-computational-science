# Final Reference and Source Audit (revised manuscript)

**Audit date:** 2026-11-26  
**Scope:** The 20 works cited in the revised integrated manuscript. Metadata and source locations were checked against publisher, repository, and preprint records. This does not replace the submitting author's substantive reading and verification.

| Reference | Verification source | Result |
|---|---|---|
| Bobbin et al. (2024), *Formalizing Chemical Physics Using the Lean Theorem Prover* | RSC DOI 10.1039/D3DD00077J | Authors, title, Digital Discovery 3(2), pages 264–280, DOI matched |
| Cherkis et al. (2026), OSforGFF | Pinned repository formalization.yaml and commit fef84a82937dfd2bb7f672108a72da329d3ef0fd | Five listed authors include Sergey A. Cherkis; exact commit and project metadata matched |
| Contessa (2007), *Scientific Representation, Interpretation, and Surrogative Reasoning* | DOI 10.1086/519478 | Title, author, Philosophy of Science 74(1), pages 48–68 matched |
| DeDeo & Duede (2026), *A Correspondence Problem for Mathematical Proof* | arXiv:2603.13680v2; PhilArchive | Title and authors matched; Philosophy of Science status listed as forthcoming in records inspected |
| Douglas et al. (2026), *Formalization of QFT* | arXiv:2603.15770v1 | Authors, title, arXiv identifier and preprint status matched |
| Douglas, Yin, & Mei (2026), OSreconstruction-comparator | Pinned repository and formalization.yaml, commit 93cdb40e728ba27b7b1b55efc30d57f7b43de9aa | Authors, project identity, exact commit matched |
| Frigg & Nguyen (2018), *The Turn of the Valve* | Springer DOI 10.1007/s13194-017-0182-4 | Title, authors, European Journal for Philosophy of Science 8(2), pages 205–224 matched |
| Gelfert (2009), *Rigorous Results, Cross-Model Justification...* | DOI 10.1007/s11229-008-9431-6 | Title, author, Synthese 169(3), pages 497–519 matched |
| Gelfert (2011), *Mathematical Formalisms in Scientific Practice* | DOI 10.1016/j.shpsa.2010.11.035 | Title, author, Studies in History and Philosophy of Science Part A 42(2), pages 272–286 matched |
| Gelfert (2022), *Thinking with Notations* | Springer DOI 10.1007/978-3-030-97833-4_11 | Title, author, book and page metadata matched |
| Glimm & Jaffe (1987), *Quantum Physics* | Springer DOI 10.1007/978-1-4612-4728-9 | Second edition, authors, publisher, year, DOI matched |
| Hughes (1997), *Models and Representation* | DOI 10.1086/392611 | Title, author, Philosophy of Science 64, pages S325–S336 matched |
| Imbert & Ardourel (2023), *Formal Verification, Scientific Code...* | DOI 10.1017/psa.2022.78 | Title, authors, Philosophy of Science 90(2), pages 376–394 matched |
| Knuuttila (2021), *Epistemic Artifacts and the Modal Dimension of Modeling* | DOI 10.1007/s13194-021-00374-5 | Title, author, European Journal for Philosophy of Science 11, article 65 matched |
| Meadows et al. (2026), *FormalScience* | ACL Anthology DOI 10.18653/v1/2026.acl-long.1057 | Title, authors, proceedings and pages 23059–23077 matched |
| Osterwalder & Schrader (1973), *Axioms for Euclidean Green's Functions* | Project Euclid / Springer DOI 10.1007/BF01645738 | Title, authors, Communications in Mathematical Physics 31(2), pages 83–112 matched |
| Osterwalder & Schrader (1975), *Axioms for Euclidean Green's Functions II* | Project Euclid DOI 10.1007/BF01608978 | Title, authors, Communications in Mathematical Physics 42(3), pages 281–305 matched |
| Parker (2020), *Model Evaluation: An Adequacy-for-Purpose View* | DOI 10.1086/708691 | Title, author, Philosophy of Science 87(3), pages 457–477 matched |
| Suárez (2004), *An Inferential Conception of Scientific Representation* | DOI 10.1086/421415 | Title, author, Philosophy of Science 71(5), pages 767–779 matched |
| Yin et al. (2026), OSreconstruction in Lean | Pinned repository commit cf0904e34a7c146a9f312f601e3707dca4a87697 | Authors, package path, exact commit and project identity matched |

## Source-critical corrections

- OSforGFF's software authorship is taken from the pinned formalization.yaml: Sergey A. Cherkis, Michael R. Douglas, Sarah Hoback, Anna Mei, and Ron Nissim. This differs from the author list of the related Douglas et al. QFT preprint.
- The Comparator challenge is described as reproducing the OSreconstruction package's own Mathlib-only audit definitions, not as an independently authored mathematical specification.
- The private companion's reported massive-free-field and Proca-Wick-square inhabitants are attributed to the OSreconstruction README; the private code was not independently inspected.
- The two OSreconstruction growth records are distinguished: the arity-linear condition and the original-coordinate OS-II E0-prime condition are connected by a proved conversion.
- The OSforGFF OS1 predicate is described as the Glimm–Jaffe generating-functional bound with the subsidiary two-point condition, not as the OSreconstruction arity-dependent growth hypothesis.

## Remaining author verification

The submitting author must read the cited works and confirm that each source supports the precise interpretation attributed to it. Metadata verification alone does not establish that a paraphrase is faithful. Repository claims should be checked against the pinned commits before submission.
