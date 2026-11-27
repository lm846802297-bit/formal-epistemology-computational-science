# Five-moment evidence audit: the four Lean cases

**Project:** *In Lean We Trust?*  
**Evidence cut-off:** 27 November 2026  
**Scope:** Four existing Lean cases only. No new cases added.  
**Purpose:** Test the five-moment model against public primary materials, with particular attention to fetishistic disavowal.

## Executive finding

The public record strongly supports the first three moments across the cases: real technical checking, distributed epistemic labour, and credential condensation. The fourth moment varies and cannot be inferred from concise communication alone. The fifth moment is a conditional feedback mechanism, not a necessary stage of every case.

**AlphaProof Nexus is the strongest borderline candidate for the fifth moment.** The same *Science* paper acknowledges the unreliability of LLM-generated natural-language proofs and reports that experts validated whether the Lean statements captured the original Erdős conjectures. It nevertheless describes the agent as having “autonomously resolved” nine problems and presents the results as evidence for autonomous mathematical discovery. This is direct co-presence of acknowledged mediation and autonomy language. It is not decisive evidence of fetishistic disavowal because “autonomous” may accurately refer to proof search and generation, with expert statement validation occurring after the solve.

No other case currently provides stronger public evidence of the fifth moment:
- Riemann: the certifying statement makes the semantic and technical components of the warrant visible.
- Navier–Stokes: OpenAI publishes both a write-up and a Lean formalization; an external critique identifies proof-route discrepancies, but the same institutional chain is not shown acknowledging the specific critique and continuing to use Lean as a guarantee of the written proof.
- Liquid Tensor: semantic risks are explicitly acknowledged and answered with sanity checks; continued confidence is grounded in additional scrutiny.

The empirical conclusion is not that the fifth moment is absent from all formal-verification practice. It is that the current four cases do not establish an unambiguous instance. The conceptual model remains useful because it distinguishes formation of the credential’s authority from its possible reproduction after awareness.

## 1. What counts as evidence for the fifth moment?

A public case must establish all of the following within the same actor or institutional communication chain:

1. **Specific boundary knowledge:** the actor acknowledges what Lean checked and what the credential does not establish by itself.
2. **Recognition of overreach:** the actor acknowledges that the credential is being used, or could be used, to warrant more than the check and its documented semantic bridge establish.
3. **Continued broader investment:** the actor nevertheless continues to mobilize the same credential as a broader guarantee or marker of mathematical closure.
4. **Practical or legitimating role:** the broader use has a recognizable role in institutional recognition, public authority, credibility allocation, or repeated practice.

Mere awareness that “AI can make mistakes” is not enough. Neither is knowledge that Lean checks a formal proposition. A participant may know the kernel’s exact function and rely on it rationally for that function. Likewise, if expert review establishes the relation between the formal proposition and the intended theorem, a broad claim may be warranted by the combined network.

The key distinction is therefore:

\[
\text{knowledge of technical scope} \neq \text{knowledge of overreach}.
\]

Fetishistic disavowal requires the latter together with continued investment beyond the acknowledged warrant.

## 2. Riemann hypothesis

### Evidence across the five moments

- **M1, real technical reliability:** the Lean FRO/Mathlib joint statement reports successful compilation, exact statement comparison, and acceptance by Lean’s kernel and independent checkers. Sutherland’s report records 175,187 compiling modules, independent kernel replay, and comparisons against the challenge statement.
- **M2, distributed epistemic labour:** the statement identifies expert vetting of the Mathlib theorem, Mathlib and Lean community work, independent checker implementations, and third-party resources. The later exposition is explicitly AI-mediated.
- **M3, credential condensation:** the title “Lean verification of the Riemann Hypothesis,” the phrase “full confidence,” and the statement that the community certifies both statement and proof make the result portable as an institutional credential.
- **M4, objectal displacement:** the credential carries substantial institutional authority, but the same statement lists the distinct grounds of that authority: statement vetting, compilation, exact comparison, and proof checking. The network remains visible.
- **M5, fetishistic disavowal:** not established. The certifying institutions explicitly address the semantic relation by reporting expert vetting and independent statement comparison. Emmerson’s later challenge is external to the certifying chain and cannot be imputed to the institutions.

### Assessment

This is a case of powerful institutional authorization through a composite warrant, not a clear case in which the machine credential is knowingly used beyond its established scope. “Full confidence” is grounded in multiple stated checks rather than attributed to the kernel alone.

Primary sources:
- https://leanprover-community.github.io/blog/posts/riemann-hypothesis/
- https://math.mit.edu/~drew/grh/
- https://doi.org/10.20944/preprints202611.2463.v1

