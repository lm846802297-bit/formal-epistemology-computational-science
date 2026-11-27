# A social-epistemic model of Lean verification and public trust

**Project:** *In Lean We Trust? The Ideology of Machine-Checked Proofs in Science*  
**Cut-off:** 27 November 2026  
**Status:** proposed original model; to be tested against the Lean cases.

## 1. Purpose

The model explains how a technically bounded Lean verification result can become a socially recognized credential of scientific reliability. It integrates social epistemology, science communication, institutional trust, and Žižekian ideology critique without treating them as interchangeable.

## 2. Five-stage chain

### Stage 1 — Knowledge production
AI systems and human researchers generate conjectures, arguments, proofs, and mathematical results.

### Stage 2 — Lean verification
Lean checks a proof term against a formal proposition under specified definitions, axioms, libraries, and trusted computing assumptions.

### Stage 3 — Semantic and expert mediation
Experts assess whether the formal proposition represents the intended mathematical or scientific claim, whether the theorem's hypotheses are instantiated, and what the result means in the discipline.

### Stage 4 — Institutional and communicative certification
Universities, companies, journals, scientific societies, and media select which features of the process to foreground. They assign labels such as “AI-discovered,” “Lean-verified,” “breakthrough,” “solved,” or “accepted.”

### Stage 5 — Public interpretation and trust
Audiences interpret the claim using prior beliefs, trust in science, trust in institutions, experience with AI, perceived transparency, and media framing.

No stage entails the next automatically.

## 3. Four objects of trust

1. **AI discovery trust:** confidence that an AI system can find conjectures, arguments, or proof strategies.
2. **Lean checker trust:** confidence that Lean correctly checks a proof of a specified formal proposition.
3. **Semantic correspondence trust:** confidence that the formal proposition and proof faithfully represent the intended mathematical or scientific claim.
4. **Institutional/communicative trust:** confidence that experts, universities, companies, journals, and media accurately assess and communicate what has been established.

A public audience may trust Lean's kernel but distrust an AI-generated claim; trust a mathematician but remain unsure about a formal artifact; or trust science institutions while disapproving of extensive AI involvement.

## 4. Three transformations

### A. Technical credentialing
A Lean check becomes evidence that a specified proposition has been proved within a formal system under stated definitions and axioms.

### B. Social authorization
Experts and institutions make the formal result legible and authorize its relevance to a wider mathematical or scientific claim. This is warranted only where semantic correspondence and assumptions are supported.

### C. Symbolic generalization
Public discourse may treat Lean verification as a more general sign that “science has certainty,” even when the check covers only one link in the chain. This is where a Žižekian ideological analysis may become relevant.

## 5. Hardwig and Žižek

### Hardwig / social epistemology
Hardwig explains why a non-expert can rationally depend on experts and collective cognitive labour. The individual cannot reproduce every proof or experiment, so justified knowledge depends on testimony, competence, honesty, division of labour, and reliable institutions.

### Žižek
Žižek asks how a social order organizes its relation to uncertainty:
- **Fantasy:** what image of a final guarantee makes the social practice appear coherent?
- **Fetishism:** how does collective labour or a social relation appear as a property of an object?
- **Cynical disavowal:** how can a limitation be known and yet remain practically ineffective in the reproduction of authority?

Žižek does not replace Hardwig's normative account. His contribution is a critical account of the symbolic function of the authority that a society invests in.

## 6. Proposed concept: mediated verification authority

**Mediated verification authority** is the socially recognized authority that accrues to a scientific or mathematical claim when a bounded Lean check is interpreted through expert testimony, institutional endorsement, and public communication.

It has four components:
1. **Checker reliability:** Lean correctly checks the encoded proof.
2. **Semantic warrant:** the formalized proposition faithfully represents the intended claim.
3. **Institutional warrant:** qualified experts and institutions assess the result and its significance.
4. **Public warrant:** audiences receive sufficient information to understand what is and is not established.

This is a descriptive concept, not automatically a critical judgment. It can identify legitimate as well as distorted authority.

## 7. Proposed concept: epistemic fetishism of Lean verification

**Epistemic fetishism of Lean verification occurs when the socially produced reliability of a Lean-checked result is represented as an autonomous property of the machine, while the human, semantic, and institutional relations that make the check relevant recede from view.**

Necessary evidence:
- a traceable collective process behind the result;
- public representations that foreground Lean as autonomous guarantor;
- a demonstrable omission or displacement of conditions necessary to interpret the check;
- comparison with alternative representations that preserve those conditions.

A headline that says “Lean verified X” is not enough on its own. If the body explains the exact theorem, assumptions, human role, and review status, the headline may be reasonable compression.

## 8. Testable implications

The Chen–Jia (2026) experiment shows that public evaluations respond to disclosure of AI's role and to statements about retained human intellectual contribution. It does not test Lean. The following are hypotheses for a later, proof-assistant-specific study:

