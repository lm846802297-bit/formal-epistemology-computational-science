# Stage 1 Acceptance: GitHub Collaboration Archives and Contribution Networks

**Snapshot:** 2026-11-28  
**Status:** completed as a first documentary GitHub study; not a complete ethnography or full four-case social network.

## 1. Scope accepted

The task was to investigate the four cases' public GitHub collaboration archives and observable contribution networks, including repository structure, commits, pull requests, comments, review events, status transitions, correction events and independent replay records.

The study uses a repository census where the available search result permits it, and a purposive event sample where a full event census is not yet available. These methods are kept distinct.

## 2. Case-level results

| Case | Observed public archive | Contribution-network finding | Principal limitation |
|---|---|---|---|
| Riemann | Generated contributor file lists 192 accounts and 6,079 summed merged-PR counts, including prior alpoge history; selected governance/provenance/audit events | Large maintenance and governance structure: cache/build, source provenance, refactoring, merge-queue, literature attribution and independent checking | Merged-PR counts are activity indicators, not theorem authorship or unique labour; selected PR endpoint returned no review events for the eight aggregate PR snapshots |
| Navier–Stokes | Two public commits, both by balexeev-oai; no public PRs/issues found in inspected repository snapshot | Public repository is a centralized release snapshot; external mathematical scrutiny appears in a separate scholarly channel | No inference about private/internal collaboration; repository trace cannot reconstruct OpenAI's internal production network |
| AlphaProof Nexus | Six commits in results archive (five aferr, one eric-wieser); four issues; no PRs in output archive; seven selected Formal Conjectures PRs | Output archive is concentrated, but integration network includes mo271, codrut3, Paul-Lez, mzhorvath1, XC0R and smmercuri; review corrects target statements, attribution and proof scope | Seven PRs are purposive, not full Formal Conjectures census; archive author is not the same as solver agent |
| Liquid Tensor | 57 PRs in retrieved census: 49 merged, 6 closed unmerged, 2 open; 76 issues; 15 PR author accounts | Concentrated but collaborative mathematical network; Topaz authors examples, Commelin reviews/co-ordinates, other contributors add examples and infrastructure; PRs expose semantic and documentation negotiation | 49 automated-upgrade issues excluded from substantive interaction coding; public PRs do not capture private Zulip or all off-platform labour |

## 3. Machine-readable evidence delivered

- github-event-ledger.csv: 46 selected event records with source URLs, locators, codes and inference limits.
- github-event-participation-edges.csv: 78 actor-event links expanded from the 46 records. Relation is NAMED_AS_ACTOR_IN_EVENT; ambiguous roles are not inferred from actor lists.
- github-pr-review-sample.csv: 23 purposively selected PR snapshots across RH, LTE and AlphaProof/Formal Conjectures, including comments, review states and immutable merge SHAs.
- liquid-tensor-pr-census.csv: 57 PR records.
- riemann-contributors-top.csv: top 20 accounts from a pinned generated contributor file; complete source file contains 192 accounts.
- alphaproof-formal-conjectures-pr-sample.csv: seven selected integration/review PRs.
- navier-stokes-commit-history.csv: two public commits.
- github-collaboration-analysis.md: four-case report.
- contribution-network.md: typed qualitative role map and cross-case comparison.

## 4. PR review evidence

Selected LTE review events include:
- #95: 9 COMMENTED and 1 APPROVED review events;
- #96: 1 APPROVED;
- #104: 1 APPROVED;
- #107: 5 COMMENTED and 1 APPROVED;
- #113: 8 COMMENTED and 1 APPROVED;
- #120: 1 APPROVED while still open;
- #121: no review event returned;
- #126: 2 COMMENTED and 1 APPROVED.

Selected AlphaProof/Formal Conjectures review events include:
- #4384: 135 issue comments and 49 review events (46 COMMENTED, 3 APPROVED);
- #3721: 1 CHANGES_REQUESTED and 1 APPROVED;
- #2398: 2 APPROVED and 2 COMMENTED;
- #3778, #3737, #3643 and #3604 each have approval events.

For the eight selected Riemann aggregate PRs, the review endpoint returned no review events. The underlying descriptions and related records mention reviewed component PRs and merge governance; these are not conflated with review events on the aggregate PR.

## 5. Cross-case empirical finding

The four public archives reveal different configurations:

1. Riemann: large-scale community maintenance and provenance governance.
2. Navier–Stokes: centralized public release snapshot and external scholarly scrutiny.
3. AlphaProof: concentrated proof-output archive connected to a broader human integration, correction and recognition network.
4. Liquid Tensor: concentrated mathematical collaboration with semantic examples, public documentation and review negotiation.

The most important empirical result is that the repository producing a proof artifact is not necessarily the same repository or network that integrates, reviews, attributes and publicly recognizes the result. AlphaProof is the clearest example: the output archive and Formal Conjectures integration network have different structures.

## 6. Acceptance checks

| Check | Result |
|---|---|
| Four cases have identified public repositories | Pass |
| Each case has source-version locators for inspected GitHub artifacts | Pass |
| Machine-readable event ledger exists | Pass |
| Machine-readable event participation edges exist | Pass |
| Selected PR metadata/review sample exists | Pass |
| LTE PR census and Riemann contributor snapshot exist | Pass |
| Qualitative role map distinguishes account actions from inferred roles | Pass |
| Cross-case report records counter-evidence and inference limits | Pass |
| Raw source artifacts archived and SHA-256 computed | Not completed; Git commit/blob IDs are recorded instead |
| Complete typed network graph for every case | Not claimed; current event edges preserve unresolved roles |
| Public reception and downstream reuse census | Outside this GitHub-focused stage; remains for the broader empirical phase |

## 7. Conclusion and handoff

The GitHub collaboration archive and contribution-network study is complete at the stated documentary scope. It provides a defensible first empirical basis for comparing how labour, review, semantic correction, status and attribution are organized in the four cases.

The study does not claim a complete social network, private belief, exhaustive reception analysis, or causal effects on mathematical behaviour.

**Stage 1 is accepted. Stage 2 may now proceed:** independently synthesize the AlphaProof and Liquid Tensor evidence to test credential-centred recognition, distributed semantic auditability, warrant-scope transfer, and the limits of the fetishistic-disavowal diagnosis. No manuscript revision is authorized by this acceptance record.
