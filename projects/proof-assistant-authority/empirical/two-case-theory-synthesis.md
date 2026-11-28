# Independent Theoretical Synthesis: AlphaProof Nexus and Liquid Tensor

**Date:** 2026-11-28  
**Empirical basis:** Stage 1 GitHub collaboration and contribution-network study, accepted in `stage1-github-acceptance.md`.  
**Cases:** AlphaProof Nexus / Formal Conjectures and Liquid Tensor Experiment.  
**Status:** second-stage analytical synthesis; no manuscript edits made.

## 1. Research question

How can the same formal verification infrastructure participate in different public arrangements of epistemic authority and subject position?

The comparison is contrastive, not a matched experiment. The cases differ in research aim, task, division of labour, audience, institution and repository architecture. The analysis therefore identifies mechanisms and contrasts; it does not attribute their differences to semantic transparency alone.

## 2. Empirical basis after Stage 1

### AlphaProof Nexus

The output archive has six commits in the inspected snapshot (five by aferr and one CI commit by eric-wieser), no PRs and four issues. Its public recognition and integration network is wider and appears in Formal Conjectures:

- PR #3778: mo271's upper-density variant of Erdős #741; approved by Paul-Lez; changes the variant status from research open to research solved and credits the DeepMind prover agent.
- PR #4384: 53 commits, 135 issue comments and 49 review events (46 COMMENTED, 3 APPROVED). codrut3's review identifies incomplete target statements and an m=8-only result; mo271 accepts corrections.
- PR #3721: one CHANGES_REQUESTED and one APPROVED review; the description separates AlphaProof's construction from Claude-assisted Lean translation.
- PRs #3643 and #3604: AlphaProof counterexamples expose defects in existing formalizations, which human contributors correct.
- PR #2398: raw AlphaProof output is cleaned for maintainability and described as joint work.

The empirical picture is therefore not “machine output accepted without review”. It is a concentrated proof-output archive connected to a human network that validates, corrects, integrates, attributes and assigns status.

### Liquid Tensor Experiment

The repository census contains 57 PRs: 49 merged, 6 closed unmerged and 2 open, with 15 author accounts. The selected review sample provides direct evidence of iterative work:

- PR #95: 26 comments and 10 review events (9 COMMENTED, 1 APPROVED); Commelin and Topaz negotiate mathematical exposition and examples.
- PR #96: one approval for the Ext universal delta-functor example, explicitly motivated as a way to help establish that Ext is defined correctly.
- PR #104: one approval for the standard Ext¹ computation.
- PR #107: 14 comments and 6 review events (5 COMMENTED, 1 APPROVED).
- PR #113: 19 comments and 9 review events (8 COMMENTED, 1 APPROVED) on Radon-measure examples.
- PR #120: remains open; one approval and a discussion of imports as evidence against notation tricks.
- PR #121: remains open; discussion of intended readers and inline explanations.
- PR #126: 9 comments and 3 review events (2 COMMENTED, 1 APPROVED).

The examples, Blueprint and repository discussions make some semantic work inspectable. They are produced through collaboration; they are not an automatic property of Lean.

## 3. Three levels that must not be conflated

Let:

- (V): kernel acceptance of a proof term for a formal proposition (P^*) in environment (Gamma);
- (M(P,P^*)): correspondence between (P^*) and the intended informal problem (P);
- (mathrm{Sig}(P)): the mathematical significance of the result as an answer to (P);
- (Pi): provenance and contribution history;
- (ho): the public procedure that records, announces, compares and attributes a result;
- (S(P)): public status;
- (A(P)): public attribution of solver, author, formalizer and validator roles.

The kernel warrants (V). It does not alone warrant (M), (mathrm{Sig}), or (Pi). Public recognition is a further social and epistemic process.

Three different phenomena follow:

1. **Credential circulation:** a valid formal artifact is stored, cited, checked or used. This can be entirely rational.
2. **Warrant-scope transfer:** the public recognition procedure allows the local warrant (V) to carry authority for distinct claims about correspondence, problem-level closure or attribution, without those additional judgments remaining equally visible and operative.
3. **Fetishistic disavowal:** the stronger case in which an acknowledged constitutive gap is practically subordinated to the credential as if the wider guarantee were complete.

A status transition does not by itself establish warrant-scope transfer. Warrant-scope transfer does not by itself establish fetishistic disavowal.

## 4. AlphaProof: credential-centred recognition, but not unreviewed recognition

### 4.1 What is established

The public chain is observable:

- The paper frames the agent as autonomously resolving nine of 353 open Erdős problems.
- The paper also states that experts validate the formal statements and that the agent can expose misformalizations.
- The results archive makes generated Lean outputs portable and retrievable.
- Formal Conjectures PR #3778 assigns a solved status to a specific upper-density variant and attributes the proof discovery to the DeepMind prover agent.
- PR #4384 shows that human review can narrow or correct the target and reject an overbroad generalization.
- PRs #3643 and #3604 show the agent functioning diagnostically by producing counterexamples to defective formalizations.

The public recognition architecture is credential-centred in a specific sense: a machine-generated proof artifact can be attached to a benchmark entry, status record and solver attribution. The output archive and the status/integration network are distinct but connected infrastructures.

### 4.2 What is not established

The nine formal statements are not nine newly solved canonical Erdős problems. The count includes multiple parts and variants; some main problem statuses predate the agent's result. The #741 status transition concerns a specific variant, not the main problem newly becoming solved.

The paper's expert-validation statement and the review record are also counter-evidence to any claim that the community simply treats the kernel certificate as a complete semantic guarantee. The reviewers actively inspect the target and alter the claim when the formal statement is too broad.

### 4.3 Warrant-scope assessment

The strongest evidence of possible scope transfer lies in headline and benchmark commensuration: heterogeneous formal targets, including variants, are presented under the compact public description “nine open Erdős problems resolved”. This wording can make a count of formal statements appear as a count of original mathematical problems.

The formal status transition in PR #3778 is a weaker candidate for scope transfer because it is explicitly attached to the upper-density variant and is reviewed and approved. In that local register event, the status can be a warranted recognition of the specified formal target rather than an unwarranted extension of kernel authority.

**Judgment:** credential-centred recognition and an agent solver-position are established. A limited public compression of formal targets into a headline count is observable. The evidence does not establish that the whole recognition network treats the certificate as settling all semantic and attributional questions. Community-wide fetishistic disavowal is not established.

## 5. Liquid Tensor: distributed semantic auditability as a procedural constraint

### 5.1 What is established

The semantic relation is made an explicit object of project work:

- The Blueprint links mathematical exposition, Lean declarations and dependencies.
- The examples test familiar mathematical behaviour of important definitions.
- PR #96 explicitly motivates the Ext universal delta-functor example as a check that Ext is defined correctly.
- PRs #95, #104, #107, #113 and #126 show examples being authored, discussed, revised and reviewed.
- PRs #120 and #121 show public negotiation about the evidence and explanation a reader needs.
- Scholze's public account grounds his trust in detailed human interaction and correction, and explicitly retains human responsibility for checking the formal statement and definitions.
- The contribution record distributes mathematical, formalization, review and infrastructure roles among named participants.

### 5.2 What semantic auditability constrains

At the level of project workflow and public exposition, LTE constrains certificate-only attribution:

- the formal target is not treated as self-interpreting;
- definitions are checked against familiar mathematical properties;
- the proof structure is made navigable through the Blueprint;
- human semantic judgment and provenance remain visible;
- readers are invited to inspect the definitions and examples.

This is more than making source code available. The project creates explicit artifacts and review events whose stated purpose is to make mathematical interpretation inspectable.

### 5.3 What remains unproven

The examples are targeted sanity checks, not a complete independent proof that every formal definition is equivalent to the intended mathematical concept. Public availability does not show that all readers inspect them. The current repository evidence does not demonstrate that this auditability causally changes downstream recognition by the wider mathematical community.

**Judgment:** LTE demonstrates a procedural counter-practice that keeps correspondence and provenance operative in the production and explanation of the result. It does not demonstrate the elimination of trust, symbolic investment or the Big Other.

## 6. Direct comparison

| Dimension | AlphaProof Nexus | Liquid Tensor |
|---|---|---|
| Main production arrangement | Agent searches proofs over supplied formal targets; humans validate and integrate | Mathematicians and formalizers collaboratively construct the formal proof |
| Public credential | Benchmark count, proof archive and formal problem-status register | Proof archive, Blueprint, examples and project completion record |
| Semantic review | Expert validation and human corrections in integration PRs | Definition examples, Blueprint, human discussion and iterative review |
| Machine subject-position | Visible prover/solver agent in public framing | Assistant to proof construction, checking and understanding |
| Human subject-positions | Target selector, formalizer, validator, integrator, reviewer and expositor | Mathematical lead, formalizer, semantic auditor, reviewer and infrastructure contributor |
| Attribution structure | Agent is credited for proof discovery; human integration and correction are visible in separate records | Human mathematical and formalization credit is explicitly distributed |
| Scope-transfer assessment | Possible local compression in benchmark/headline representation; formal status events are variant-specific and reviewed | Procedural constraint through visible semantic work; external causal effect not shown |
| Fetishistic disavowal | Not established | Not established |

