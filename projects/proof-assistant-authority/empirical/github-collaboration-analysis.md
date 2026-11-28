# GitHub Collaboration Archives and Contribution-Network Analysis

**Snapshot:** 2026-11-28  
**Research phase:** Empirical Research, Stage 1  
**Method:** public repository census plus purposive event-level analysis  
**Status:** first documentary pass complete; full reception and reuse study remains open.

## 1. Scope and method

This report examines public GitHub traces for four cases. The unit of observation is a repository event: commit, pull request, review, issue, merge, status change, provenance correction, or independent replay record.

The collection distinguishes:
- **repository census:** counts and visible repository structure at the snapshot date;
- **purposive event sample:** records selected because they concern theorem production, formal statement, semantic checking, infrastructure, attribution, or public status;
- **network inference:** observed author–reviewer–maintainer relations in the sampled records.

The sample is not a random sample of mathematicians, and GitHub is not the whole research process. Private Zulip, email, seminars, institutional meetings, and unrecorded labour are outside this dataset.

## 2. Repository-level comparison

| Case | Public repositories inspected | GitHub record at snapshot | Initial structural reading |
|---|---|---|---|
| Riemann | `leanprover-community/riemann-hypothesis` | 192 accounts in generated contributor file; 6,079 summed merged-PR counts; active PR and issue archive | Community-led maintenance, refactoring, CI/cache governance, provenance work and independent audits |
| Navier–Stokes | `openai/NavierStokesAndEuler` | 2 commits, both by `balexeev-oai`; 0 PRs; 0 issues | Publication-oriented technical snapshot, with external scrutiny occurring outside the repository |
| AlphaProof Nexus | `google-deepmind/alphaproof-nexus-results`, `google-deepmind/formal-conjectures`, `teorth/erdosproblems` | Results archive: 6 commits, 5 by `aferr`, 1 by `eric-wieser`; 0 PRs; 4 issues. Substantive human review appears in Formal Conjectures PRs. | Small output archive connected to a much larger human-maintained statement, review and status infrastructure |
| Liquid Tensor | `leanprover-community/lean-liquid` | 57 PRs, 49 merged, 6 closed unmerged, 2 open; 76 issues; 15 PR authors in the census | Small, concentrated mathematical collaboration with visible semantic examples, documentation negotiation and infrastructure work |

These numbers are not directly comparable measures of labour. The repositories have different purposes: a publication archive, a large maintained proof development, a community library project, and a formal-conjecture integration repository.

## 3. Riemann Hypothesis: community maintenance, gatekeeping and provenance

### 3.1 Repository purpose and history

The repository README describes the project as a community-led effort to clean up and maintain a Lean formalization of the 2026 RH/GRH proofs. It explicitly separates three archival/workflow layers:
- `main`: a condensed, readable working version;
- `alpoge`: earlier community cleanup history;
- `original`: the first public version retrieved on 20 November 2026.

The README states the goals as accessibility, readability, and integration with the mathematical community. It also specifies that the repository is not seeking unrelated additions or unsupported claims about individual builds.

The README blob at this snapshot is `6a98a3faa41f6c59cf0fb4b8e4d4b4ca7c45c1d1`. The generated `CONTRIBUTORS.md` blob is `f8e211a17347be739b2b89ab582ca4bbb0f97cdf`.

### 3.2 Contribution concentration

The generated contributor file lists 192 GitHub accounts and, when the per-account merged-PR counts are summed, 6,079 merged PRs. Its header explicitly says that PRs from the earlier `alpoge` edition are included.

- Top 2 accounts: 2,047 merged PRs (33.7% of the listed total).
- Top 5 accounts: 3,148 (51.8%).
- Top 10 accounts: 3,799 (62.5%).

This is a repository-maintenance activity measure, not a count of RH theorem authors, independent mathematical contributions, or unique human researchers. PR batching and historical branch inclusion affect the count. The top-account snapshot is preserved in `riemann-contributors-top.csv`.

### 3.3 Selected workflow and governance events

