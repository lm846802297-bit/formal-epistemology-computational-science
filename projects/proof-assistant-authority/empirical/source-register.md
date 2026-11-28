# Source Register

Snapshot date: 2026-11-28. Status: located / inspected / version-pinned / to-collect. This is a structured starting corpus, not an exhaustive collection.

## A. Riemann Hypothesis: 2026 Lean verification archive

| ID | Source | Evidence role | Status and caveat |
|---|---|---|---|
| RH-01 | [Lean FRO and Mathlib joint statement](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/) | Institutional certification, statement vetting, replay claims | Inspected. Certification is not a survey of universal mathematical consensus. |
| RH-02 | [Alpöge research note and archive](https://alpo.ge/) | Primary mathematical exposition and Lean artifact | Located. Pin exact archive release and hashes. |
| RH-03 | [Sutherland MIT verification files](https://math.mit.edu/~drew/grh/) | Independent verification | Inspected. Independent replay is distinct from adjudicating informal correspondence. |
| RH-04 | [Readable Lean roadmap, Zenodo](https://doi.org/10.5281/zenodo.24562451) | AI-mediated exposition | Located. Record its generation and checking provenance. |
| RH-05 | [Emmerson critique](https://doi.org/10.20944/preprints202611.2463.v1) | Independent counter-assessment | Located. Preprint; assess argument and responses independently. |
| RH-06 | [Mathlib RiemannZeta definition](https://leanprover-community.github.io/mathlib4_docs/Mathlib/NumberTheory/LSeries/RiemannZeta.html) | Exact formal target | Inspected. Pin source commit and compare with informal statement. |
| RH-07 | Public Lean, Mathlib and mathematician discussions | Reception and follow-up | To collect systematically, with dated thread locators. |

Key question: does public certification make its grounds and division of labour visible, and how does this affect the result's public status?

## B. Navier–Stokes: OpenAI 2026 announcement and Lean formalization

| ID | Source | Evidence role | Status and caveat |
|---|---|---|---|
| NS-01 | [OpenAI announcement](https://openai.com/index/navier-stokes-solution/) | Institutional framing and public claim | Located. Interested participant account, not independent adjudication. |
| NS-02 | [OpenAI Lean repository](https://github.com/openai/NavierStokesAndEuler) | Primary technical archive | Inspected README and Comparator instructions. Pin commit, toolchain and declarations. |
| NS-03 | [Navier–Stokes analytical paper](https://cdn.openai.com/pdf/32d9f210-8b73-45e0-91bc-82a30aef8a9a/navier-stokes.pdf) | Primary mathematical exposition | Located. Compare theorem and proof route with Lean declarations. |
| NS-04 | [Bastounis, Circelli and Hansen critique](https://arxiv.org/abs/2610.08144) | Independent critique | Located. A proof-route discrepancy is not automatically a theorem-statement mismatch or kernel failure. |
| NS-05 | [Clay official problem description](https://www.claymath.org/wp-content/uploads/2022/06/navierstokes.pdf) | Authoritative target statement | Located. Compare domains, quantifiers, forcing and solution concepts. |
| NS-06 | [Cotton, The formal statement](https://navier.microprediction.org/formal.html) | Independent statement analysis | Located. Verify comparison independently and pin version. |
| NS-07 | [Comparator instructions](https://github.com/openai/NavierStokesAndEuler/tree/main/ComparatorChallenges) | Independent checker procedure | Inspected. Checker success does not adjudicate significance, exposition or credit. |
| NS-08 | Public mathematical responses, seminars, issues and citations | Reception and adjudication | To collect. News repetition alone is not mathematical uptake. |

Key question: how are the formal theorem, written proof and public solution claim related, checked and contested?

## C. AlphaProof Nexus and Erdős problems

| ID | Source | Evidence role | Status and caveat |
|---|---|---|---|
| AP-01 | [Tsoukalas et al., Science](https://doi.org/10.1126/science.aej2213) | Benchmark, expert validation, target corrections and attribution | Located. Primary research article. |
| AP-02 | [Pinned AlphaProof results archive](https://github.com/google-deepmind/alphaproof-nexus-results/tree/0647711a71183c1ea492ad60860776617ce1ea88) | Primary proof archive | Version-pinned. Record per-file hashes and distinguish Lean outputs from prose proofs. |
| AP-03 | [Formal Conjectures PR #3778](https://github.com/google-deepmind/formal-conjectures/pull/3778) | Localized formal recognition event | Inspected. Variant status changed from research open to research solved; not proof of community-wide consensus. |
| AP-04 | [Erdős problems database](https://github.com/teorth/erdosproblems) | Community status register | Inspected. Pin data file commit before citing individual dates. |
| AP-05 | [AI contributions wiki](https://github.com/teorth/erdosproblems/wiki/AI-contributions-to-Erd%C5%91s-problems) | Community attribution classification | Inspected. Provisional and non-definitive; preserve snapshot date. |
| AP-06 | [Toledo independent audit](https://carlostoledo.co/reports/alphaproof-nexus.html) | External technical audit | Inspected. Ten proof items replayed through two kernels; separates derivation from original-problem correspondence. |
| AP-07 | [Erdős, Some problems in number theory](https://mathematica-pannonica.ttk.pte.hu/articles/mp05-2/mp05-2-261-269.pdf) | Original problem source | Located. Compare original density wording with formal variants. |
| AP-08 | Later papers, citations, forks and repository reuse | Actual uptake | To collect. Stars, downloads and views do not establish epistemic reuse. |

Key question: how do formal machine-generated results acquire public status and solver attribution, and where are target selection and human validation located?

## D. Liquid Tensor Experiment

| ID | Source | Evidence role | Status and caveat |
|---|---|---|---|
| LTE-01 | [Scholze original challenge (2020)](https://xenaproject.wordpress.com/2020/12/05/liquid-tensor-experiment/) | Original motivation | Inspected. |
| LTE-02 | [Scholze progress account (2021)](https://xenaproject.wordpress.com/2021/06/05/half-a-year-of-the-liquid-tensor-experiment-amazing-developments/) | Participant account of attribution and human semantic judgment | Inspected. |
| LTE-03 | [Commelin project update (2021)](https://leanprover-community.github.io/blog/posts/lte-update/) | Project lead account | Located. |
| LTE-04 | [Mathlib completion announcement (2022)](https://leanprover-community.github.io/blog/posts/lte-final/) | Community recognition and contributors | Inspected. |
| LTE-05 | [Lean Liquid repository](https://github.com/leanprover-community/lean-liquid) | Technical and collaboration archive | Inspected. Pin exact commit. |
| LTE-06 | [LTE Blueprint](https://leanprover-community.github.io/liquid/) | Public proof exposition and dependency graph | Inspected. |
| LTE-07 | [Topaz, Definitions in LTE](https://leanprover-community.github.io/blog/posts/lte-examples/) | Semantic audit rationale | Inspected. |
| LTE-08 | [PR #113, Radon examples](https://github.com/leanprover-community/lean-liquid/pull/113) | Collaboration trace | Inspected. |
| LTE-09 | [PR #126, example modifications](https://github.com/leanprover-community/lean-liquid/pull/126) | Collaboration trace | Inspected. |
| LTE-10 | [PR #120, comments](https://github.com/leanprover-community/lean-liquid/pull/120) | Documentation negotiation | Inspected; open PR is negotiation, not settled policy. |
| LTE-11 | [PR #121, profinite example comments](https://github.com/leanprover-community/lean-liquid/pull/121) | Audience and accessibility negotiation | Inspected. |
| LTE-12 | [Buzzard retrospective (2022)](https://xenaproject.wordpress.com/2022/09/12/beyond-the-liquid-tensor-experiment/) | Human/machine attribution | Inspected. |
| LTE-13 | [Commelin and Topaz (2024), Abstraction boundaries](https://doi.org/10.1090/bull/1831) | Formalization as mathematical practice | Located. |
| LTE-14 | Public Zulip discussion and downstream formalizations | Reception and reuse | To collect systematically. |

Key question: does public semantic auditability redistribute authority and make human mediation visible, and what trust structures remain?

## E. Methodological literature

| ID | Source | Relevance | Status |
|---|---|---|---|
| M-01 | MacKenzie, [Computing and the cultures of proving](https://doi.org/10.1098/rsta.2005.1649) | Sociology of proof | Abstract inspected; full text not retrieved |
| M-02 | MacKenzie, *Mechanizing Proof: Computing, Risk, and Trust* (2001) | Historical sociology of mechanized proof | Retrieve book |
| M-03 | Rosental, [Certifying Knowledge](https://doi.org/10.1177/000312240306800407) | Ethnography, interviews and theorem recognition | Located |
| M-04 | De Millo, Lipton and Perlis, [Social Processes and Proofs](https://doi.org/10.1145/359104.359106) | Social processes of proof | Located |
| M-05 | Mathlib Community, [The Lean Mathematical Library](https://doi.org/10.1145/3372885.3373824) | Community governance and collective authorship | Full text inspected |
| M-06 | Baanen et al., [Growing Mathlib](https://doi.org/10.1007/978-3-032-07021-0_4) | Maintenance, review, triage and maintainer load | Full text inspected |
| M-07 | Pease et al., [Using crowdsourced mathematics](https://doi.org/10.1007/s11858-020-01181-7) | Digital traces, network analysis and ethnography | Full text inspected |
| M-08 | Habgood-Coote and Tanswell, [Group Knowledge and Mathematical Collaboration](https://doi.org/10.1017/epi.2021.26) | Group knowledge and division of labour | Full text inspected |
| M-09 | Habgood-Coote, [Group Inquiry](https://doi.org/10.1007/s10670-020-00232-5) | Distributed inquiry and epistemic labour | Full text inspected |
| M-10 | Ochigame, [Automated Mathematics and Proof and Labor](https://doi.org/10.1090/bull/1821) | Automation, labour, credit and authorship | Full text inspected |
| M-11 | De Toffoli and Tanswell, [Trust in Mathematics](https://doi.org/10.1093/philmat/nkaf019) | Mathematical trust and proof checking | Abstract only |
| M-12 | Pease et al., [Explanation in mathematical conversations](https://doi.org/10.1098/rsta.2018.0159) | Empirical mathematical interaction | Located |
| M-13 | Gargiulo et al., [Distribution of labor in collaborative science](https://doi.org/10.1007/s41109-022-00456-0) | Polymath network analysis | Located |
| M-14 | Kallel and El Louadi, [Verification abundance, adjudication scarcity](https://arxiv.org/abs/2608.28997) | Adjacent three-layer warrant argument | Full text inspected; preprint and priority risk |
| M-15 | López-Corona, [From Authorial Mathematics to Studio Mathematics](https://arxiv.org/abs/2608.22194) | LTE/Polymath comparison and contribution-authority | Full text inspected; preprint and priority risk |
| M-16 | Hansson, [Technology and Mathematics](https://doi.org/10.1007/s13347-019-00348-9) | Material and technological dependence of mathematics | Full text inspected |

## Collection priorities

1. Pin exact commits for all four technical repositories.
2. Record core theorem declarations and target statements.
3. Collect complete relevant PR/review/issue histories, including rejected and closed changes.
4. Systematically sample public reception, independent assessments and responses.
5. Search citation and dependency graphs for actual downstream reuse.
6. Build a machine-readable evidence ledger.
7. Archive raw source files and compute SHA-256 only after actual retrieval.
8. Retrieve full texts for M-01, M-02 and M-11 where lawful access permits.
9. Study M-14 and M-15 carefully before claiming novelty for a three-layer warrant distinction, distributed labour or the LTE comparison.


## F. GitHub collaboration archives and contribution-network sources

| ID | Source | Type / evidence role | Status | Main use / caveat |
|---|---|---|---|---|
| GH-RH-01 | [Riemann repository README](https://github.com/leanprover-community/riemann-hypothesis/blob/main/README.md) | Project scope and branch provenance | inspected; blob `6a98a3faa41f6c59cf0fb4b8e4d4b4ca7c45c1d1` | Describes main/alpoge/original branch roles and project goals. |
| GH-RH-02 | [Riemann CONTRIBUTORS.md](https://github.com/leanprover-community/riemann-hypothesis/blob/main/CONTRIBUTORS.md) | Generated contributor counts | inspected; blob `f8e211a17347be739b2b89ab582ca4bbb0f97cdf` | 192 accounts; summed 6,079 merged-PR counts, including alpoge history. Not theorem authorship. |
| GH-RH-03 | [Riemann GitHub event sample](github-event-ledger.csv) | PR/issue and audit events | inspected | Selected PRs #1, #7, #8, #12, #64, #101, #115, #9842; Issues #39, #47, #56, #96, #8738, #8747. |
| GH-NS-01 | [OpenAI NavierStokesAndEuler commit 8937a8f4](https://github.com/openai/NavierStokesAndEuler/commit/8937a8f4cbc7abaab5e9e97d1cc7f5d2319d9538) | Root release commit | inspected; immutable SHA | 2,496 files and 616,833 added lines; author `balexeev-oai`. |
| GH-NS-02 | [OpenAI NavierStokesAndEuler commit f9e8bc5b](https://github.com/openai/NavierStokesAndEuler/commit/f9e8bc5b38b6e212696e8a30e3e91517af887bbd) | Follow-up release commit | inspected; immutable SHA | Same author; repository has two commits and no public PRs/issues in the inspected snapshot. |
| GH-APN-01 | [AlphaProof Nexus results commit history](https://github.com/google-deepmind/alphaproof-nexus-results/commits/main) | Output archive provenance | inspected | Six commits: five by `aferr`, one CI commit by `eric-wieser`. |
| GH-APN-02 | [Formal Conjectures PR #3778](https://github.com/google-deepmind/formal-conjectures/pull/3778) | Localized status transition | inspected | Upper-density variant of #741; agent attribution and approval. |
| GH-APN-03 | [Formal Conjectures PR #4384](https://github.com/google-deepmind/formal-conjectures/pull/4384) | Human review and integration of AlphaProof OEIS outputs | inspected | 53 commits, 135 comments, detailed statement correction. |
| GH-APN-04 | [Formal Conjectures PR #3737](https://github.com/google-deepmind/formal-conjectures/pull/3737), [#3721](https://github.com/google-deepmind/formal-conjectures/pull/3721), [#3643](https://github.com/google-deepmind/formal-conjectures/pull/3643), [#3604](https://github.com/google-deepmind/formal-conjectures/pull/3604), [#2398](https://github.com/google-deepmind/formal-conjectures/pull/2398) | Attribution, provenance, and counterexample-led correction | inspected | Purposive sample, not full Formal Conjectures PR census. |
| GH-APN-05 | [AlphaProof Formal Conjectures PR sample](alphaproof-formal-conjectures-pr-sample.csv) | Machine-readable integration/review sample | inspected | Seven PRs with author, review actors, commit counts, merge SHAs and event summaries. |
| GH-LTE-01 | [Liquid Tensor PR census](liquid-tensor-pr-census.csv) | Complete PR search result for repository snapshot | inspected | 57 PRs, 49 merged, 6 closed unmerged, 2 open, 15 author accounts. |
| GH-LTE-02 | [Liquid Tensor issues](https://github.com/leanprover-community/lean-liquid/issues) | Project task and CI history | inspected | 76 issues returned; 49 are automated-upgrade failures and excluded from substantive interaction counts. |
| GH-LTE-03 | [Liquid Tensor PR #95–#126 sample](https://github.com/leanprover-community/lean-liquid/pulls?q=is%3Apr) | Semantic examples, documentation and review | inspected | Key records #95–#107, #113, #115, #120, #121, #126. |
| GH-NS-03 | [Navier–Stokes commit history](navier-stokes-commit-history.csv) | Machine-readable public release history | inspected | Two commits by one public account at the snapshot date. |

Machine-readable event-level records are in `github-event-ledger.csv`; `github-event-participation-edges.csv` expands its 46 records into 78 actor-event links, retaining unresolved roles where the actor field alone does not establish a specific action; `github-pr-review-sample.csv` records 23 purposively selected PRs with issue-comment counts, review states, and immutable merge SHAs.  the complete LTE PR census and pinned Riemann contributor snapshot are separate CSV files.