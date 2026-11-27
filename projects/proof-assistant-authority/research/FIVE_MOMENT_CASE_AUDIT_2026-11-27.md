# Five-moment case audit: evidence and argument assessment

**Project:** *In Lean We Trust?*  
**Evidence cut-off:** 27 November 2026  
**Scope:** The four existing Lean cases only.

## Executive finding

The public record strongly supports the first three moments: real technical checking, distributed epistemic labour, and credential condensation. The fourth moment varies and cannot be inferred from concise communication alone. The fifth is a conditional feedback mechanism, not a necessary stage of every case.

**AlphaProof Nexus provides the positive existence case for the fifth moment at the level of public institutional representation.** The *Science* paper reports that experts validated whether the Lean statements captured the original Erdős conjectures. Its author-contribution statement also identifies human roles in selecting problems, validating generated solutions, and writing natural-language proofs. Aarhus University's institutional report likewise identifies the co-author's human role in problem selection, solution validation, and exposition. Yet the same research and institutional communication chain retains the formulation that the agent “autonomously resolved” the problems. Human mediation is explicitly acknowledged, while the machine remains the grammatical and public subject of the achievement.

The narrow operational meaning of autonomy—proof search and proof generation after a formal target is supplied—is real. The public formulation nevertheless allows this operational autonomy to stand for the resolution of the mathematical problems as a whole. This is the relevant symbolic displacement: human work is acknowledged, but the achievement is publicly attributed to the autonomous machine. The case supports a public-discourse diagnosis, not a claim about the authors' private motives.

Riemann shows powerful institutional certification with its warrant network explicitly described. Navier–Stokes associates a Lean formalization with a public solution claim, but the external critique concerns proof-route correspondence and is not acknowledged by the same institutional chain in the public record reviewed. Liquid Tensor explicitly acknowledges semantic risks and answers them through sanity checks. These three cases clarify the contrast conditions; they do not need to reproduce the positive case.

## 1. Evidence standard for fetishistic disavowal

A public case supports the fifth moment when the following elements occur within a traceable publication or institutional communication chain:

1. **Acknowledged mediation:** the source explicitly identifies human, semantic, or technical work that qualifies the machine's contribution—for example, problem selection, statement validation, interpretation, or natural-language exposition.
2. **Continued autonomous representation:** the same chain continues to describe the machine as having autonomously resolved the mathematical problem, or otherwise presents it as the apparent bearer of the whole achievement.
3. **Available wider reading:** the public formulation can reasonably be read as attributing the overall mathematical achievement to the autonomous machine, rather than being clearly restricted to proof search or proof-term generation.
4. **Public-authority function:** the formulation serves as the portable description through which the achievement is announced, recognized, or institutionally communicated.

This is a Žižekian analysis of public practice and attribution. It does not require proof of private motives, conscious deception, or an explicit admission that the wording overstates the technical warrant. It asks whether acknowledged mediation and continued investment in autonomous machine authority coexist in the same public communication chain.

The key distinction is:

\[
\text{knowledge of human/semantic mediation}
\neq
\text{dissolution of symbolic investment in machine autonomy}.
\]

A narrow operational claim that an agent autonomously searches for and generates a proof can be true. The ideological question arises when this narrow truth becomes the public sign of the whole mathematical achievement, while the human and semantic work that qualifies it remains acknowledged.

## 2. Riemann hypothesis

- **M1:** The Lean FRO/Mathlib statement reports successful compilation, exact statement comparison, and acceptance by Lean’s kernel and independent checkers. Sutherland records 175,187 compiling modules and independent replay.
- **M2:** The same statement identifies expert vetting of the Mathlib theorem, community work, and independent checker implementations.
- **M3:** “Lean verification of the Riemann Hypothesis,” “full confidence,” and the certification of statement and proof make the result a portable institutional credential.
- **M4:** The credential has considerable institutional force, but the statement lists the distinct grounds of its authority. The network remains visible.
- **M5:** Not established. The certifying institutions explicitly report expert vetting and independent comparison of the semantic statement. Emmerson’s later challenge is external to the certifying chain and cannot be imputed to those institutions.

**Assessment:** composite institutional authorization, not demonstrated fetishistic disavowal.

Sources: https://leanprover-community.github.io/blog/posts/riemann-hypothesis/ ; https://math.mit.edu/~drew/grh/ ; https://doi.org/10.20944/preprints202611.2463.v1

