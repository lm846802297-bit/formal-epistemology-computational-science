# Collection Log

## 2026-11-28 — Initial empirical research architecture

### Repository and manuscript inspection

- Inspected lm846802297-bit/philosophy-papers.
- Existing full-length base: research/phte-full-length-revision.
- Existing PR #6 head: research/phte-zizek-materialist-revision; open and Draft.
- PR #6 changes the manuscript only.
- Created separate branch research/empirical-evidence-dossier from research/phte-full-length-revision, keeping empirical assets separate from manuscript edits.
- Base manuscript contains four cases: Riemann, Navier–Stokes, AlphaProof Nexus and Liquid Tensor. Preserve this architecture during evidence collection.

### Scholarly sources retrieved or inspected

Full texts inspected:
- Pease et al. (2020), Using crowdsourced mathematics to understand mathematical practice.
- The mathlib Community (2020), The Lean Mathematical Library.
- Baanen et al. (2025), Growing Mathlib.
- Ochigame (2024), Automated Mathematics and the Reconfiguration of Proof and Labor.
- Habgood-Coote and Tanswell, Group Knowledge and Mathematical Collaboration.
- Habgood-Coote (2020), Group Inquiry.
- Hansson (2020), Technology and Mathematics.
- Kallel and El Louadi (2026), Verification abundance, adjudication scarcity (preprint).
- López-Corona (2026), From Authorial Mathematics to Studio Mathematics (preprint).

Abstract only:
- De Toffoli and Tanswell, Trust in Mathematics.
- MacKenzie, Computing and the cultures of proving.

### Repositories and public records already inspected

- LTE repository and PRs #113, #126, #120 and #121.
- AlphaProof results archive at pinned tree 0647711a71183c1ea492ad60860776617ce1ea88.
- Formal Conjectures PR #3778.
- Erdős problem data and community AI-contributions wiki.
- OpenAI NavierStokesAndEuler README and Comparator instructions.
- RH institutional statement and MIT verification archive previously located; immutable snapshot still needs recording.

### Methodological decisions

- Core method: documentary digital ethnography and comparative case study.
- Supporting methods: process tracing, repository trace analysis, discourse analysis and citation/dependency analysis.
- No interviews have been conducted; do not describe this as interview-based ethnography.
- Treat public statements as situated accounts, not transparent reports of private belief.
- Code negative and contradictory evidence as well as support.
- Do not assume all four cases confirm the theory.

### Priority novelty checks

Two 2026 preprints closely overlap the topic:
- Kallel and El Louadi distinguish derivational validity, representational fidelity and epistemic significance; argue that abundant machine checking can transfer burden to expert adjudication.
- López-Corona compares Polymath and LTE and develops studio mathematics and contribution-authority trace.

Study these carefully before claiming novelty for a three-layer warrant distinction, distributed mathematical labour or LTE/Polymath comparison. The intended contribution must remain the narrower Žižekian account of how a locally reliable credential can become a material bearer of wider public authority.

## Next tasks

1. Pin exact commits for RH, Navier–Stokes, AlphaProof and LTE technical repositories.
2. Record exact core theorem declarations and informal target statements.
3. Collect relevant PR/review/issue histories, including closed and rejected changes.
4. Systematically sample public reception, independent assessments and responses.
5. Search citation and dependency graphs for actual downstream reuse.
6. Create machine-readable evidence ledger using the schema in coding-framework.md.
7. Archive raw artifacts and compute SHA-256 only after actual retrieval.
8. Retrieve full texts for MacKenzie and De Toffoli/Tanswell where lawful access permits.
9. Record inaccessible sources rather than replacing them with summaries.


## 2026-11-28 — First-pass GitHub collaboration and contribution-network survey

### Repository census