## 3. Navier–Stokes

### Evidence across the five moments

- **M1, real technical reliability:** the public repository contains Lean formalizations of the Navier–Stokes and Euler results. An independent formal-statement audit reports a successful build and details the relation between the formal alternatives C/D and the paper’s Theorem 1.1.
- **M2, distributed epistemic labour:** OpenAI describes approximately 10,000 concurrent agents, Codex-mediated consolidation, a mathematical write-up, and a separate Lean formalization and verification phase.
- **M3, credential condensation:** the public announcement presents a “solution” to a Millennium Prize problem, says that both a write-up and a Lean formalization are being shared, and links directly to the formal artifact. The repository describes its artifacts as “Lean certificates accompanying” the results.
- **M4, objectal displacement:** Bastounis, Circelli, and Hansen identify discrepancies between parts of the natural-language proof and the Lean proof route. These concern proof correspondence, not necessarily theorem-statement fidelity. A separate audit reports that the formal alternatives C/D are copied from the Clay formulation and that Theorem 1.1 is formally bridged to them. The announcement does not explicitly claim that Lean alone verifies every step of the prose.
- **M5, fetishistic disavowal:** not established. The public record reviewed here does not show OpenAI acknowledging the specific proof-correspondence critique and then continuing to use the Lean credential as a guarantee that the written proof itself was checked.

### Assessment

This case should not be described simply as a mismatch between the formal theorem and the intended theorem. The crucial distinction is between **theorem-statement fidelity** and **proof-route correspondence**. A Lean proof may establish the same theorem through a different proof route; that does not mean it faithfully formalizes the argument in the accompanying paper. Conversely, a proof-route discrepancy does not by itself show the theorem is false or the kernel check invalid.

The case is important for analyzing how a Lean certificate is associated with a public solution claim, but it does not currently support a fifth-moment diagnosis.

Primary sources:
- https://openai.com/index/navier-stokes-solution/
- https://github.com/openai/NavierStokesAndEuler
- https://arxiv.org/abs/2610.08144
- https://navier.microprediction.org/formal.html

## 4. Erdős problems and AlphaProof Nexus

### Evidence across the five moments

- **M1, real technical reliability:** the agent generates formal proof terms and Lean checks them. The *Science* abstract reports nine successes among 353 open Erdős problems; the denominator refers to formalized statements in the Formal Conjectures repository.
- **M2, distributed epistemic labour:** after each solve, experts validated that the Lean statement faithfully captured the original conjecture. The author-contribution statement records human roles in problem selection, validation of generated solutions, and writing natural-language proofs. Aarhus University's report identifies Bérczi's role in selecting suitable problems, validating solutions, and co-writing natural-language proofs.
- **M3, credential condensation:** the *Science* abstract and Table 1 describe the agent as having “autonomously resolved” the problems; Aarhus University's headline and opening account repeat this formulation.
- **M4, objectal displacement:** the agent is the grammatical subject of “resolved,” and the open mathematical problem is its object. Human labour is acknowledged but positioned as selecting, validating, and explaining around the machine's central act.
- **M5, fetishistic disavowal: affirmative public-discourse case.** The same research and institutional communication chain acknowledges human and semantic mediation yet continues to present the agent as having autonomously resolved the mathematical problems. The narrow operational meaning of autonomy—proof search after a formal target is supplied—is real; the public attribution allows it to signify the problem-level achievement.

### S–O–E assessment

- **S — Agency-attribution extension (S_a):** autonomy in formal proof search is publicly attributed as autonomy in resolving the mathematical problem itself. The shift is from “the agent autonomously searches for and generates a Lean proof” to “the agent autonomously resolved open mathematical problems.” This is not a claim that the theorem is invalid or that the formal statement lacks expert validation.
- **O — Objectal displacement:** the machine is the grammatical and symbolic bearer of “resolution,” while human work is acknowledged but positioned as selection, validation, and exposition around the machine's central achievement.
- **E — Social efficacy:** the formulation appears in the *Science* abstract and Table 1 and in Aarhus University's official headline and opening account. It functions as the portable public description through which the achievement is announced and institutionally recognized.

### Assessment

The case turns on the public wording's grammatical object and attribution of agency. The technical operation is autonomous proof search over formalized targets, with Lean checking the resulting proof terms and experts validating that the formal statements correspond to the original conjectures. The public description makes the agent the subject of “resolved” and open mathematical problems its object. The institutional report repeats this formulation while explicitly identifying the mathematician's role in problem selection, solution validation, and natural-language exposition. Thus, the agent is not merely credited with generating proofs; it is publicly named as the solver of the mathematical problems, while human contribution is placed in a supporting and validating position.