- **PR #1 (20 Feb 2026 in the project record):** configures Mathlib cache retrieval. The author tested a clean clone and reported 8,690 cache files downloaded.
- **PR #7:** adds a public Cloudflare/Lake cache and verified archive bootstrap. This is infrastructure for reproducible builds and external access.
- **PR #8:** simplifies Main imports and removes six modules considered unreachable. The change triggered a provenance discussion because the README and mirror check still described the source as unmodified.
- **PR #12:** an external contributor proposed additional RH reductions from a collaborative Principia project. It was closed without merge. The repository's stated scope distinguishes maintenance of the published proof from accepting new mathematical results.
- **PR #44:** proposed a large simplification of the shared five-theorem proof and a 1.54-million-line source reduction; it was closed without merge.
- **PR #54:** a 180-commit, 129-file batch proposed 3,220 net Lean lines of proof refactoring; it was closed without merge when the upstream batch workflow had moved.
- **PR #64:** records source changes since the original submission and repairs the provenance/mirror check. It changes documentation and CI rather than Lean theorem content.
- **PR #101:** introduces a controlled donor-runner mode for bounded proof shards. Its policy pins source/configuration, affected-module lists, runner identity, leases, dependency manifests and workflow provenance.
- **PR #115:** lands a reviewed Lean 4.36 cleanup batch. Its description reports a full build of 149,396 modules and a 4.35 GB public cache, while preserving the attributed commits of the component PRs.
- **PR #9842:** a maintainer batch merges three already-approved PRs, one merge commit per PR, preserving authorship and rechecking approval labels immediately before merge.
- **PR #9845:** an open one-commit external refactor PR at the snapshot date; not yet a recognized/merged contribution.

### 3.4 Public disputes and semantic audit work

- **Issue #39:** an AI-assisted table initially listed 105 named statements and 83 not-yet-reviewed statements. The author later withdrew the proposal for a references file because source locations were missing. A small source-checked batch found that a Linnik statement initially called faithful was only a close match. Maintainer Deicyde later stated that many AI-added literature references were wrong and that citations should not be added until a checkable process exists. This is a concrete example of community review resisting unverified attribution.
- **Issue #47 and PR #64:** a provenance check became stale after source edits; the issue identified the mismatch and PR #64 documented the exact submission commit and declared source delta.
- **Issue #56:** participants debated whether to preserve Alpöge's original code unchanged in a sibling archive while continuing to refactor the working repository. Maintainer Deicyde agreed that exact preservation was valuable but defended a separate clean, performant importable version. A sibling `riemann-hypothesis-original` repository was subsequently created.
- **Issue #96:** a public structural audit alleged that trivial predicates appeared in the dependency chain. Other contributors supplied dependency analyses and counter-readings. This is evidence of contestation and audit work, not a settled proof that the theorem is invalid.
- **Issue #8738:** an independent Apple Silicon reproduction reports matching SHA-256 inputs and successful `con-ron` verification of all five headline theorems.
- **Issue #8747:** an independent check reports both editions building from source, three standard axioms, and several independent checkers accepting the formal claims. The author explicitly says that nobody read the mathematics; this is evidence for derivational verification, not a complete semantic audit.

### 3.5 Riemann case finding

The RH repository displays a large, stratified maintenance network: mathematical refactoring, cache and build infrastructure, review and batch governance, source provenance, literature attribution, and independent verification. Its public records also show that the community does not treat every proposed contribution as admissible. The distinction between preserving the original artifact and improving the working artifact is itself an object of negotiation.

## 4. Navier–Stokes: a publication snapshot with external scrutiny

The repository `openai/NavierStokesAndEuler` has two commits on `main` at the snapshot date:
- `8937a8f4cbc7abaab5e9e97d1cc7f5d2319d9538` (8 September 2026): root commit by `balexeev-oai`, 2,496 files and 616,833 added lines.
- `f9e8bc5b38b6e212696e8a30e3e91517af887bbd` (10 September 2026): subsequent update, also by `balexeev-oai`.

The repository has no public PRs or issues in the inspected record. Its `formalization.yaml` identifies the project authors as OpenAI. This is a centralized public release structure, not evidence that no internal collaboration occurred.

The principal independent critique is Bastounis, Circelli and Hansen, arXiv:2610.08144, which is outside the repository's GitHub review workflow. The critique concerns correspondence between the natural-language proof and the Lean formalization. It should be coded as an external assessment, not as a repository review or a final adjudication of the mathematical claim.

### Navier–Stokes case finding

The contrast is not simply “no collaboration.” It is that the public GitHub archive contains almost no visible internal review trace, while independent scrutiny appears in a separate scholarly channel. Therefore the repository itself cannot support a rich contribution-network reconstruction. Its public attribution and external adjudication must be studied through the paper, formalization metadata, commits, and external responses.

## 5. AlphaProof Nexus: output archive versus human review infrastructure

### 5.1 Results archive