- Riemann: inspected repository README and generated CONTRIBUTORS.md. The contributor file lists 192 accounts and sums to 6,079 merged-PR counts, including the earlier `alpoge` branch history. Created a top-20 CSV snapshot.
- Navier–Stokes: inspected the full public commit history. Two commits, both by `balexeev-oai`; root commit `8937a8f4cbc7abaab5e9e97d1cc7f5d2319d9538` adds 2,496 files / 616,833 lines. No public PRs or issues found in the repository.
- AlphaProof results archive: six commits (five by `aferr`, one CI commit by `eric-wieser`), four issues, no PRs. Inspected issues #1–#4. The QuantumOptics `sorry` issue is explicitly separated from the Erdős proof set.
- Formal Conjectures: purposively inspected PRs #3778, #4384, #3737, #3721, #3643, #3604 and #2398. PR #4384 has 53 commits and 135 comments, including detailed review of statement scope and an m=8-only result.
- Liquid Tensor: enumerated 57 PRs and 76 issues. Fetched all 57 PR metadata records; 49 merged, 6 closed unmerged and 2 open; 15 PR author accounts. 49 issue titles are automatic-upgrade failures and are excluded from substantive human-interaction coding.

### Event-level evidence captured

- Riemann: cache/build PRs, import cleanup, out-of-scope proof proposal, source provenance, donor-runner infrastructure, reviewed batch merges, citation/attribution audit, original-archive versus refactor dispute, structural audit discussion, independent replay and checker reports.
- Navier–Stokes: two release commits and external critique as a separate scholarly channel.
- AlphaProof: output archive authorship, missing natural-language artifact request, proof provenance issue, independent replay, Formal Conjectures status change, extensive OEIS statement review, attribution corrections and counterexample-led formalization fixes.
- LTE: CI/sorry-free workflow, theorem milestones, p-Banach and Ext semantic examples, Radon/profinite examples, open documentation/audience negotiations.

### Machine-readable outputs

- `github-collaboration-analysis.md`
- `contribution-network.md`
- `github-event-ledger.csv` (46 event records)
- `liquid-tensor-pr-census.csv` (57 PR records)
- `riemann-contributors-top.csv` (20-account snapshot)
- `alphaproof-formal-conjectures-pr-sample.csv` (7 selected integration/review PRs)
- `navier-stokes-commit-history.csv` (2 public commits)

### PR review snapshot and event-network data