- **H1 — Human-accountability visibility:** named human review and responsibility increase trust relative to an otherwise identical AI-only disclosure.
- **H2 — Lean credential:** adding a credible Lean-verification statement increases perceived reliability of the formal proposition, but may not increase trust in the broader scientific conclusion unless semantic correspondence is also disclosed.
- **H3 — Scope comprehension:** explaining the difference between Lean proof checking and source-claim correspondence improves participants' ability to identify what has been established.
- **H4 — Institutional mediation:** endorsement by a reputable university or mathematical society may affect trust independently of AI role and Lean status.
- **H5 — AI experience:** prior AI use may moderate responses; direction and functional form should be tested rather than assumed.

A future factorial experiment could vary AI contribution, Lean verification, human review, and institutional endorsement. It is not part of the current phase.

## 9. Fit to the four Lean cases

- **Riemann:** high checker reliability; Mathlib statement correspondence reported; human understanding and conventional review remain distinct.
- **Navier–Stokes:** Lean checks formal declarations; an independent critique reports mismatch with some natural-language estimates. Tests semantic warrant directly.
- **Erdős:** Lean proof search and checking are accompanied by human validation of formal statements. Tests transparent mediated authority.
- **Liquid Tensor:** Lean formalization and human mathematical interaction jointly shaped expert confidence. Tests hybrid human-machine authority.

## 10. Provisional contribution

Hardwig explains the rational possibility and conditions of epistemic dependence. The proposed model adds an account of how a technical credential travels through institutions and communication to become public authority. Žižek adds a critical account of the symbolic function of this authority: how a society may invest in an image of final certainty, how collective labour can appear as an autonomous machine property, and how known limits may or may not be displaced in practice.

The contribution is not that all trust is ideological. It distinguishes warranted mediated reliance on Lean from cases where a bounded verification result is made to carry an unwarranted symbolic guarantee.

## 11. Why society values a symbolic guarantee: uncertainty relocation

The model must not assume that society simply desires absolute certainty. A more defensible starting point is the structural asymmetry between the social reach of scientific claims and the unequal distribution of the capacity to assess them. Lay audiences often lack first-hand access to data, methods, proofs, and institutional deliberation. Public trust therefore depends on a network of testimony, source credibility, communication, and research practices.

Lean offers a visible, reproducible credential: a proof term is checked against a specified formal proposition. This can make one part of a complex epistemic chain legible to non-specialists through a simple public sign such as “formally verified.” The sign can be useful and warranted within its scope.

Yet verification does not abolish uncertainty; it relocates it. The kernel can settle a derivational question about a formal object. It does not by itself settle whether the object represents the intended problem, whether the assumptions are appropriate, what the result contributes, or whether the public description is accurate. As technical uncertainty at the kernel level falls, the importance of semantic, interpretive, institutional, and communicative judgments can rise.

Thus the central hypothesis is not that Lean removes uncertainty, but that **Lean makes one form of uncertainty highly controllable and thereby gives a visible form to the wider social desire for reliable knowledge**. Whether that visible credential is understood as limited or generalized beyond its warrant is the key empirical question.

## 12. Close prior literature and novelty boundary

Kallel and El Louadi (2026), “Verification Abundance, Adjudication Scarcity” (arXiv:2608.28997), already distinguish derivational validity, representational fidelity, and epistemic significance, and argue that machine checking transfers rather than eliminates the human adjudication burden. This project does not claim those distinctions as original.

De Millo, Lipton, and Perlis (1979), “Social Processes and Proofs of Theorems and Programs,” DOI 10.1145/359104.359106, argue that mathematical confidence is shaped by social processes of reading, criticism, simplification, and acceptance. Their account is a historical precursor for the social dimension of proof.

Fetzer (1988), “Program Verification: The Very Idea,” DOI 10.1145/48529.48530, distinguishes the formal algorithmic structure from the program as a causal object. The present paper should engage the analogy carefully: a mathematical theorem in Lean is not identical to a program's empirical behaviour, but both cases expose the need to distinguish formal relations from what the formal object is taken to represent.

Iordanou, Antoniou, and De Vos (2026), “Public Trust in Science: A Systematic Literature Review,” DOI 10.1007/s10805-026-09732-5, synthesize 124 empirical studies and organize public trust factors around receiver, message, and source. Their review identifies integrity, transparency, epistemic inclusion, and communication channels as important. This supports the society-wide framing and warns against a single-factor account in which a technical credential alone creates trust.

**Proposed originality:** the paper investigates the symbolic and ideological function of a highly visible formal-verification credential in the public mediation of scientific knowledge. It connects the bounded epistemic warrant of Lean to the wider social organization of trust and to Žižek's account of fantasy and fetishism. The original claim is about the social life of the guarantee, not the technical distinction between proof checking and semantic interpretation.