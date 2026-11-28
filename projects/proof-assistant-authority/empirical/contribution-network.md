# Observed Contribution Network

**Snapshot:** 2026-11-28  
**Status:** purposive, documentary network map; not a complete social network.

## 1. Network model

Nodes:
- human GitHub accounts;
- institutions/project teams;
- repositories and formal artifacts;
- problem-status registers;
- independent auditors.

Edges are recorded only when public records show an action:
- authored;
- committed;
- reviewed/commented;
- approved;
- requested changes;
- merged;
- corrected;
- linked/imported;
- assigned status;
- independently replayed.

A PR author is not automatically the mathematical author. A reviewer is not automatically a semantic validator. A maintainer's merge is a localized institutional action, not proof of universal community consensus.

## 2. Riemann Hypothesis network

| Account / actor | Observed role | Evidence |
|---|---|---|
| Deicyde | High-volume contributor and maintainer; sets scope and citation rules | CONTRIBUTORS.md: 991 merged PRs; Issue #39 closes unverified citation-file proposal; Issue #56 explains repository goals |
| kim-em | Infrastructure and merge-queue maintainer | CONTRIBUTORS.md: 99 merged PRs; PR #7 cache/bootstrap; #101 donor workers; #115 cleanup batch; #9842 batch merge |
| sqrt-of-2 | Highest merged-PR count in generated contributor list | 1,056 merged PRs; activity count only, substantive role requires file/PR sampling |
| dga471 | High-volume contributor | 586 merged PRs; role requires file/PR sampling |
| aapolipponen | Source-to-statement attribution audit | Issue #39, AI-assisted initial list followed by withdrawal and source-checked subset |
| Antimatter543 | Provenance documentation | PR #64 |
| Jamesyc | External participant advocating preservation of original proof archive | Issue #56 |
| homeowmorphism | Creates sibling original-source archive and cache | Issue #56 discussion; sibling repository and PR #93 |
| tsarihan | Independent Apple Silicon reproduction | Issue #8738 |
| carlostoledo1891 | Independent formal verification audit | Issue #8747 |
| harryt ong / Visio-Vanitas / dial481 | Independent structural dependency analyses and responses | Issue #96 discussion; allegations and replies remain contested |

Observed network structure:
- Deicyde and kim-em occupy visible governance/maintenance positions.
- Many accounts contribute merged PRs, but contribution counts do not identify the mathematical content of their work.
- External auditors can enter the public record through issues without becoming repository contributors.
- A conflict over archival fidelity versus refactoring produces a sibling repository, not simply a code-level resolution.

## 3. Navier–Stokes network

| Account / actor | Observed role | Evidence |
|---|---|---|
| balexeev-oai | Author and committer of both public repository commits | Root commit 8937a8f4… (2,496 files, 616,833 additions) and update f9e8bc5… |
| OpenAI | Organization-level project authorship in formalization metadata | README and formalization.yaml |
| Bastounis, Circelli, Hansen | External scholarly critics of natural-language/Lean correspondence | arXiv:2610.08144; not a GitHub PR/review network in the project repository |

No public PRs or issues were found in the inspected repository. This records the shape of the public GitHub archive, not the absence of internal collaboration.

## 4. AlphaProof Nexus network

### Results archive

| Account / actor | Observed role | Evidence |
|---|---|---|
| aferr | Author/committer of five of six archive commits | Results, README, attempted-problem list and Stacks Project updates |
| eric-wieser | Adds Lean CI | Commit 9c591620… |
| rwst | Requests missing natural-language OEIS proofs | Issue #1 |
| lazarus-boop | Audits proof provenance in QuantumOptics file | Issue #3; this is not the Erdős proof set |
| carlostoledo1891 | Independent replay of published Erdős items | Issue #4 and external audit report |

### Formal Conjectures integration network

| Account / actor | Observed role | Evidence |
|---|---|---|
| mo271 | Integrator, PR author and frequent reviewer | PR #3778, #4384, #3737, #2398; 89 of 135 comments in #4384 |
| codrut3 | Detailed statement and scope reviewer | 42 of 135 comments in #4384; identifies incomplete conjecture statements and an m=8-only proof |
| Paul-Lez | Approval/merge authority | Approval on PR #3778 and #4384 review history |
| mzhorvath1 | Formal proof integrator | PR #3737 and #2398 |
| XC0R | Contributor using AlphaProof construction with Claude-assisted Lean translation | PR #3721 |
| smmercuri | Formal statement correction contributor | PR #3643 and #3604, both using AlphaProof counterexamples to find prior formalization defects |

Observed network structure:
- The published proof archive has concentrated commit authorship.
- The public recognition network is broader and includes integrators, statement reviewers and approvers.
- AlphaProof output is not simply accepted as a finished theorem: human review corrects the target, narrows the claim, changes status and records attribution.
- The agent also acts as a source of counterexamples that exposes errors in existing formalizations.

## 5. Liquid Tensor network

| Account / actor | Observed role | Evidence |
|---|---|---|
| jcommelin / Johan Commelin | Project lead, frequent reviewer, formalization coordinator | Issues #7, #32, #37, #38, #78; reviews and comments across PRs #95–#126 |
| adamtopaz / Adam Topaz | Main author of semantic example files and Ext examples | PRs #95, #96, #97, #105, #107, #113, #115, #126 |
| kbuzzard / Kevin Buzzard | Advocates inline explanations and reader-oriented documentation | Open PRs #120 and #121 |
| riccardobrasca | Mathematical/code review and library maintenance | PRs #90, #92, #94, #103, #112, #127; comments on examples |
| adomani | Reviewer/contributor on Radon-measure examples | PR #113 |
| bentoner | CI/cache infrastructure | PRs #44–#50 and #93, #99–#102 |
| faabian | PID module contribution | PRs #84 and #85 |
| faenuccio | p-Banach definition fix | Issue #82 and related PR history |

PR census:
- 57 PRs;
- 49 merged, 6 closed unmerged, 2 open;
- 15 author accounts.
- Author counts: Adam Topaz 14; Johan Commelin 11; bentoner 10; Riccardo Brasca 6; five accounts with 2 each; six accounts with 1 each.

Observed network structure:
- Commelin's review connects the example-file work to the wider formalization and Mathlib infrastructure.
- Topaz's examples are iteratively revised in response to comments.
- Buzzard's open documentation PRs expose a negotiation over the intended audience and what counts as sufficient public explanation.
- Semantic auditability is produced by collaboration; it is not a default property of the kernel or repository.

## 6. Cross-case network patterns

| Pattern | Riemann | Navier–Stokes | AlphaProof | LTE |
|---|---|---|---|---|
| High-volume contributor concentration | Yes | Not observable in repo | Yes in results archive | Moderate, with 15 PR authors |
| Visible review/approval | Extensive | No PR review | Extensive in Formal Conjectures | Extensive in selected mathematical PRs |
| Public semantic correction | Literature/source audits and target discussions | External critique | Formal target corrections and reviewer narrowing | Examples and definition review |
| Infrastructure labour | Highly visible | Mostly packaged in release | CI and repository integration | CI, cache, Mathlib bumps |
| Public attribution negotiation | Original author vs cleanup contributors | Organization-level authorship | Agent attribution plus human integration | Human distributed credit; machine role negotiated |

## 7. Inference limits

- This is a public-record interaction map, not a complete social network or co-authorship graph.
- Account names are platform identifiers; no private identity or motive is inferred.
- PR counts measure platform activity, not intellectual contribution.
- The absence of public PRs/issues does not prove absence of internal collaboration.
- Public comments evidence public positions and actions, not private belief.
