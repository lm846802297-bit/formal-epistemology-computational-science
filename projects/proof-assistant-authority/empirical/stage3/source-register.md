# Stage 3 — Source Register

**Snapshot:** 2026-11-28  
**Search scope:** public documentary and scholarly sources for the four fixed cases.  
**Status:** first-pass collection and screening complete at the stated boundary.

## A. Existing public-reception evidence reused

The earlier PUBLIC_TRUST_AND_RECEPTION.md was read and reused. No existing source was silently replaced. Waring's problem was excluded because Stage 3 is restricted to the four cases below. Population-level surveys are retained only as contextual sources; none measures public trust in Lean or machine-checked proofs specifically.

| ID | Source | Date / version | Evidence use |
|---|---|---|---|
| CTX-01 | [Wellcome Global Monitor 2026](https://wellcome.org/insights/reports/wellcome-global-monitor-2026) | Published 2026-10-10; fieldwork 2025 | General trust-in-science baseline; not proof-assistant trust |
| CTX-02 | [Trust in scientists across 68 countries](https://doi.org/10.1038/s41562-024-02090-5) | Nature Human Behaviour, 2025 | Distinguishes trust in scientists from trust in abstract science |
| CTX-03 | [Bretter et al., Public skepticism about the use of AI in scientific research](https://doi.org/10.31234/osf.io/3h5n6_v1) | OSF preprint, 2026-03-05 | Survey evidence on AI disclosure; not Lean-specific |
| CTX-04 | [Chen & Jia, When researchers use AI](https://doi.org/10.1007/s43681-026-01039-w) | AI and Ethics, 2026-03-26 | Preregistered disclosure experiment; not proof-assistant-specific |
| CTX-05 | [Pew, How the US public and AI experts view AI](https://www.pewresearch.org/internet/2025/04/03/how-the-us-public-and-ai-experts-view-artificial-intelligence/) | 2025-04-03 | Expert/public attitude contrast; not scientific-proof trust |

These sources cannot establish that the public trusts or distrusts Lean. They provide context for the difference between trust in science, scientists, AI, and a formal proof artifact.

## B. Riemann Hypothesis (2026 Lean archive)

| ID | Source | Version / locator | Evidence use |
|---|---|---|---|
| RH-01 | [Lean FRO and Mathlib joint statement](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/) | 2026-11-21 | Formal-community certification and statement vetting |
| RH-02 | [Alpöge archive](https://alpo.ge/) | Public archive, 2026-11 | Primary proof exposition and Lean artifact |
| RH-03 | [Drew Sutherland verification files](https://math.mit.edu/~drew/grh/) | Public verification archive | Independent machine checking |
| RH-04 | [Waterloo reconstruction and verification page](https://www.math.uwaterloo.ca/~mrubinst/alpoge_claude_grh/) | Snapshot 2026-11-27 | Independent checking and human-readable reconstruction |
| RH-05 | [G.R.H. Polymath project](https://terrytao.wordpress.com/2026/11/24/g-r-h-polymath/) | 2026-11-24 | Collective mathematical reading, reconstruction and generalization |
| RH-06 | [Riemann community repository](https://github.com/leanprover-community/riemann-hypothesis) | README blob 6a98a3faa41f6c59cf0fb4b8e4d4b4ca7c45c1d1; CONTRIBUTORS blob f8e211a17347be739b2b89ab582ca4bbb0f97cdf | Version preservation, readable refactor, maintenance history |
| RH-07 | [Luke Sernau readable refactor](https://github.com/lsernau/grh-lean/commit/72fead102f) | Commit 72fead102f (pinned by community README) | Direct artifact refactor |
| RH-08 | [Jimmie Adriazola reconstruction](https://github.com/jimjamzola/RH-Alpoge-Reconstruction) | README blob 43b538f8e6c0b65e8dcb55d8cdd9c41b47b7a1e3 | Human-readable reconstruction; explicitly incomplete and conditional |
| RH-09 | [Nature coverage](https://www.nature.com/articles/d41586-026-03812-7) and [Nature follow-up](https://www.nature.com/articles/d41586-026-03835-0) | 2026-11-20 and 2026-11-25 | Public representation and named mathematician reactions |
| RH-10 | [Science Media Centre expert comments](https://www.sciencemediacentre.org/experts-comment-on-announcement-from-levant-alpoge-that-he-has-solved-the-riemann-hypothesis-with-the-help-of-claude/) | 2026-11-24 | Expert distinction between kernel checking, statement correspondence and understanding |
| RH-11 | [Alpöge, “Remark”](https://alpo.ge/remark.pdf) | 2026-11-20 | First-person account of collaboration with Claude and division of mathematical work |
| RH-12 | [Clay Mathematics Institute, Riemann Hypothesis](https://www.claymath.org/millennium/Riemann-Hypothesis/) | Status checked 2026-11-28; page labels problem “Active” | Official institutional status; not a prize award or acceptance statement |
| RH-13 | [Clay Mathematics Institute, Millennium Prize rules](https://www.claymath.org/millennium-problems/rules/) | Rules adopted 2018-09-26; accessed 2026-11-28 | Qualifying publication, two-year interval, and general-acceptance requirements for prize consideration |

The community README states that the original branch preserves the first public release, the alpoge branch preserves earlier cleanup history, and main is based on a readable refactor. The generated contributor file lists 192 accounts and 6,079 merged-PR counts, including the earlier alpoge history. These are repository-maintenance measures, not theorem authorship.

## C. Navier–Stokes (OpenAI, 2026)

| ID | Source | Version / locator | Evidence use |
|---|---|---|---|
| NS-01 | [OpenAI announcement](https://openai.com/index/navier-stokes-solution/) | 2026-09-08 | Institutional framing and public claim |
| NS-02 | [Initial OpenAI repository commit](https://github.com/openai/NavierStokesAndEuler/commit/8937a8f4cbc7abaab5e9e97d1cc7f5d2319d9538) | 2026-09-08 | Initial formal artifact |
| NS-03 | [Second OpenAI repository commit](https://github.com/openai/NavierStokesAndEuler/commit/f9e8bc5b38b6e212696e8a30e3e91517af887bbd) | 2026-09-10 | Added the actual candidate and theorem files that discharge energy and support obligations |
| NS-04 | [Bastounis, Circelli & Hansen, Navier-Stokes lost in translation](https://arxiv.org/abs/2610.08144) | arXiv:2610.08144, 2026-10-06 | Independent critique of paper-to-Lean proof-route correspondence |
| NS-05 | [New Scientist report](https://www.newscientist.com/article/2592824-openai-mistranslated-mathematics-into-code-for-its-navier-stokes-proof/) | 2026-10-08 | Public response and OpenAI acknowledgement |
| NS-06 | [King's College London summary](https://www.kcl.ac.uk/news/openais-navier-stokes-proof-called-into-question) | 2026-10-27 | Independent summary of the mismatch dispute |
| NS-07 | [cert-machine audit](https://github.com/carlostoledo1891/cert-machine/tree/47a01c2e076d3b0e5e95262bb1030f5ed5873382/corpus/navier-stokes) | Commit 47a01c2e076d3b0e5e95262bb1030f5ed5873382 | Initial-commit gap, head-commit correction and paper/Clay/Lean comparison |
| NS-08 | [SafeVerifyAgent Navier–Stokes audit](https://github.com/GasStationManager/SafeVerifyAgent/tree/main/audits/nse-deep) | Snapshot 2026-11-28 | Partial independent audit; coverage and unread proof mass recorded |
| NS-09 | [Vilin97 formalization benchmark](https://github.com/Vilin97/ns-formalization-benchmark) | README blob and upstream/provenance.json pinned in repository | Direct artifact reuse, source SHA-256 manifest and reproducible build comparison |
| NS-10 | [KTS Global Lean proof port](https://github.com/kts-global/lean-proofs-public) | Release s437-v1; [Zenodo record](https://doi.org/10.5281/zenodo.23535805) | Lean 4 port and R2/R3 verification package; not an independent mathematical proof |
| NS-11 | [Tengoku formal library](https://github.com/competemath/tengoku) | NOTICE and NavierStokesEuler/ComparatorSolution.lean | Downstream library integration with upstream attribution |
| NS-12 | [Buckmaster signed statement](https://cims.nyu.edu/~tristanb/statement.pdf) | 2026-09-08; four-page signed statement | Buckmaster’s account of the Alpöge collaboration, upstream Córdoba–Martínez-Zoroa programme, OpenAI discussions, and stated limits of his knowledge |

The OpenAI repository has two public commits and no public issues in the inspected snapshot. The first-to-second commit comparison reports 188 changed files, 19,388 additions and 79 deletions.

## D. AlphaProof Nexus / Erdős problems

| ID | Source | Version / locator | Evidence use |
|---|---|---|---|
| AP-01 | [Tsoukalas et al., Advancing mathematics research with AI-driven formal proof search](https://doi.org/10.1126/science.aej2213) | Science 394 (6820), 2026-10-08 | Peer-reviewed recognition, benchmark framing, author contributions and statement validation |
| AP-02 | [Pinned AlphaProof results archive](https://github.com/google-deepmind/alphaproof-nexus-results/tree/42f344cfa9d57154f36e6b9bef1f71760a438c54) | Commit 42f344cfa9d57154f36e6b9bef1f71760a438c54 | Nine Erdős formal proof files and other research outputs |
| AP-03 | [Formal Conjectures PR #3778](https://github.com/google-deepmind/formal-conjectures/pull/3778) | Upper-density variant of Erdős #741(i) | Localized status transition and agent attribution |
| AP-04 | [Formal Conjectures PR #4384](https://github.com/google-deepmind/formal-conjectures/pull/4384) | 53 commits, 135 comments | Human review, target correction and integration |
| AP-05 | [Carlos Toledo independent audit](https://carlostoledo.co/reports/alphaproof-nexus.html) | 2026 | Ten proof items replayed through two kernels; semantic correspondence treated separately |
| AP-06 | [Krenn et al., Monochromatic quantum graphs and photonic GHZ states](https://arxiv.org/abs/2611.26300) | arXiv:2611.26300v1, 2026-11-19 | Human-digested quantum-optics result discovered by AlphaProof Nexus |
| AP-07 | [Formal Conjectures proof commit](https://github.com/google-deepmind/formal-conjectures/commit/af88acbf9da0f26e3e934743a819e986e02f6875) | Commit af88acbf9da0f26e3e934743a819e986e02f6875 | Actual Lean proof for the even-N, D=N monochromatic-quantum-graph theorem |
| AP-08 | [Rishi Rajasekaran Krenn-conjecture proof](https://github.com/rrajasek95/krenn-conjecture/tree/56f495ae11cf4729e6173477cb25afff7342c8cf) | Commit 56f495ae11cf4729e6173477cb25afff7342c8cf | Separate GPT/Claude-assisted all-orders proof; no human expert review recorded |
| AP-09 | [Formal Conjectures PR #6627](https://github.com/google-deepmind/formal-conjectures/pull/6627) and [PR #8283](https://github.com/google-deepmind/formal-conjectures/pull/8283) | PR #6627 open; #8283 merged | External proof registration and narrower N=6 integration |
| AP-10 | [Palomar registry entry](https://palomar-registry.org/entry.html?id=PALOMAR-2026-11-27-000065) | PALOMAR-2026-11-27-000065 | External formal-verification record for the separate all-orders proof |
| AP-11 | [Reiher, Rödl & Sales, “Colouring versus density in integers and Hales–Jewett cubes”](https://doi.org/10.1112/jlms.12987) | *Journal of the London Mathematical Society* 110(5), e12987; first published 2024-10-10; Theorems 1.5 and 1.7 | Prior published result implying the negative answer to Erdős #846 under the collinear-triple specialization |
| AP-12 | [Erdős Problems #846](https://www.erdosproblems.com/846) | Page checked 2026-11-28 | Catalogue record for the planar problem; notes Rödl’s observation that RRS24 implies a counterexample after suitable projection |
| AP-13 | [Hedegreen, “Nine Became Eight”](https://hedegreenresearch.com/articles/nine-became-eight/) | 2026-07-21, version 1.0 | External row-level novelty audit; retains eight newly resolved results and reclassifies #846 while explicitly limiting its mathematical review |

The nine Erdős proof files are pinned in AP-02. Their individual blob SHAs are recorded in the evidence ledger. The list contains nine formal statements but only seven unique problem numbers; it includes parts and variants, and the #26 item is a Tenenbaum variant rather than an original Erdős problem.

## E. Liquid Tensor Experiment

| ID | Source | Version / locator | Evidence use |
|---|---|---|---|
| LTE-01 | [Scholze original challenge](https://xenaproject.wordpress.com/2020/12/05/liquid-tensor-experiment/) | 2020-12-05 | Original motivation |
| LTE-02 | [Scholze progress account](https://xenaproject.wordpress.com/2021/06/05/half-a-year-of-the-liquid-tensor-experiment-amazing-developments/) | 2021-06-05 | Participant account of human/machine collaboration |
| LTE-03 | [Commelin project update](https://leanprover-community.github.io/blog/posts/lte-update/) | 2021 | Project organization and progress |
| LTE-04 | [Mathlib completion announcement](https://leanprover-community.github.io/blog/posts/lte-final/) | 2022 | Community recognition and contributors |
| LTE-05 | [Lean Liquid repository](https://github.com/leanprover-community/lean-liquid) | Lean 3.48; Mathlib3 revision 5947fb69cc1fdfebaba1e1b1f0a04f26f0f612bf | Formal definitions, proofs, examples and project structure |
| LTE-06 | [LTE Blueprint](https://leanprover-community.github.io/liquid/) | Public project blueprint | Natural-language/formal dependency map |
| LTE-07 | [Topaz, Definitions in the Liquid Tensor Experiment](https://leanprover-community.github.io/blog/posts/lte-examples/) | 2022 | Semantic sanity-check examples |
| LTE-08 | [Commelin & Topaz, Abstraction boundaries and spec-driven development in pure mathematics](https://doi.org/10.1090/bull/1831) | Bulletin of the AMS, 2024 | Scholarly analysis of the experiment's methodological contribution |
| LTE-09 | [Formalizing Carleson's Theorem in Lean](https://arxiv.org/abs/2609.31334) | arXiv:2609.31334v1, 2026 | Explicitly traces definition-sanity-check strategy to LTE and uses a Blueprint |
| LTE-10 | [Mathlib4 Condensed.Basic](https://github.com/leanprover-community/mathlib4/blob/master/Mathlib/Condensed/Basic.lean) | Current Mathlib4 source | Related condensed-mathematics formalization; not a direct port of LTE's Lean3 proof |
| LTE-11 | [Atlas Lean condensed topological rings](https://github.com/facebookresearch/atlas-lean/blob/4eb2a94dcb1e933e6bf0a7a8ba5da6771d62c343/MathlibExt/Condensed/TopologicalRings.lean) | Commit 4eb2a94dcb1e933e6bf0a7a8ba5da6771d62c343 | Downstream use of Mathlib4 condensed infrastructure, not LTE proof code |

## F. Methodological and theoretical antecedents

| Source | Relevance | Novelty boundary |
|---|---|---|
| De Millo, Lipton & Perlis (1979), [Social Processes and Proofs](https://doi.org/10.1145/359104.359106) | Social assimilation of proofs | Do not claim that proof acceptance is purely formal or that social processes are new |
| MacKenzie (2001), *Mechanizing Proof* | Historical sociology of mechanized proof | Prior account of proof assistants, trust and institutional practice |
| Rosental (2003), [Certifying Knowledge](https://doi.org/10.1177/000312240306800407) | Ethnography of theorem certification | Prior empirical study of recognition and proof certification |
| Hardwig (1985), [Epistemic Dependence](https://www.jstor.org/stable/2026523) | Rational reliance on expert testimony | Distinguish justified dependence from ideological disavowal |
| Druskat (2019), [Software and Dependencies in Research Citation Graphs](https://doi.org/10.1109/mcse.2019.2952840) | Software dependencies, credit and citation graphs | Do not claim novelty for dependency graphs or transitive software credit |
| Smith et al. (2016), [Software Citation Principles](https://doi.org/10.7717/peerj-cs.86) | Attribution, persistence, specificity and accessibility | Use as a provenance/citation standard |
| Desrochers et al. (2018), [Symbolic capital in the reward system of science](https://doi.org/10.1177/0539018417752089) | Bourdieu/Merton, authorship, citations and visibility | Prior account of symbolic capital and scientific recognition |
| Tahamtan & Bornmann (2022), [Social Systems Citation Theory](https://doi.org/10.3145/epi.2022.jul.11) | Citation as recognition and persuasion | Do not equate citation with substantive reuse |
| Kallel & El Louadi (2026), [Verification abundance, adjudication scarcity](https://arxiv.org/abs/2608.28997) | Derivational validity, representational fidelity and epistemic significance | Direct novelty constraint; do not claim the three-layer distinction as new |
| López-Corona (2026), [From Authorial Mathematics to Studio Mathematics](https://arxiv.org/abs/2608.22194) | Studio mathematics, provenance, understanding audit and contribution-authority trace | Direct novelty constraint; do not claim distributed authorship, provenance or LTE collaboration as new |

## Search boundary

The Stage 3 manuscript update adds RH-11–RH-13, NS-12 and AP-11–AP-13. These sources were checked directly for the Claude collaboration, CMI status and prize rules, Buckmaster’s attribution account, and the #846 novelty reclassification.

Searches covered:
- Exact titles, DOI and arXiv records for the four cases and their named follow-up projects.
- GitHub code/repository search for exact project names, theorem filenames and imports.
- Public PRs, commit histories, status registers, audit reports and repository source manifests.
- CoChat scholarly search for downstream citations, formal proof reuse, software dependencies, mathematical theorem use and methodological uptake.

Negative findings mean “not located within this search boundary as of 2026-11-28”, not “does not exist”. Stars, views, downloads and generic imports are not coded as mathematical reuse. No representative public-opinion survey or interview claim is made.
