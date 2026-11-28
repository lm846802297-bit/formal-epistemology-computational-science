# Stage 3 Acceptance: Public Recognition, Downstream Use, and Attribution

**Snapshot:** 2026-11-28  
**Branch:** research/stage3-recognition-reuse  
**Status:** completed as a source-pinned comparative documentary study. No manuscript text changed.

## 1. Research question and acceptance criteria

This stage asks what happens to a formally verified mathematical result after its initial release. The four cases are compared along six dimensions: public and institutional recognition; independent technical checking; human mathematical interpretation; citation and direct technical reuse; correction or extension; and attribution of intellectual, formal, infrastructural, and interpretive labour.

A repository import, a paper citation, a theorem dependency, a human-readable reconstruction, and a public headline are different events. A claim of downstream mathematical use requires an identifiable later mathematical artifact that cites, imports, adapts, or explicitly depends on the target result or its proof. A project that cites another project only as an organizational precedent is methodological influence, not mathematical reuse.

## 2. Riemann hypothesis

The Lean FRO/Mathlib joint statement of 21 November 2026 recognizes the formal statement and proof after statement review, independent comparison, full compilation, and kernel-based checking. This is strong institutional and technical recognition within the Lean ecosystem, not evidence of unanimous acceptance by all number theorists.

The community repository leanprover-community/riemann-hypothesis describes itself as a community-led effort to clean up and maintain the RH/GRH formalization. Its aims include accessibility, readability, improved build performance, bibliographic integration, and reliance on existing formalization projects. Its README records the move to a condensed version on 25 November and preserves earlier work on separate branches. The generated contributor file records a large maintenance network. These are observable forms of institutional uptake and governance, not a measure of the number of mathematicians who independently accept the informal argument.

The G.R.H. Polymath initiative, announced on 24 November, coordinates mathematicians to translate the Lean proof into a human-readable argument, examine the mathematical literature, and investigate generalizations. Jimmie Adriazola's public reconstruction repository contains a 297-page reconstruction of the original archive, a 117-page working manuscript, and a 59-page classical-RH specialization. The repository explicitly labels the manuscripts incomplete and conditional, identifies unresolved arithmetic inputs, and asks specialists to review them.

These projects establish sustained mathematical engagement and attempts at interpretation. They do not establish that a complete, independent classical proof has already been produced in conventional mathematical form.

The strongest observed downstream effects are maintenance and refactoring of the formal artifact; construction of human-readable expositions and proof maps; and coordinated investigation of mathematical dependencies and generalizations. No independently published later theorem or research paper was identified in this snapshot that uses the newly claimed RH result as a premise for a subsequent mathematical result. This is a time-bounded negative finding.

Attribution distinguishes the original proof strategy, credited to Levent Alpöge with Claude credited for a key proof-strategy proposal, from later exposition, refactoring, review, infrastructure maintenance, and independent checking. The reconstruction repository explicitly preserves Alpöge's priority while identifying reconstruction as a separate interpretive contribution.

**Finding:** Riemann has the strongest public and institutional recognition of the four cases, accompanied by an unusually visible programme of mathematical reconstruction. Recognition and interpretive uptake are better evidenced than downstream theorem reuse.

## 3. Navier–Stokes

Bastounis, Circelli, and Hansen's 2026 paper, Navier–Stokes Lost in Translation, identifies mismatches between the published mathematical exposition and the Lean development, including a derivative-order discrepancy in Lemma 8.6 and issues in the pressure-flux estimate. These are representational-fidelity criticisms: they concern whether the checked formal declarations match the paper's mathematical claims, not whether Lean's kernel accepts an invalid derivation.

The public OpenAI repository's original September 8 commit and later September 9 commit are pinned in the source record. The later commit adds substantial modules and modifies comparator theorem adapters. The repository has no public PR or issue discussion in the inspected snapshot, so repository history alone does not document a public response to the independent criticism.

The SafeVerifyAgent audit of the September 8 artifact reports no load-bearing weakening in its four paper/Lean slices, but distinguishes source reading from compilation and notes incomplete line-by-line coverage of the full dependency cone. Its auditor family is not model-independent. This is evidence of a structured review effort, not a final specialist consensus.

The clearest direct technical reuse is the public Vilin97/ns-formalization-benchmark project. It extracts the complete transitive dependency closures for the two final Navier–Stokes breakdown targets from OpenAI's original source and LeanPool's pooled version, pins upstream commits and source SHA-256 hashes, and builds both under the same Lean 4.34.0-rc2 compiler and Mathlib revision.

