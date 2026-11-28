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
