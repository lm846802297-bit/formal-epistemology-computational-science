# Two-Case Theoretical Synthesis: Warrant-Scope Transfer in AlphaProof Nexus and Liquid Tensor

**Date:** 2026-11-28  
**Manuscript snapshot examined:** `PHTE_Anonymous_Manuscript.tex`, blob `403657444bff5686bf795872b26005f73bce8409`, branch `research/phte-zizek-materialist-revision`  
**Purpose:** Test whether warrant-scope transfer explains two different public recognition structures, and whether LTE's semantic auditability constrains that transfer.  
**Status:** Analytical memo; no manuscript edits made in this stage.

## 1. Research question and conclusion

The comparison asks:

> How can the same formal verification infrastructure participate in different public arrangements of epistemic authority and subject position?

The two cases do not form a matched experiment. They differ in task, project aim, division of labour, institutional setting, and audience. They are nevertheless a useful contrastive comparison because both rely on Lean while organizing proof production and public recognition differently.

**Main conclusion:** The evidence supports a localized, partial warrant-scope transfer in AlphaProof's public solver attribution and benchmark presentation. LTE provides a documented counter-practice that keeps semantic judgment and human mediation visible in the production and explanation of the formal result. It constrains the scope of the warrant at the level of project workflow and public exposition. The available evidence does not establish that LTE's transparency causally changes downstream community recognition, nor that it eliminates symbolic investment or the need for trust.

This distinction prevents two overclaims:
1. AlphaProof does not establish a community-wide fetishistic disavowal.
2. LTE is not an ideology-free or trust-free counterexample.

## 2. Analytical distinctions

Let:
- (V): kernel acceptance of a proof term for a formal proposition (P^*) in environment (Gamma);
- (M(P,P^*)): correspondence between the formal proposition and intended mathematical problem;
- (Sig(P)): the result's mathematical significance as an answer to the intended problem;
- (Pi): provenance and contribution history;
- (ho): the public procedure that records, announces, compares and attributes a result;
- (S(P)): public problem status;
- (A(P)): public attribution of solver/author/validator roles.

A kernel verdict warrants (V). It does not alone warrant (M), (Sig), or (Pi). Public recognition is therefore a further social and epistemic process.

### 2.1 Warrant-scope transfer

Warrant-scope transfer occurs when a public recognition procedure allows the genuine, proposition-relative warrant (V) to carry authority for wider claims about (M(P,P^*)), problem-level closure (S(P)), or attribution (A(P)), without the distinct judgments that warrant those claims remaining equally operative in the public account.

The transfer is not a logical inference and not necessarily a false statement. It is a practical and representational substitution in the way the result is recognized.

### 2.2 Fetishistic disavowal is a stronger diagnosis

Warrant-scope transfer and fetishistic disavowal must not be collapsed.

A diagnosis of fetishistic disavowal requires:
1. an acknowledged limit or constitutive gap;
2. a material credential/status that can stand in for the missing guarantee;
3. observable practical investment in that status as if the distinct judgments were settled;
4. reproduction of this substitution in public records or subsequent practice.

The mere use of Lean, the existence of a benchmark, or the public circulation of a proof artifact is insufficient. A project can use a reliable credential rationally while keeping its scope explicit.

## 3. AlphaProof Nexus: credential-centred recognition with human adjudication

### 3.1 What the evidence establishes

The public recognition chain is directly observable:
- Tsoukalas et al. describe the agent as having “autonomously resolved 9 of 353 open Erdős problems”.
- The paper also states that experts validated each formal target and that the agent helped identify misformalizations.
- PR #3778 changes the upper-density variant of Erdős #741 from `research open` to `research solved`, applies `solution found`, and credits the DeepMind prover agent.
- The results archive separates machine-generated Lean outputs from human-written natural-language proofs.
- The Erdős register records differentiated statuses, while the nine formal statements are not nine newly solved canonical Erdős problems.
- The external replay audit reports that ten published/corrected proof items pass Lean and nanoda, while treating statement correspondence as a separate question.