- Retrieved PR metadata and review-event snapshots for eight purposively selected Riemann PRs (#1, #7, #8, #12, #64, #101, #115, #9842), eight LTE PRs (#95, #96, #104, #107, #113, #120, #121, #126), and seven AlphaProof/Formal Conjectures PRs (#3778, #4384, #3737, #3721, #3643, #3604, #2398).
- Selected LTE PR review events: #95 (9 COMMENTED + 1 APPROVED), #96 (1 APPROVED), #104 (1 APPROVED), #107 (5 COMMENTED + 1 APPROVED), #113 (8 COMMENTED + 1 APPROVED), #120 (1 APPROVED while still open), #121 (no review event returned), #126 (2 COMMENTED + 1 APPROVED).
- Selected AlphaProof/Formal Conjectures PRs: #4384 (135 issue comments and 49 review events: 46 COMMENTED, 3 APPROVED), #3721 (1 CHANGES_REQUESTED and 1 APPROVED), #2398 (2 APPROVED and 2 COMMENTED), and approval events on #3778, #3737, #3643 and #3604.
- The selected Riemann aggregate PR records returned no PR review events through the review endpoint. Some descriptions refer to reviewed component PRs, approvals or merge-queue checks; these are not recoded as review events on the aggregate PR itself.
- Added github-pr-review-sample.csv with 23 PR snapshots, exact merge SHAs where merged, and separate issue-comment/review-event counts.
- Expanded 46 event records into 78 actor-event links in github-event-participation-edges.csv. The relation is deliberately NAMED_AS_ACTOR_IN_EVENT; the CSV does not infer author/reviewer/approver role from a semicolon-separated actor field. Typed qualitative roles remain in contribution-network.md.
- A complete network graph is still not claimed: event participation edges are a reproducible event index, not a complete social network or co-authorship graph.

### Important methodological conclusions

- Do not compare raw PR counts across the four repositories: their purposes and histories differ.
- The Riemann contributor count includes earlier `alpoge` history and is not a measure of theorem authorship.
- Navier–Stokes' lack of public PRs/issues is a property of the public repository, not proof of no internal collaboration.
- AlphaProof's results archive is not the same as its human integration network; Formal Conjectures is essential.
- The AlphaProof QuantumOptics `sorry` issue is not evidence that the Erdős proof items contain `sorry`.
- LTE has a concentrated author/reviewer network; the examples and docs are collaboratively produced and reviewed.
- No raw repository files have been archived locally in this step; therefore no SHA-256 values are claimed. Immutable Git commit/blob identifiers and PR numbers are recorded instead.

### Remaining Stage 1 tasks

1. Complete a targeted review of RH PR/review histories beyond the purposive sample, especially source-attribution and proof-refactor batches.
2. Expand Formal Conjectures sampling around AlphaProof results and collect review threads for the selected PRs.
3. Capture exact head/merge commit SHAs for all selected PRs; seven AlphaProof/Formal Conjectures merge SHAs are now recorded in the PR-sample CSV.
4. Search downstream citations, imports, forks and actual reuse for all four cases.
5. Complete the public reception sample and record counter-evidence.


## 2026-11-28 — Second-stage theoretical synthesis: AlphaProof and LTE

- Reopened the exact manuscript snapshot at blob `403657444bff5686bf795872b26005f73bce8409` and reviewed the theoretical framework, AlphaProof subsection, LTE subsection, contribution statement and conclusion.
- Re-examined the full texts of Kallel & El Louadi (2026) and López-Corona (2026) as priority novelty checks.
- Created `two-case-theory-synthesis.md`.
- Updated `theory-evidence-map.md` with case-specific judgments and inference limits.
- No manuscript text was changed.

### Main synthesis

- AlphaProof provides strong evidence of credential-centred recognition and asymmetrical solver attribution, but only localized/partial warrant-scope transfer. Human validation, statement correction, variant-specific status and independent replay constrain the stronger fetishistic interpretation.
- LTE provides a documented counter-practice: semantic checks and provenance are made operative in project workflow and public exposition. It constrains certificate-only attribution at the procedural level, but the evidence does not show that it causally changes downstream community recognition.
- Neither case establishes community-wide private belief or universal fetishistic disavowal.
- The comparison is contrastive, not a matched causal test.
- Kallel & El Louadi already distinguish derivational validity, representational fidelity and epistemic significance; López-Corona already develops studio mathematics and contribution-authority trace. The distinctive claim must remain the Žižekian account of how a genuine local warrant becomes a material bearer of wider public recognition and attribution.

### Next sequential step

Complete the remaining Stage 1 evidence collection on public reception and downstream reuse before treating the overall empirical phase as closed. Only after that should the theory-evidence map be finalized and manuscript revisions considered.


## 2026-11-28 — Sequential research-stage acceptance

### Stage 1: GitHub collaboration archives and contribution networks

- Accepted at the documentary scope stated in stage1-github-acceptance.md.
- Added 78 actor-event links from 46 selected event records. These are named participation edges, not inferred author/reviewer roles.
- Added a 23-PR metadata/review sample across Riemann, LTE and AlphaProof/Formal Conjectures, including immutable merge SHAs where available.
- Updated contribution-network.md with PR review event counts and the distinction between issue comments and formal review states.
- Stage 1 does not claim a complete typed social network, full internal collaboration history, or a downstream reuse census.

### Stage 2: AlphaProof/LTE theoretical synthesis

- Conducted after Stage 1 acceptance.
- Revised two-case-theory-synthesis.md and theory-evidence-map.md.
- Main refinement: credential circulation, warrant-scope transfer and fetishistic disavowal are three distinct levels.
- AlphaProof: credential-centred recognition and agent solver attribution are observable; possible scope compression is localized to headline/benchmark framing. PR #3778 is a reviewed variant-specific status change, not automatically an unwarranted transfer.
- LTE: semantic auditability is a procedural counter-practice built through examples, Blueprint, discussion and review; causal effects on downstream recognition are not demonstrated.
- Neither case establishes community-wide private belief or universal fetishistic disavowal.
- No manuscript text was changed.

### Acceptance records

- stage1-github-acceptance.md
- stage2-theory-synthesis-acceptance.md

### Next research boundary

The two requested sequential tasks are complete. The wider empirical phase still has distinct future work: systematic public reception, downstream citations/reuse, exact raw artifact archiving with SHA-256, and any interview-based research under a separate consent/ethics protocol. These are not retroactively treated as completed.