The `alphaproof-nexus-results` repository has six commits in the inspected history:
- five authored/committed by `aferr`;
- one Lean CI commit by `eric-wieser`.

It has no PRs and four issues. This archive is therefore not the place where most public human review of the mathematical targets occurs.

The four issues reveal different provenance and scrutiny questions:
- **Issue #1:** asks where the natural-language proofs for the 44 OEIS results are; at the time, only one such proof was present in the repository.
- **Issue #2:** an external group proposes a machine-usable Lean frontier workbench; this is a proposal for future collaboration, not an accepted contribution.
- **Issue #3:** identifies eight `research solved` declarations in an AICollaborator QuantumOptics file that are `sorry` in this repository and link to proofs elsewhere. This issue concerns that QuantumOptics file, not the published Erdős proofs. It reveals a documentation/provenance ambiguity in what `lake build` checks.
- **Issue #4:** an external auditor reports replaying the published Erdős proof items and corrected #741(i) through Lean's kernel and nanoda; all ten pass. The same report separately notes discrepancies and prior results in the OEIS subset.

### 5.2 Formal Conjectures integration and review

The public recognition and integration network is visible in `google-deepmind/formal-conjectures`:

- **PR #3778:** authored by `mo271`; adds the upper-density variant of Erdős #741, records the DeepMind prover agent as having found a proof, changes the formal-conjecture status from research open to research solved, and is approved by `Paul-Lez` before merge on 24 April 2026.
- **PR #4384:** authored by `mo271`; upstreams AlphaProof Nexus OEIS results. It contains 53 commits, 3,709 additions, and 135 comments. Comment authors: `mo271` (89), `codrut3` (42), `eric-wieser` (2), `Paul-Lez` (1), and the welcome bot (1). Three APPROVED review events are recorded.
- During PR #4384, `codrut3` identified incomplete or inaccurate conjecture statements and one result that proved only the (m=8) case rather than the general statement. `mo271` accepted the correction and noted that the OEIS had already falsely reported the AlphaProof result as solving the general case.
- **PR #3737:** the reviewer asked for more precise attribution to AlphaProof; the author revised the docstring to say that the result was also proved by AlphaProof.
- **PR #3721:** the PR body attributes the construction to AlphaProof and Lean translation assistance to Claude. The reviewer requested preservation of docstrings and use of the formal-proof mechanism.
- **PR #3643 and #3604:** AlphaProof counterexamples exposed weaknesses or contradictions in earlier formalizations; human contributors changed the formal statements.
- **PR #2398:** describes an AlphaProof formal proof cleaned up for maintainability and labels the work as joint with `mo271`.

### 5.3 AlphaProof case finding

The public result archive is small and author-concentrated, but the integration network is not. Human maintainers and reviewers convert outputs into community statements, correct target mismatches, distinguish variants, assign attribution, and change public statuses. AlphaProof is therefore both a proof producer and, in some cases, a diagnostic instrument for discovering defects in existing formalizations.

The #4384 record is particularly important: it demonstrates that public status and solver attribution are mediated by sustained human review rather than being automatically conferred by the output archive.

## 6. Liquid Tensor Experiment: concentrated mathematical collaboration and public semantic work

### 6.1 PR census

The repository has 57 PRs in the retrieved census:
- 49 merged;
- 6 closed without merge;
- 2 open at the snapshot date;
- 15 distinct PR-author accounts.

The most active PR authors in this census are:
- `adamtopaz`: 14 PRs;
- `jcommelin`: 11;
- `bentoner`: 10;
- `riccardobrasca`: 6;
- `kim-em`, `robertylewis`, `faabian`, `vihdzp`, and `kbuzzard`: 2 each;
- six further accounts: one each.

The complete 57-row census is preserved in `liquid-tensor-pr-census.csv`. The issue search returned 76 issues; 49 are titled “Automatic upgrade has failed”, so these bot-generated maintenance tickets are excluded from the substantive mathematical discussion count.

### 6.2 Mathematical and semantic work

- **PR #95:** Adam Topaz begins the examples folder with a p-Banach example. Johan Commelin supplies extensive inline suggestions and comments, including discussion of non-canonical norms.
- **PR #96:** explicitly says that proving `Ext^*(-, X)` is a universal delta functor should help “convince ourselves that Ext is defined correctly”. This is direct evidence that the examples are intended as semantic checks, not merely code demonstrations.
- **PR #97:** proves effaceable delta functors are universal.
- **PR #104:** adds the computation (operatorname{Ext}^1(mathbb Z/nmathbb Z,mathbb Z/nmathbb Z)).
- **PR #105:** proves Ext universality.
- **PR #107:** iteratively improves the Ext example; comments discuss notation, categorical presentation and readability.
- **PR #113:** adds the Radon-measure example. The PR has 148 commits and comments from Commelin, Topaz and Adomani; the review discusses whether proof material belongs in the examples file or a prerequisite file.
- **PR #115:** adds the profinite example.
- **PR #126:** adds explanatory docstrings and examples and receives detailed review from Commelin.