## 3. Navier–Stokes

- **M1:** OpenAI’s public repository contains Lean formalizations of its Navier–Stokes and Euler results. An independent formal-statement audit reports a successful build and details the relation between alternatives C/D and Theorem 1.1.
- **M2:** OpenAI describes approximately 10,000 concurrent agents, Codex-mediated consolidation, a mathematical write-up, and a separate Lean formalization and verification phase.
- **M3:** The public announcement presents a solution to a Millennium Prize problem alongside a Lean formalization; the repository describes the artifacts as Lean certificates accompanying the results.
- **M4:** Bastounis, Circelli, and Hansen identify discrepancies between parts of the natural-language proof and the Lean proof route. These concern proof correspondence, not necessarily theorem-statement fidelity. The formal alternatives C/D are copied from the Clay formulation, and a formal bridge connects Theorem 1.1 to them. OpenAI’s announcement does not explicitly claim that Lean alone verifies every step of the prose.
- **M5:** Not established. The public record reviewed does not show OpenAI acknowledging the specific proof-correspondence critique and then continuing to use Lean as a guarantee that the written proof itself was checked.

**Assessment:** credential association and possible scope ambiguity; no actor-level evidence of disavowal.

Sources: https://openai.com/index/navier-stokes-solution/ ; https://github.com/openai/NavierStokesAndEuler ; https://arxiv.org/abs/2610.08144 ; https://navier.microprediction.org/formal.html

**Important distinction:** theorem-statement fidelity is different from proof-route correspondence. A Lean proof may establish the same theorem through a different proof route; that does not mean it faithfully formalizes the argument in the accompanying paper. Conversely, a proof-route discrepancy does not by itself show the theorem is false or the kernel check invalid.

## 4. Erdős problems and AlphaProof Nexus

- **M1 — real technical reliability:** the system generates formal proof terms and Lean checks them. The *Science* paper reports that the agent autonomously resolved 9 of 353 open Erdős problems; the evaluation set consists of formalized statements in the Formal Conjectures repository.
- **M2 — distributed epistemic labour:** Section 3 states that after each Erdős solve, experts validated that the Lean statement faithfully captured the original conjecture. The author-contribution statement records human roles in selecting problems, validating generated solutions, and writing natural-language proofs. Aarhus University's report identifies Gergely Bérczi's role in identifying suitable problems, validating the system's solutions, and co-writing the natural-language versions.
- **M3 — credential condensation:** the *Science* abstract states that the agent “autonomously resolved 9 of 353 open Erdős problems”; Table 1 repeats “autonomously resolved” in its description of the results. Aarhus University's headline and opening paragraph repeat the autonomous-resolution formulation.
- **M4 — objectal displacement:** the grammatical subject of “autonomously resolved” is the agent, and the object is the open mathematical problem. Human roles are acknowledged but represented as selecting, validating, and explaining around the machine's central act of resolution. The machine is thereby made the apparent bearer of the problem-level achievement.
- **M5 — fetishistic disavowal:** **positive existence case in public institutional representation.** The same research and institutional communication chain acknowledges human problem selection, statement validation, and mathematical exposition while retaining the machine as the autonomous subject of the achievement. The public attribution does not conceal mediation; it subordinates acknowledged mediation to the machine's headline act.

### S–O–E assessment

- **S — Agency-attribution extension (S_a):** autonomy in proof search is attributed as autonomy in resolving the mathematical problem itself. The shift is visible in the contrast between the paper's technical account of formal proof search and its abstract/Table 1 formulation “autonomously resolved open problems.” This is not a claim that the theorem is invalid or that the expert-validated formal statement lacks warrant.
- **O — Objectal displacement:** the agent is the grammatical and symbolic bearer of “resolution,” while human work is acknowledged but positioned as selection, validation, and exposition around the machine's central achievement.
- **E — Social efficacy:** the formulation appears in the *Science* abstract and Table 1 and in Aarhus University's official headline and opening account. These are high-visibility research and institutional forms through which the achievement is announced and recognized. This establishes a public-authority function, not a causal claim about audience belief.

### Assessment

