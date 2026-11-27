# Lean-centered case-study audit

**Project:** *In Lean We Trust? The Ideology of Machine-Checked Proofs in Science*  
**Evidence cut-off:** 27 November 2026  
**Primary empirical scope:** Lean  
**Status:** source-based comparative audit; not an independent rebuild or mathematical referee report.

## 1. Purpose and common audit template

The four cases are not ranked by a single AI-capability or trustworthiness score. Each is examined through the same questions:
1. What exact mathematical proposition is stated?
2. What did AI contribute, and what did humans contribute?
3. What exactly does Lean check?
4. Which axioms, libraries, dependencies, build settings, and source versions are involved?
5. Is the Lean statement semantically faithful to the intended theorem and accompanying natural-language text?
6. Who independently checked the formal artifact?
7. What human mathematical understanding, peer review, and institutional recognition exist?
8. How do project authors, institutions, media, and public audiences represent the result?

This audit distinguishes **kernel validity**, **statement identity**, **source-text correspondence**, **mathematical understanding**, and **social acceptance**. They are separate claims.

## 2. Case A — Riemann hypothesis: Claude-assisted Lean development

### 2.1 Primary claim and formal target

On 20 November 2026, Levent Alpöge published a four-page note saying: “I believe I have, working with Claude, discovered a proof of the Riemann Hypothesis.” He released the result as a Lean 4 development, not as a conventional mathematical paper. The archive contains 175,187 modules and about 17.4 million lines. The five headline theorems concern the Riemann hypothesis and the generalized Riemann hypothesis for Dirichlet L-functions.

Primary sources:
- Alpöge's note: https://alpo.ge/
- Lean FRO/Mathlib community statement: https://leanprover-community.github.io/blog/posts/riemann-hypothesis/
- Waterloo verification and exposition page: https://www.math.uwaterloo.ca/~mrubinst/alpoge_claude_grh/
- MIT verification materials: https://math.mit.edu/~asutherland/
- Compact proof repository: https://github.com/lsernau/grh-lean
- Public reading guide: https://nasqret.github.io/riemann-rev/summary/grh-condensed-summary.pdf

### 2.2 Formal verification status

Waterloo's record reports that the original archive compiles in full, the five headline theorems use only Lean's three standard axioms (propext, Classical.choice, Quot.sound), every module was replayed through Lean's kernel, and the independent kernel nanoda checked 1,484,729 dependent declarations without typechecker errors. The Mathlib statement comparison was also reported successful.

A shorter rewrite was released on 25 November by Luke Sernau and collaborators. Waterloo's 26 November report says its compact edition has 794 modules; all compile; the five theorem statements are unchanged; the standard three axioms are the only ones used; all modules pass kernel replay; and lake comparator --paranoid accepts the five challenge statements using six kernels/checkers. The report notes that the Waterloo cluster did not support Comparator's sandbox, while Andrew Sutherland's sandboxed runs reached the same verdict.

These are strong machine-level verification results. They support the claim that the formal proof terms establish the specified Lean propositions in the stated formal environment.

### 2.3 Human understanding and recognition

The Waterloo working guide (version 2, 22 November, 265 pages) explicitly says it does not yet prove the central inequality (M) in classical terms; it reduces RH to thirteen numbered hypotheses and lists remaining work. The 26 November RIEMANN-REV note states that no mathematician has read the proof through and that no conventional mathematical paper accompanies the formal archive. This is not evidence that the proof is false. It is evidence that machine-level certification and human mathematical understanding are distinct.

The Clay Mathematics Institute's recognition and prize process are separate from Lean kernel acceptance. News coverage reports that the Clay Institute still lists the problem as open pending rigorous mathematical assessment and general acceptance.

### 2.4 Public framing

The public narrative includes “AI solves the Riemann hypothesis,” “historic breakthrough,” and “proof checked by Lean.” More careful reporting distinguishes the author's claim, the Lean proof's formal validity, statement identity, and the absence of a human-readable argument. The Associated Press reports that Rutgers mathematician Alex Kontorovich found the machine verification encouraging but had not independently understood the proof; the Clay Institute president emphasized the need for rigorous assessment and broader mathematical understanding.

### 2.5 Provisional philosophical interpretation

- **Fantasy:** the formal checker may become a visible symbol of certainty around a historically unresolved problem.
- **Fetishism:** some compressed narratives may attribute the achievement to “Claude + Lean” while obscuring the mathematician's direction, formalization work, Mathlib infrastructure, checker authors, and independent review.
- **Counter-evidence:** the multiple independent checker results are real technical achievements; Waterloo's detailed documentation and expert commentary make the human and institutional mediation visible.
- **Cynical ideology:** not established. The public materials include explicit qualifications; no evidence shows that relevant actors knowingly maintain a stronger claim in practice despite those qualifications.