### 6.3 Documentation and audience negotiation

- **PR #120:** Kevin Buzzard proposes removing irrelevant imports and explaining every remaining command for non-expert readers. Commelin replies that apparently redundant imports also provide evidence against notation tricks.
- **PR #121:** Buzzard argues for inline comments so readers can follow code and explanation together. Topaz says the original target audience was mathematicians familiar with the mathematics but unfamiliar with Lean, while agreeing that more detail may help. Both PRs remain open at the snapshot date.

### 6.4 Infrastructure and project coordination

Issues #32, #37 and #38 track Theorem 9.5, sorry-free CI and olean caches. Issue #78 tracks completion of the challenge. The PR history includes CI, cache, mathlib-bump and toolchain maintenance alongside mathematical formalization.

### 6.5 Liquid Tensor case finding

The PR census shows a relatively concentrated mathematical collaboration network, with Topaz producing many examples and Commelin reviewing and shaping them. The project explicitly turns definitions into objects of public inspection. Semantic auditability is therefore a socially produced practice, involving examples, mathematical discussion, documentation and review. The two open documentation PRs show that the intended audience and degree of transparency were still being negotiated.

## 7. Cross-case contribution-network comparison

| Dimension | Riemann | Navier–Stokes | AlphaProof Nexus | Liquid Tensor |
|---|---|---|---|---|
| Public repository structure | Large multi-actor maintenance network | Two-commit release snapshot | Small output archive plus external integration network | Small, sustained collaborative project |
| Main visible human roles | Maintainers, proof refactorers, infrastructure, auditors | OpenAI release account; external critics elsewhere | Output publisher, formal-conjecture integrators, reviewers, auditors | Mathematical lead, formalizers, example authors, reviewers, infrastructure maintainers |
| Review visibility | High and multi-layered | Low inside the project repo | High in Formal Conjectures PRs | High in selected mathematical PRs |
| Semantic checking | Literature attribution, statement audits, independent replay | External proof-to-Lean correspondence critique | Target corrections, variant checks, formal statement review | Examples, definitions, Blueprint and human discussion |
| Attribution pattern | Original author plus broad maintenance contributors | Organization-level authorship in metadata | Agent named as prover; human integration and review visible | Human mathematical and formalization credit distributed; machine treated as assistant/checker |
| Key limitation | PR counts mix historical branches and many types of work | No public PR history does not prove no internal collaboration | Output archive alone misses integration and review work | Public accessibility does not prove every reader actually checks examples |

## 8. Methodological limitations and safeguards

1. GitHub commits and PRs are not direct measures of mathematical labour or intellectual originality.
2. PR author, reviewer and maintainer roles are recorded as platform actions; they do not reveal private belief or all off-platform work.
3. The RH contributor count includes `alpoge` branch history and should not be interpreted as theorem authorship.
4. The Navier–Stokes repository's lack of PRs/issues is a property of its public repository record, not proof of no collaboration.
5. AlphaProof's QuantumOptics `sorry` issue is not evidence that the Erdős proof items are `sorry`; the latter have a separate external replay record.
6. LTE's 49 automated-upgrade issues are not substantive mathematical contributions and are excluded from human interaction coding.
7. The PR samples identify observable relations, not a complete social network. A complete network study would also require systematic reviewer extraction, issue comments, forks, citations, and downstream repository dependencies.

## 9. Interim conclusion

The four cases exhibit four different public organizations of mathematical labour and recognition:

- Riemann: large-scale community maintenance with explicit archival, provenance and review governance.
- Navier–Stokes: centralized publication snapshot, with external adjudication largely outside the repository.
- AlphaProof: machine-produced results enter public mathematical status through a human review and integration network.
- Liquid Tensor: semantic auditability is built through collaborative examples, documentation and mathematical review.

This supports the research question about how the same formal verification technology can participate in different authority and subject-position structures. It does not yet establish the second-stage Žižekian interpretation. The next stage must test whether these differences constrain or facilitate warrant-scope transfer, especially in the AlphaProof/LTE comparison.