The case turns on a precise linguistic and institutional shift. The technical operation is autonomous proof search over formalized targets, with Lean checking the resulting proof terms and experts validating that the formal statements correspond to the original conjectures. The public description, however, makes the agent the subject of the verb “resolved” and makes open mathematical problems its object. The institutional report repeats this formulation while explicitly identifying the mathematician's role in problem selection, solution validation, and natural-language exposition. Thus, the autonomous agent is not merely credited with generating proofs; it is publicly named as the solver of the mathematical problems, while the human contribution is placed in a supporting and validating position.

The narrow operational reading of “autonomous” remains true. The ideological effect lies in the public attribution of the whole achievement to the machine, not in a denial that the proof search was autonomous. This is a positive instance of fetishistic disavowal as a structure of public representation, not an inference about private motives. It establishes the existential claim without implying that all formalization projects exhibit the same structure.

The provenance audit of #26, #741(i), #741(ii), and #125 concerns the identity and traceability of particular formal files. It is not evidence of kernel failure or, by itself, part of the fifth-moment argument.

Primary sources:
- Tsoukalas et al., *Science* (2026), Abstract, Table 1, §3, and Author Contributions: https://doi.org/10.1126/science.aej2213
- Aarhus University institutional report: https://math.au.dk/en/currently/news/news-item/artikel/gergely-deepmind
- arXiv version: https://arxiv.org/abs/2605.22763
- Erdős Problems research library: https://erdosproblems.ai/wiki/library/additive_combinatorics/tsoukalas_2026_advancing_mathematics_research_ai_driven_formal_proof_search

## 5. Liquid Tensor Experiment

- **M1:** The project formally verifies the main theorem of liquid vector spaces in Lean.
- **M2:** The completion announcement lists mathematical, formalization, technical, library, and institutional contributors and identifies Scholze’s mathematical support.
- **M3:** The public announcement states that the main theorem has been formally verified and the experiment completed.
- **M4:** Topaz explicitly asks how mathematicians can know Lean definitions are correct, identifies the possibility of pathological definitions, and describes the examples folder of semantic sanity checks.
- **M5:** Not established. The participants acknowledge a semantic risk and respond with additional scrutiny. Continued confidence follows the added checks; it is not an overextended guarantee maintained while leaving the acknowledged gap unaddressed.

**Assessment:** counter-practice in which semantic mediation remains visible and supports confidence.

Sources: https://leanprover-community.github.io/blog/posts/lte-final/ ; https://leanprover-community.github.io/blog/posts/lte-examples/ ; https://xenaproject.wordpress.com/2021/06/05/half-a-year-of-the-liquid-tensor-experiment-amazing-developments/

## 6. Comparative result

| Case | M1 reliability | M2 distributed labour | M3 condensation | M4 displacement | M5 disavowal |
|---|---|---|---|---|---|
| Riemann | Strong | Strong and visible | Strong | Limited / not established | Not established |
| Navier–Stokes | Strong formal check | Strong | Strong | Ambiguous association | Not established |
| AlphaProof Nexus | Strong formal check | Explicit human validation | Strong autonomy framing | Supported at public-discourse level | Affirmative existence case |
| Liquid Tensor | Strong formal check | Highly visible | Present | Counter-practice | Not established |

The model should therefore distinguish:
- enabling conditions (technical reliability and distributed labour);
- communicative transformation (credential condensation);
- fetishistic conversion (objectal displacement);
- conditional reproduction (fetishistic disavowal after acknowledged overreach).

The four cases provide one affirmative existence case for the fifth moment: AlphaProof Nexus. The evidence is strongest at the level of public institutional representation, where the same communication chain acknowledges human validation and retains the autonomous-machine framing. Riemann and Navier–Stokes clarify different configurations, while Liquid Tensor provides a counter-practice. The claim is existential, not a claim about prevalence across all formalization projects.

## 7. Consequences for the manuscript

1. Distinguish formation from reproduction.
2. Distinguish operational proof-search autonomy from symbolic autonomy in the public attribution of the whole mathematical achievement.
3. Treat AlphaProof as the positive existence case for public-discourse fetishistic disavowal.
4. Distinguish theorem-statement fidelity from proof-route correspondence in Navier–Stokes.
5. Present Riemann as composite institutional certification and Liquid Tensor as a transparent semantic counter-practice.
6. Preserve the central philosophical claim that genuine technical reliability can support symbolic authority without claiming that every Lean practice exhibits fetishistic disavowal.