Recorded single clean builds:
- OpenAI original: 580 modules, 18m 4.27s, 13.273 GiB peak aggregate compiler RSS.
- LeanPool: 422 modules, 11m 11.04s, 6.451 GiB peak aggregate compiler RSS.

The benchmark reports 1.62x speedup and 51.4% lower peak aggregate compiler RSS for LeanPool. It preserves machine metadata, exact compiler commands, per-module logs, RSS samples, and source hashes. Both theorem pairs were separately checked for axioms, with only the standard propext, Classical.choice, and Quot.sound dependencies and no sorryAx. The benchmark cautions that this checks axiom dependencies, not semantic equivalence to the informal statement.

The project competemath/tengoku registers and redistributes LeanPool, including the OpenAI Navier–Stokes project, with per-source attribution and licensing records. KTS Global's public package describes itself as a port/rebuild of OpenAI's formalization, but explicitly states that it is not a Clay-recognized result and that independent specialist review of statement correspondence has not occurred. It is a derivative verification/packaging effort, not independent mathematical confirmation.

**Finding:** Navier–Stokes has the clearest evidence of direct technical reuse and reproducibility infrastructure. It also has the clearest documented dispute over correspondence between the informal paper and formal artifact. Code reuse must not be equated with acceptance of the Clay-level mathematical claim.

## 4. AlphaProof Nexus

### The nine Erdős outputs and their scope

The Science paper reports that the full-featured AlphaProof Nexus agent solved 9 of 353 formalized Erdős problems attempted. It says that after each solve, experts on the team checked that the Lean statement faithfully captured the original conjecture. The nine public archive files at pinned commit 42f344cfa9d57154f36e6b9bef1f71760a438c54 are:

| Output file | Recorded problem | Scope note |
|---|---|---|
| erdos_12.parts.i.lean | #12(i) | Part of #12 |
| erdos_12.parts.ii.lean | #12(ii) | Separate part of #12 |
| erdos_125.variants.positive_lower_density.lean | #125, positive-lower-density variant | Variant file; density interpretation is material |
| erdos_138.variants.difference.lean | #138, difference variant | Variant file |
| erdos_152.lean | #152 | Main numbered statement |
| erdos_26.variants.tenenbaum.lean | #26, Tenenbaum variant | Paper says this more general variant was not itself posed by Erdős |
| erdos_741.parts.i.lean | #741(i) | Part of #741 |
| erdos_741.parts.ii.lean | #741(ii) | Separate part of #741 |
| erdos_846.lean | #846 | Main numbered statement |

Thus the nine outputs are not nine unqualified, distinct original Erdős conjectures. They include separate parts and explicitly marked variants. The paper explicitly says #26 is a more general variant of a question posed by Erdős, not a problem posed by Erdős himself.

The nine files were inspected individually at the pinned archive commit. All nine contain neither sorry nor an explicit axiom token. This is source-level inspection; the paper and project validation pipeline supply the broader compilation and validation claims.

### Statement correction and human intervention

The Science paper records a substantive correction discovered during proof search: the informal word density in #125 and #741(i) was clarified as lower density and upper density respectively. The agent found proofs under a natural-density interpretation; the target was amended and the agent still solved the corrected statements. This shows that formal proof search did not merely validate a fixed target: it exposed ambiguity in the mathematical statement, while the project team adjudicated the intended formulation.

The paper also reports failure modes in which candidate sketches hid the target in a sorry helper or relied on hallucinated literature lemmas. Its final validation pipeline checks complete, sorry-free proofs and disallowed axioms before registration. Incomplete sketches and accepted proof artifacts are therefore distinct.

### Downstream mathematical use and extension

The strongest concrete downstream-use evidence is the quantum-optics deployment reported in the same Science article. With Mario Krenn, the team investigated monochromatic quantum graphs. The public AlphaProof Nexus archive contains a formalization of the quantum-graph problem and a separate 2,196-line formalization of Open Quantum Problem 35, concerning absolutely maximally entangled states. The latter includes reusable lemmas on reduced density matrices and explicit Bell/GHZ examples. The paper describes quantum-optics research as an application of the system in an active research collaboration.

A particularly strong subsequent mathematical artifact is the all-orders Krenn–Gu proof in rrajasek95/krenn-conjecture. Its Lean Solution proves the theorem for all even N >= 6 and all D >= 3, using definitions copied from the Formal Conjectures statement repository. The external proof is registered in Palomar and referenced by Formal Conjectures PR #6627. PR #6627 remains open in this snapshot and explicitly records that the in-file theorem body remains sorry while the external proof is linked through a formal_proof attribute. The proof exists as a separate checked artifact; the upstream PR has not yet been merged.