The contrast is not “opaque AI versus transparent humans”. Both cases depend on formal verification, human judgment, libraries and distributed expertise. The difference is the public organization of (ho): how the formal artifact is translated into recognized status and attribution, and how visibly (M) and (Pi) remain part of that procedure.

## 7. Žižekian interpretation: what the evidence permits

### 7.1 Practical belief

The public records show practical reliance on formal artifacts and on human review procedures. They do not give direct access to private belief.

- AlphaProof: the paper acknowledges expert validation while the agent remains the public solver in the benchmark framing. This is evidence of institutionalized reliance and divided labour, not proof that an individual privately thinks the certificate settles every issue.
- LTE: Scholze's account explicitly grounds trust in human interaction and correction. This is compatible with rational reliance on Lean and is not evidence of cynical or fetishistic belief in the machine.

The “I know well, but all the same” structure requires actor-specific evidence of an acknowledged limit plus observable practical substitution. That threshold is not met at the level of private belief in either case.

### 7.2 Subject positions

The machine's solver-position is publicly assigned, not evidence that the machine is a Lacanian subject.

- AlphaProof: the agent occupies a visible proof-discovery/solver position; human actors occupy target-selection, semantic validation, integration, correction and review positions.
- LTE: the machine is positioned as an assistant/checker within a human mathematical process; human agency and credit are distributed across the project.

These positions are produced through papers, repository metadata, status registers, review events and contributor acknowledgements.

### 7.3 The Big Other

The Big Other should not be identified literally with GitHub, Lean, Mathlib, a benchmark or a committee. These are material supports and sites through which anticipated symbolic recognition is staged.

- AlphaProof: Science publication, benchmark framing, Formal Conjectures status records and the Erdős database.
- LTE: Scholze's mathematical authority, Commelin's coordination, Zulip interaction, Blueprint, Mathlib and the project community.

The two cases show different material arrangements of recognition, not two different “Big Others” in a literal institutional sense.

### 7.4 Fetish-form and disavowal

The evidence supports analysis of the proof artifact as a material bearer of public recognition. It does not yet show that either case exhibits a complete fetishistic disavowal.

- AlphaProof offers the stronger candidate for a credential-centred fetish-form because the portable proof artifact and benchmark count can condense distributed work into a solver-centred public result.
- LTE offers a counter-practice in which semantic checks and human mediation remain operative and visible.
- Neither case proves that all actors knowingly subordinate the acknowledged gap to the credential as if a complete guarantee existed.

This distinction preserves Žižek's stronger account of practical disavowal rather than reducing it to ordinary trust in a useful tool.

## 8. Novelty boundary

The paper must not claim originality for the three-layer distinction between derivational validity, representational fidelity and significance, nor for the general existence of distributed mathematical labour, human-machine collaboration or the social organization of proof.

Kallel and El Louadi (2026) already develop verification abundance/adjudication scarcity and distinguish derivational validity, representational fidelity and epistemic significance. López-Corona (2026) already develops studio mathematics, provenance and contribution-authority traces, including LTE. MacKenzie, Rosental, Ochigame, Mathlib sociology and social epistemology also address proof cultures, certification, labour, credit and trust.

The narrower contribution remains a Žižekian account of how a genuine local proof warrant can become a material bearer of wider public recognition and attribution through a fetish-form. The present comparison refines this claim by showing that the process is variable and can be constrained by semantic auditability.

## 9. Final analytical judgment

The two cases support a contrast between credential-centred recognition and distributed semantic auditability, but not a simple binary.

AlphaProof shows how machine-generated proof artifacts can become portable public credentials and acquire solver attribution through benchmarks and status registers. Its human integration network also shows that recognition remains mediated by statement review, correction and approval.

LTE shows how semantic auditability can be built into the workflow through examples, documentation, mathematical discussion and review. This keeps correspondence and provenance visible, but does not prove that all readers inspect the material or that external recognition changes causally.

The most defensible theoretical conclusion is therefore:

**Warrant-scope transfer is a variable public process, not an intrinsic property of Lean verification.** It becomes plausible where public recognition compresses a proposition-relative proof warrant into broader claims about problem closure or solver attribution. Semantic auditability constrains this transfer when correspondence and provenance remain operative in the actual recognition procedure, not merely available in a repository.

The evidence does not establish community-wide private belief or universal fetishistic disavowal. It does establish the material and institutional practices through which public mathematical authority and subject positions are organized.

No manuscript edits are made by this memo. Any later revision must be based on this calibrated account and the accepted Stage 1 evidence.