**Best use in the paper:** distinguish strong proof-term checking from human understanding and social acceptance. The case demonstrates that technical certainty can be very high at the formal level while explanatory and institutional processes remain incomplete.

## 3. Case B — Navier–Stokes: OpenAI discovery and Lean formalization

### 3.1 Primary claim

OpenAI's 8 September 2026 announcement states that an internal system produced an analytical proof and a Lean formalization of finite-time singularity for three-dimensional incompressible Navier–Stokes with smooth forcing, and claims this establishes Clay alternatives C and D. OpenAI says the discovery used an internal model more capable than GPT-6 Astra; the model used for discovery must not be conflated with the separate formalization process.

Primary sources:
- OpenAI announcement: https://openai.com/index/navier-stokes-solution/
- Paper: linked from the announcement
- Lean repository: https://github.com/openai/NavierStokesAndEuler
- Independent critique: https://arxiv.org/abs/2610.08144
- King's College London summary: https://www.kcl.ac.uk/news/openais-navier-stokes-proof-called-into-question

### 3.2 What Lean checks and the correspondence dispute

The OpenAI repository publishes Lean formalization and configuration metadata. The critical issue is not whether Lean's kernel can accept a proof of its formal declarations; it is whether those declarations and proofs faithfully correspond to the separate natural-language paper and its claimed theorem.

Bastounis, Circelli, and Hansen (arXiv:2610.08144, 6 October 2026) report discrepancies between the paper and Lean formalization, including an inverse estimate in Lemma 8.6 using m+4 input derivatives in the written proof but m+5 in the corresponding Lean estimate, as well as a difference in the pressure-flux estimate/proof route. Their stated conclusion is that the formalized Lean proof does not correspond to the natural-language proof; they do not establish that either proof is false.

King's College London's 27 October summary similarly states that the mismatch does not prove OpenAI's result wrong, but that verifying the formal version alone cannot establish that the original written proof was correctly represented.

The math.observer record, last reviewed 25 November, reports that OpenAI's Lean proof is accepted by 29 of 37 checkers on Lean Kernel Arena, including Lean's official kernel, while the written proof remains disputed as not matching it. This is a secondary status tracker, not a substitute for checking the repository and exact commit.

### 3.3 Public framing and philosophical interpretation

OpenAI's announcement uses the language of “sharing a solution” to a Millennium Prize Problem. Later independent criticism reframes the issue as a translation/correspondence problem. This sequence provides unusually direct evidence of how the meaning of “Lean-verified” can change when the formal object is compared with the source text.

- **Fantasy:** the label “Lean-verified solution” can be received as a guarantee of the complete published result.
- **Fetishism:** the kernel's genuine authority over formal declarations can stand in for the semantic relation between those declarations and the written proof.
- **Counter-evidence:** OpenAI published both the proof and Lean repository; the critique and OpenAI response are public; the mismatch is debated rather than hidden.
- **Cynical ideology:** not established. The available public record does not justify attributing deliberate disavowal or bad faith.

**Best use in the paper:** the clearest case for the distinction between formal correctness and semantic correspondence. Do not describe the mismatch as a Lean kernel failure or as a refutation of the Navier–Stokes result.

## 4. Case C — Erdős problems: AlphaProof Nexus

### 4.1 Primary claim and method

Tsoukalas et al., “Advancing Mathematics Research with AI-Driven Formal Proof Search,” Science 394 (6820) (8 October 2026), DOI: https://doi.org/10.1126/science.aej2213; preprint https://arxiv.org/abs/2605.22763.

The system reports 9 solved problems among 353 open Erdős problems represented in a formal conjecture repository and 44 proofs among 492 OEIS conjectures attempted. The denominator is the formalized benchmark available to the project, not all open Erdős problems.

The system alternates LLM-generated proof attempts with Lean checking. The paper describes human validation of the correspondence between the nine Lean statements and the intended Erdős conjectures; it also reports manual review of OEIS formalizations.

### 4.2 Independent commentary and audit

The Science Media Centre Spain collected expert reactions on 8 October 2026. The comments differ: some emphasize the research potential; others question the added value/cost of the more elaborate agent, the fidelity of formal statements to intended problems, and the danger of producing certified results that are not fully understood.

Carlos Toledo's secondary audit reports that published Lean proofs replay under two kernels but raises questions about novelty and statement interpretation for some OEIS and Erdős results. The audit itself limits its conclusions: some interpretations are AI-generated and not specialist-confirmed, and it does not settle whether every formal Erdős statement matches the original historical problem.

### 4.3 Philosophical interpretation