The quantum-graph source contains other declarations and research-solved labels whose bodies remain sorry. Those labels alone are not proof artifacts. The separately pinned external solution is the relevant complete proof evidence.

The Science paper also says an optimization result was subsequently extended by later work. This is a downstream-use claim in the paper, but the exact extension should be source-checked before it is used as a central example in the manuscript.

### Attribution

The paper's author-contribution statement distinguishes problem selection and validation, Lean formalization, natural-language proof writing, agent design, systematic evaluation, repository coordination, and strategic direction. It credits George Tsoukalas with initiating and leading the system's use in mathematics research; other contributors validated solutions, wrote informal proofs, formalized problems, built the repository, and integrated Lean with AlphaProof. The first three authors are stated to be in random order. The paper does not attribute the entire mathematical result to a single autonomous system.

**Finding:** AlphaProof Nexus offers the richest example of distributed and explicitly documented authorship. The nine Erdős outputs are heterogeneous in scope. The strongest downstream-use evidence is the transition into quantum-optics research and a separate all-orders mathematical proof, rather than a simple citation count.

## 5. Liquid Tensor Experiment

The original leanprover-community/lean-liquid README defines LTE as digitising mathematical definitions, theorem statements, and proofs from Scholze's Bonn lecture notes. It distinguishes two targets: the technically demanding Analytic 9.4 (with related 9.5), represented by first_target; and Scholze's public challenge, Theorem 1.1, represented by liquid_tensor_experiment.