Sources:
- [Science paper](https://doi.org/10.1126/science.aej2213)
- [Formal Conjectures PR #3778](https://github.com/google-deepmind/formal-conjectures/pull/3778)
- [Formal Conjectures PR #4384](https://github.com/google-deepmind/formal-conjectures/pull/4384)
- [AlphaProof results archive](https://github.com/google-deepmind/alphaproof-nexus-results)
- [Erdős problem register](https://github.com/teorth/erdosproblems)
- [Independent audit](https://carlostoledo.co/reports/alphaproof-nexus.html)

### 3.2 What the contribution network adds

The results archive itself has concentrated commit authorship, but the integration network is broader:
- `mo271` integrates results and reviews other formalizations;
- `codrut3` performs detailed statement review;
- `Paul-Lez` approves/merges status-changing work;
- other contributors clean, translate, correct and attribute proof artifacts.

PR #4384 has 53 commits and 135 comments. The reviewer identified incomplete statement scope and an (m=8)-only proof; the integrator accepted the correction. PRs #3643 and #3604 show AlphaProof being used to find counterexamples to defective existing formalizations. Thus the agent is not only a solver; it also functions as a diagnostic instrument within a human adjudication network.

### 3.3 Scope-transfer assessment

The evidence supports **localized and partial warrant-scope transfer**:
- the headline and benchmark framing foreground the agent as solver;
- the public archive makes machine-generated proof artifacts the portable record of success;
- the formal register assigns a public solved status and agent attribution.

The evidence also constrains the diagnosis:
- the paper explicitly reports expert target validation;
- #741 is a variant with a distinct density interpretation;
- PR review corrects overbroad or incomplete formal statements;
- the community database records differentiated statuses;
- external replay confirms derivational validity but does not claim to settle all informal correspondence questions.

**Judgment:** Credential-centred recognition and asymmetrical solver attribution are established. A public fetish-form is a defensible interpretation of particular benchmark/headline/status practices. A community-wide fetishistic disavowal is not established. The current evidence does not show that the relevant actors knowingly treated all semantic and provenance judgments as settled by the certificate.

## 4. Liquid Tensor: distributed semantic auditability as a counter-practice

### 4.1 What the evidence establishes

LTE's semantic work is built into the project:
- Scholze's challenge arose from concern about independent scrutiny of a delicate proof.
- The formalization process exposed and corrected mathematical details.
- The Blueprint connects the mathematical argument to Lean declarations and dependencies.
- Topaz's examples test whether definitions behave as expected, including real numbers, profinite spaces, Radon measures, (p)-Banach spaces and Ext.
- PR #96 explicitly describes the Ext universal (delta)-functor property as a way to help establish that Ext is defined correctly.
- PRs #113 and #126 add mathematical examples and explanatory material.
- PRs #120 and #121 show ongoing negotiation about inline explanations, imports and intended readers.
- Scholze's public account identifies detailed human interaction through Zulip as the basis of trust and says that checking statement/definition correspondence remains a human task.
- Buzzard's retrospective explicitly attributes the mathematics to humans and the wider team.

Sources:
- [Scholze's original challenge](https://xenaproject.wordpress.com/2020/12/05/liquid-tensor-experiment/)
- [Scholze's 2021 progress account](https://xenaproject.wordpress.com/2021/06/05/half-a-year-of-the-liquid-tensor-experiment-amazing-developments/)
- [LTE Blueprint](https://leanprover-community.github.io/liquid/)
- [Topaz on semantic examples](https://leanprover-community.github.io/blog/posts/lte-examples/)
- [PR #96](https://github.com/leanprover-community/lean-liquid/pull/96)
- [PR #113](https://github.com/leanprover-community/lean-liquid/pull/113)
- [PR #120](https://github.com/leanprover-community/lean-liquid/pull/120)
- [PR #121](https://github.com/leanprover-community/lean-liquid/pull/121)
- [PR #126](https://github.com/leanprover-community/lean-liquid/pull/126)
- [Buzzard's retrospective](https://xenaproject.wordpress.com/2022/09/12/beyond-the-liquid-tensor-experiment/)

### 4.2 What the contribution network adds

The PR census records 57 PRs, 49 merged, 6 closed unmerged and 2 open, with 15 author accounts. Adam Topaz authored most semantic examples; Johan Commelin frequently reviewed and coordinated the work; Kevin Buzzard publicly pressed for more accessible inline explanations. The network makes visible that semantic auditability is produced through collaborative mathematical and documentary labour.

### 4.3 Does semantic auditability actually constrain warrant-scope transfer?

The answer must be divided into two levels.

**At the level of project procedure and public exposition: yes, a constraint is demonstrated.**
- The formal target is not treated as self-interpreting.
- Definition behaviour is checked against familiar mathematical examples.
- The Blueprint and source code make parts of the proof structure inspectable.
- Human semantic adjudication and contributor roles remain explicit.
- Public comments debate what evidence a reader needs to trust the formalization.

This makes (M(P,P^*)) and (Pi) more visible and keeps them operative in the project's warrant structure. The certificate is not presented as the sole source of mathematical meaning or credit.

**At the level of downstream recognition and reader behaviour: not yet demonstrated.**
- There is no evidence that every reader inspected the examples or Blueprint.
- The examples are targeted sanity checks, not a complete independent proof of equivalence for every definition.
- The open documentation PRs show that accessibility was still being negotiated.
- No causal evidence shows that these practices changed how the wider mathematical community recognized the result.

**Judgment:** LTE is a strong example of a counter-practice that constrains the conditions for warrant-scope transfer. It is not proof that semantic transparency eliminates the transfer or fetishistic investment.

## 5. Direct comparison

| Dimension | AlphaProof Nexus | Liquid Tensor |
|---|---|---|
| Proof production | Agent performs proof search over supplied formal targets | Human mathematicians and formalizers construct the formal proof |
| Semantic validation | Expert target validation, corrections and formal-conjecture review | Blueprint, examples, human discussion and iterative definition checks |
| Public recognition | Benchmark count, problem-status register and agent solver attribution | Project completion, public proof structure and named human contributors |
| Machine subject-position | Visible solver / prover agent | Assistant to construction, checking and understanding |
| Human subject-positions | Target selector, formalizer, validator, integrator, reviewer and expositor | Mathematical lead, formalizer, semantic auditor, reviewer and infrastructure contributor |
| Provenance visibility | Machine proof files and human prose files are separate; integration PRs expose correction and credit | Human roles and public review history are more directly distributed across the project |
| Scope-transfer assessment | Localized transfer in benchmark and solver attribution, constrained by human review | Procedural constraint through visible semantic work; downstream effect not established |
| Fetishistic disavowal | Not established community-wide; evidence supports a narrower public fetish-form diagnosis | Not established; evidence instead shows a counter-practice that keeps mediation visible |

The contrast is not “opaque AI versus transparent humans”. Both cases rely on Lean, mathematical judgment, libraries and distributed expertise. The difference is the public organization of (ho), the recognition procedure, and the visibility and authority of (M) and (Pi).

## 6. What the comparison does and does not show

### It shows

1. The same verification infrastructure can be embedded in different production and recognition arrangements.
2. Public solver attribution is not determined by kernel verification; it is organized through benchmark, repository, paper and review practices.
3. Public semantic auditability can keep target correspondence and provenance operative in the production and explanation of a result.
4. The subject-position of the machine is a public attribution, not evidence that the machine is a Lacanian subject.
5. The symbolic Other is supported by different material arrangements: benchmark/status registers and publication channels in AlphaProof; expert interaction, Blueprint, Mathlib, named mathematicians and project community in LTE.

### It does not show

1. That AlphaProof users privately believe the agent independently performed every mathematical task.
2. That all mathematicians accept the benchmark's solver attribution.
3. That LTE's semantic examples are universally inspected or causally alter external recognition.
4. That transparency eliminates the big Other or symbolic investment.
5. That the difference between the cases is caused by semantic transparency alone; task, project aim, division of labour, audience and institutional setting also differ.

## 7. Relation to adjacent literature and originality

The article must not claim originality for distinctions or empirical findings already developed elsewhere.

### Kallel and El Louadi (2026)

Their preprint, *Verification Abundance, Adjudication Scarcity*, explicitly distinguishes:
- derivational validity;
- representational fidelity;
- epistemic significance.

It argues that reducing the cost of kernel checking shifts pressure onto expert adjudication. It also supplies a mismatch taxonomy and measures the ratio between proof artifact size and the statement audit surface.

**Consequence:** The present paper's originality is not the three-layer distinction or the claim that human semantic adjudication remains necessary. Its contribution is the Žižekian analysis of how a genuine local warrant becomes a material bearer of wider public recognition and solver attribution.

### López-Corona (2026)

*From Authorial Mathematics to Studio Mathematics* develops the human-machine assemblage as a unit of mathematical production, proposes a contribution-authority trace and an understanding audit, and compares LTE with other collaborative projects. The abstract explicitly says these are governance designs rather than validated measures.

**Consequence:** The present paper should not claim to be the first to identify distributed mathematical labour, human-machine production, traceable provenance or the LTE as a collaborative case. Its distinctive question is how the public credential can become a fetish-form through which a wider symbolic guarantee appears available.

### Ochigame, MacKenzie, Rosental, and social epistemology

Existing work already covers proof cultures, theorem certification, automation, labour and credit, and trust in mathematical practice. The contribution must be framed as a specific ideological mechanism, not a general discovery that mathematical knowledge is social.

## 8. Theoretical refinement recommended

No new concept is needed. The existing framework should be stated more rigorously:

1. **Credential circulation** is not itself fetishism.
2. **Institutionalized recognition** is a necessary social translation from formal artifact to public status; it can be entirely rational.
3. **Warrant-scope transfer** occurs when the public status gives the local kernel warrant authority over distinct correspondence, significance or attribution judgments.
4. **Fetishistic disavowal** is the stronger case in which an acknowledged constitutive gap is practically subordinated to the credential as if the guarantee were complete.
5. **Semantic auditability** is a counter-practice when it makes correspondence and provenance operative in the recognition procedure, not merely available in a repository.

This preserves the distinction between a useful public status, a transfer of warrant scope, and a fetishistic relation to the credential.

## 9. Implications for the manuscript

The current manuscript's main architecture is sound, but the integrated conclusion should be calibrated as follows:

- Retain AlphaProof as the case of credential-centred recognition and asymmetrical solver attribution.
- Retain LTE as distributed semantic auditability and negotiated attribution.
- Describe AlphaProof's transfer as localized and partial, especially in benchmark/headline and solver-position practices.
- Describe LTE's semantic audit as a procedural constraint, not as proof of a causal change in community reception.
- Do not claim that either case establishes community-wide private belief or universal fetishistic disavowal.
- Make clear that the comparison is contrastive, not a matched causal test.

**Final theoretical judgment:** Warrant-scope transfer remains a promising and distinctive mechanism for the article, provided it is treated as a variable public process rather than a universal property of Lean verification. AlphaProof shows how a local proof warrant can be condensed into a solver-centred public status; LTE shows how semantic audit and distributed attribution can keep the additional judgments visible and constrain that condensation. The difference between these cases is precisely where the Žižekian analysis becomes most useful: it explains not whether a certificate is technically valid, but how its real validity is invested with a wider symbolic authority.