- **Fantasy:** “AI solves Erdős problems” can symbolize autonomous mathematical discovery.
- **Fetishism:** less clearly supported, because the Science paper describes the formal benchmark, Lean verification, and human validation.
- **Counter-evidence:** explicit denominators and human statement checks make the mediation more visible than in a simple “AI solved mathematics” headline.
- **Cynical ideology:** not established.

**Best use in the paper:** a scope-aware counter-case showing that Lean can be integrated into a transparent human-AI research workflow without automatically producing epistemic fetishism.

## 5. Case D — Liquid Tensor Experiment

### 5.1 Exact theorem and Lean result

The Lean community announced completion on 15 July 2022, stating that the main theorem of liquid vector spaces had been formally verified on 14 July. The theorem concerns vanishing of higher Ext groups for specified condensed real vector spaces:

\[
\\operatorname{Ext}^{i}(\\mathcal{M}_{p'}(S),V)=0
\\quad\\text{for all }i\\geq 1.
\]

The community post gives the corresponding Lean theorem statement and identifies contributors, including Johan Commelin, Peter Scholze, Adam Topaz, and many other Lean community members. It explicitly credits mathematical support, homological algebra and condensed mathematics contributions, Mathlib dependencies, and institutional support.

Primary sources:
- Lean completion announcement: https://leanprover-community.github.io/blog/posts/lte-final/
- Lean repository: https://github.com/leanprover-community/lean-liquid
- Quanta coverage (2021): https://www.quantamagazine.org/lean-computer-program-confirms-peter-scholze-proof-20210728/
- Scholze's 2021 contemporaneous account: https://xenaproject.wordpress.com/2021/06/05/half-a-year-of-the-liquid-tensor-experiment-amazing-developments/

### 5.2 Human-machine authority

Scholze's June 2021 post states that the challenge was not yet complete, but the key Theorem 9.4 had been formalized. In a contemporaneous comment, he emphasized that his confidence came from human mathematical interaction and scrutiny, not from the computer alone. The final 2022 announcement openly lists the many contributors and support structures.

### 5.3 Philosophical interpretation

- **Fantasy:** possible in media framing that says Lean “confirms” a proof.
- **Fetishism:** weakly supported by the primary institutional record, which makes collective human labour visible.
- **Counter-evidence:** the primary announcement is unusually transparent about people, mathematical contributions, software library, and institutional support.
- **Cynical ideology:** not established.

**Best use in the paper:** historical counter-case. It shows how Lean authority can be embedded in a visible collective process rather than represented as autonomous machine authority.

## 6. Cross-case findings

| Case | Lean role | Semantic bridge | Human mediation | Best analytical use |
|---|---|---|---|---|
| Riemann | Extensive proof checking; multiple independent checkers | Mathlib statement matching reported | Mathematical explanation and broad review remain incomplete | Formal certainty vs understanding |
| Navier–Stokes | Proofs of published formal declarations | Disputed correspondence with natural-language paper | Independent mathematical critique and institutional response | Kernel validity vs source-text fidelity |
| Erdős | Automated proof search with Lean verification | Human statement validation reported; secondary audit adds questions | Experts and Science publication | Transparent mediated authority |
| Liquid Tensor | Formal verification of a specified theorem | Theorem tied to Scholze/Clausen mathematical statement | Extensive visible human collaboration | Collective labour vs machine fetishism |

## 7. Provisional theoretical result

The evidence does not support the thesis that Lean is inherently fetishized or that society blindly trusts machines. Rather:

**Lean can function as a public credential of mathematical reliability, but the social meaning of that credential depends on how the formal statement, source claim, human labour, and institutional review are connected and communicated.**

The strongest case for an ideological-fetishism analysis is Navier–Stokes, because a formal proof's authority can be made to stand in for semantic correspondence that is separately disputed. Riemann shows that extensive formal certification can coexist with incomplete human understanding. Erdős and Liquid Tensor provide counter-cases in which human mediation and scope are more visible.

No case yet establishes cynical ideology in the strict sense. The public record supports analysis of representations and institutional practices, not unconscious motives.

## 8. Remaining audit items

1. Pin and archive exact Lean commits and theorem declaration locators for Riemann, Navier–Stokes, Erdős, and Liquid Tensor.
2. For Navier–Stokes, compare cited estimates directly against pinned written-paper equations and Lean declarations; do not rely solely on summaries.
3. For Erdős, choose two representative Lean theorems and compare the original conjecture, Formal Conjectures statement, generated proof, and independent audit.
4. For Riemann, keep the 26 November compact proof verification distinct from the original 17-million-line archive and from human mathematical exposition.
5. For Liquid Tensor, pair the primary Lean community announcement with Quanta's article and Scholze's contemporaneous statements, respecting their dates.

These are bounded case-audit tasks, not reasons to expand the sample.