The narrow operational reading of “autonomous” remains true. The ideological effect lies in the public attribution of the whole achievement to the machine, not in a denial that the proof search was autonomous. This is a positive instance of fetishistic disavowal as a structure of public representation, not an inference about private motives. It establishes the existential claim without implying that all formalization projects exhibit the same structure.

The provenance audit of #26, #741(i), #741(ii), and #125 concerns artifact identity and traceability. It is not evidence of kernel failure or, by itself, of disavowal.

Primary sources:
- https://doi.org/10.1126/science.aej2213
- https://math.au.dk/en/currently/news/news-item/artikel/gergely-deepmind
- https://arxiv.org/abs/2605.22763
- https://erdosproblems.ai/wiki/library/additive_combinatorics/tsoukalas_2026_advancing_mathematics_research_ai_driven_formal_proof_search

## 5. Liquid Tensor Experiment

### Evidence across the five moments

- **M1, real technical reliability:** the project formally verifies the main theorem of liquid vector spaces in Lean.
- **M2, distributed epistemic labour:** the completion announcement lists mathematical, formalization, technical, library, and institutional contributors and identifies Scholze’s mathematical support.
- **M3, credential condensation:** the public announcement states that the main theorem has been formally verified and that the experiment is complete.
- **M4, objectal displacement:** Topaz explicitly asks how mathematicians can know that Lean definitions are correct, identifies the possibility of pathological definitions, and describes the examples folder of semantic sanity checks. The credential is presented alongside the work that makes its formal statement meaningful.
- **M5, fetishistic disavowal:** not established. The participants acknowledge a semantic risk and respond with additional scrutiny. Continued confidence follows the added checks; it is not an instance of maintaining an overextended guarantee while leaving the acknowledged gap unaddressed.

### Assessment

Liquid Tensor is a counter-practice. It demonstrates that the condensation of collective labour into a formal verification credential need not culminate in autonomous machine authority. Semantic mediation can remain visible and become part of the basis for confidence.

Primary sources:
- https://leanprover-community.github.io/blog/posts/lte-final/
- https://leanprover-community.github.io/blog/posts/lte-examples/
- https://xenaproject.wordpress.com/2021/06/05/half-a-year-of-the-liquid-tensor-experiment-amazing-developments/

## 6. Comparative result and revision to the argument

| Case | M1 reliability | M2 distributed labour | M3 condensation | M4 displacement | M5 disavowal |
|---|---|---|---|---|---|
| Riemann | Strong | Strong and visible | Strong | Limited / not established | Not established |
| Navier–Stokes | Strong formal check | Strong | Strong | Ambiguous association | Not established |
| AlphaProof Nexus | Strong formal check | Explicit human validation | Strong autonomy framing | Supported at public-discourse level | Affirmative existence case |
| Liquid Tensor | Strong formal check | Highly visible | Present | Counter-practice | Not established |

The evidence supports a refinement of the diagnostic architecture, not a change to the five-moment model:

- Scope extension has two forms: warrant-scope extension (S_w) and agency-attribution extension (S_a). AlphaProof is analyzed under S_a; the case does not allege that its mathematical results lack warrant.
- The first two moments are enabling conditions, not sufficient causes.
- Credential condensation is a communicative transformation, not yet fetishism.
- Objectal displacement is the specifically fetishistic conversion and must be assessed through S, O, and E.
- Fetishistic disavowal is a conditional feedback mechanism that may reproduce symbolic authority through the public acknowledgement of human mediation. It is not a necessary step in every case.
- AlphaProof is the positive existence case; Liquid Tensor is the clearest counter-practice.
- The claim is existential: one well-documented public case is sufficient to establish that this configuration can occur. The other cases clarify the conditions and contrasts.

## 7. Consequences for the manuscript

The main text should:
1. distinguish formation from reproduction;
2. distinguish knowledge of the kernel’s technical scope from knowledge that the credential is being used beyond that scope;
3. treat AlphaProof as the positive existence case for public-discourse fetishistic disavowal;
4. revise Navier–Stokes language to distinguish theorem-statement fidelity from proof-route correspondence;
5. present Riemann as composite institutional certification and Liquid Tensor as a transparent semantic counter-practice;
6. preserve the philosophical claim that genuine technical reliability can support symbolic authority, without claiming that every case or every Lean practice exhibits fetishistic disavowal.