The README records the first part's preliminary completion announcement on 28 May 2021 and the second part's completion on 14 July 2022. The formal target liquid_tensor_experiment states the vanishing of Ext^i(M_{p'}S,V) for i > 0, for a profinite set S and a p-Banach space V under the stated exponent conditions. The project used Lean 3.48.0 and a pinned Mathlib revision.

The LTE Blueprint was not merely a progress dashboard. The repository describes it as a guide comprehensible to mathematicians without Lean training, a visual representation of proof dependencies, and a cross-referenced route between mathematical statements and Lean declarations. It coordinated the two subprojects: proving the technical intermediate theorem and proving that it implies the public challenge theorem.

### Later mathematical use: three distinct levels

1. **Mathematical-library continuity:** Mathlib's Mathlib/Condensed/Basic.lean defines condensed objects as sheaves on compact Hausdorff spaces and cites Clausen–Scholze and Barwick–Haine. Its provenance is not an import of the LTE repository, and it does not import LTE's first_target or liquid_tensor_experiment theorem.
2. **Later technical development in the same area:** Meta's ATLAS Lean repository imports Mathlib.Condensed.TopComparison in its condensed topological-rings development. This is direct use of Mathlib's condensed-mathematics infrastructure, not evidence that the LTE proof theorem itself is imported or used.
3. **Methodological influence:** Becker et al.'s 2026 paper on the Lean formalization of Carleson's theorem cites LTE as a precedent for large collaborative formalization and discusses mathematical blueprints as a common coordination device. This establishes methodological and organizational influence, not reuse of LTE's condensed-mathematics theorem.

No later research paper or formal project was identified in this snapshot that directly imports or cites the LTE theorem as a mathematical premise in a new result. The record supports durable influence on formalization practice and the condensed-mathematics library ecosystem, while direct theorem-level reuse remains unestablished.

**Finding:** LTE's clearest afterlife is methodological and infrastructural: a reusable blueprint model, a formalized condensed-mathematics vocabulary, and a visible precedent for collaborative theorem formalization. Direct reuse of the central LTE theorem in later mathematical results is not demonstrated by the current source corpus.

## 6. Unified four-case comparison

| Dimension | Riemann | Navier–Stokes | AlphaProof Nexus | LTE |
|---|---|---|---|---|
| Recognition pattern | Institutional certification and number-theory engagement | Public release, technical scrutiny, derivative packaging | Research benchmark and publication, human target validation | Community completion and specialist recognition |
| Independent checking | Multiple Lean/kernel/comparator checks and external replay | Independent criticism, audits, reproducible derivative builds | Lean/SafeVerify validation plus expert target review | Community proof development and formal completion |
| Human interpretation | Polymath and readable reconstructions | Paper-to-Lean audits and technical dissections | Natural-language proof accounts and domain collaborators | Blueprint and explanatory project documentation |
| Direct downstream theorem reuse | Not yet evidenced in this snapshot | Strong: dependency-closure reuse, LeanPool, Tengoku, reproducible benchmark | Strong in quantum optics and separate Krenn–Gu all-orders proof | Not yet evidenced for the central LTE theorem |
| Methodological/infrastructural reuse | Proof maps, refactoring, governance, replay practices | Packaging, benchmark, audit, repository aggregation | Proof-search workflow, validation pipeline, quantum-optics deployment | Blueprint as shared proof/coordination artifact; Mathlib condensed infrastructure |
| Correction/qualification | Reconstruction still identifies open steps | Concrete paper/Lean correspondence criticisms | Density reinterpretation in #125 and #741(i); variants distinguished | Two-stage proof architecture and explicit target documentation |
| Attribution pattern | Original strategy separated from exposition, maintenance, checking | Original proof separated from audit, packaging, benchmarking | Distributed and itemized contribution roles | Community formalization of source mathematics, library, coordination labour |

## 7. Empirical synthesis

The cases do not support a single linear path from formal verification to universal mathematical authority. They exhibit at least three different afterlives:

- **Recognition and reconstruction:** Riemann shows how a formal proof can trigger institutional certification and a large programme of human mathematical interpretation before theorem-level reuse is visible.
- **Artifact reuse under contested correspondence:** Navier–Stokes shows that a proof artifact can be copied, rebuilt, benchmarked, and incorporated into other repositories while the relationship between the formal statement and the published mathematical claim remains contested.
- **Distributed research production and infrastructure:** AlphaProof Nexus and LTE show two distinct forms of collective production. AlphaProof Nexus makes the agent, human validation, formalization, exposition, and domain collaboration visible in an authorial contribution structure. LTE makes the mathematical blueprint and community coordination central to the formalization process.

The central empirical distinction is that technical reuse, mathematical reliance, institutional recognition, and public symbolic authority are separate outcomes. A repository can be reused without the theorem being used as a premise; a theorem can be institutionally recognized without yet becoming a tool for later results; a blueprint can influence research practice without its target theorem being imported elsewhere.

The empirical question to carry into final theoretical selection is:

> How do distinct forms of verification, recognition, interpretation, reuse, and attribution convert a bounded formal artifact into different kinds of epistemic authority?

This result does not yet authorize a manuscript rewrite.

## 8. Source pins and primary links

- Riemann community repository: https://github.com/leanprover-community/riemann-hypothesis
- Riemann reconstruction: https://github.com/jimjamzola/RH-Alpoge-Reconstruction
- G.R.H. Polymath announcement: https://terrytao.wordpress.com/2026/11/24/riemann-hypothesis-polymath-project/
- Navier–Stokes original repository: https://github.com/openai/NavierStokesAndEuler
- Navier–Stokes reproducible comparison: https://github.com/Vilin97/ns-formalization-benchmark
- Navier–Stokes pooled reuse: https://github.com/competemath/tengoku
- Navier–Stokes audit: https://github.com/GasStationManager/SafeVerifyAgent
- AlphaProof Nexus paper: https://doi.org/10.1126/science.aej2213
- AlphaProof Nexus output archive, pinned commit: https://github.com/google-deepmind/alphaproof-nexus-results/tree/42f344cfa9d57154f36e6b9bef1f71760a438c54
- Krenn–Gu downstream proof: https://github.com/rrajasek95/krenn-conjecture/tree/56f495ae11cf4729e6173477cb25afff7342c8cf
- Formal Conjectures PR #6627: https://github.com/google-deepmind/formal-conjectures/pull/6627
- LTE repository: https://github.com/leanprover-community/lean-liquid
- Mathlib condensed definitions: https://github.com/leanprover-community/mathlib4/blob/master/Mathlib/Condensed/Basic.lean
- ATLAS condensed development: https://github.com/facebookresearch/atlas-lean
- Carleson formalization paper: https://arxiv.org/abs/2609.31334

## 9. Stage 3 acceptance decision

**Accepted.** The predeclared six dimensions have been examined for all four cases; primary artifacts and repository records have been pinned; direct mathematical reuse has been separated from methodological influence; and the comparison yields a stable empirical synthesis.

No further case expansion is required for this stage. Additional source collection is a targeted follow-up only if a concrete claim in the final theoretical analysis depends on it. Manuscript revision remains a separate next stage.
