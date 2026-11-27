# A social-epistemic model of machine verification and public trust

**Project:** *In Lean We Trust? The Ideology of Machine-Checked Proofs in Science*  
**Cut-off:** 27 November 2026  
**Status:** proposed original model; to be tested against the four cases.

## 1. Purpose

The model explains how a technically bounded verification result can become a socially recognized credential of scientific reliability. It integrates social epistemology, science communication, institutional trust, and Žižekian ideology critique without treating them as interchangeable.

## 2. The five-stage chain

### Stage 1 — Knowledge production
AI systems, human researchers, and research teams generate conjectures, arguments, proofs, data analyses, or models.

Questions:
- What did AI actually contribute?
- Which intellectual and practical tasks remained human?
- Who selected the target problem and formal statement?

### Stage 2 — Technical checking
A formal proof assistant checks a proof term against a formal proposition under specified definitions, axioms, and trusted computing assumptions.

Questions:
- What exact proposition was checked?
- Which axioms, libraries, assumptions, and placeholders were used?
- Was the build reproducible and independently checked?

### Stage 3 — Semantic and expert mediation
Experts assess whether the formal proposition represents the intended mathematical or scientific claim, whether the model/protocol instantiates the theorem's hypotheses, and what the result means in the discipline.

Questions:
- Does the formal statement correspond to the source text?
- Does the source text prove the stated theorem?
- Has the result been independently reviewed and understood?

### Stage 4 — Institutional and communicative certification
Universities, companies, journals, scientific societies, and media select which features of the process to foreground. They assign labels such as “AI-discovered,” “formally verified,” “breakthrough,” “solved,” or “accepted.”

Questions:
- Which institution or expert is presented as the guarantor?
- Are the roles of AI, human contributors, formal checkers, and reviewers visible?
- Are uncertainty and status distinctions retained?

### Stage 5 — Public interpretation and trust
Audiences interpret the claim using prior beliefs, trust in science, trust in institutions, experience with AI, perceived transparency, and media framing.

Questions:
- Do audiences trust the finding, the researcher, the institution, or the checker?
- Do they distinguish formal checking from human understanding and social acceptance?
- Does disclosure of AI contribution change perceived legitimacy?

## 3. Three transformations

The model focuses on three possible transformations. None is automatic.

### A. Technical credentialing
A bounded formal check becomes evidence that a specified proposition has been proved within a formal system.

### B. Social authorization
Experts and institutions make the formal result legible and authorize its relevance to a wider scientific claim. This may be legitimate if semantic correspondence and assumptions are properly supported.

### C. Symbolic generalization
Public discourse may treat the formal check as a more general sign that “science has certainty,” even when the check covers only one link in the chain. This is the point at which a Žižekian ideological analysis may become relevant.

## 4. Where Hardwig and Žižek differ

### Hardwig / social epistemology

Hardwig explains why a non-expert can rationally depend on experts and collective cognitive labour. The individual cannot reproduce every proof or experiment, so justified knowledge depends on testimony, competence, honesty, division of labour, and the reliability of institutions.

Hardwig's framework can explain why the public reasonably trusts a chain of experts and checkers. It can also identify failures in that chain: lack of competence, inadequate review, or unsupported testimony.

### Žižek

Žižek's contribution is not another checklist for deciding which expert is trustworthy. It asks how a social order organizes its relation to uncertainty and authority:
- **Fantasy:** what image of a final guarantee makes the social practice appear coherent?
- **Fetishism:** how does a collective relation or labour process appear as a property of an object?
- **Cynical disavowal:** how can a limitation be known and yet remain practically ineffective in the reproduction of authority?

The additional question is thus not only whether trust is justified, but what symbolic function a particular form of guarantee performs in maintaining the social practice of trusting.

## 5. Proposed concept: mediated verification authority

**Mediated verification authority** is the socially recognized authority that accrues to a scientific claim when a bounded technical check is interpreted through expert testimony, institutional endorsement, and public communication.

It has four analytically distinct components:
1. **Checker reliability:** the formal system correctly checks the encoded proof.
2. **Semantic warrant:** the formalized proposition faithfully represents the intended claim.
3. **Institutional warrant:** qualified experts and institutions assess the result and its significance.
4. **Public warrant:** audiences receive sufficient information to understand what is and is not established.

The concept is descriptive, not automatically critical. It can identify legitimate as well as distorted authority.

## 6. Proposed concept: epistemic fetishism of formal verification

This is a narrower, critical hypothesis:

**Epistemic fetishism of formal verification occurs when the socially produced reliability of a machine-checked result is represented as an autonomous property of the machine, while the human, semantic, and institutional relations that make the check relevant recede from view.**

Necessary evidence:
- a traceable collective process behind the result;
- public representations that foreground the machine as autonomous guarantor;
- a demonstrable omission or displacement of conditions necessary to interpret the check;
- comparison with alternative representations that preserve those conditions.

A headline that says “AI proved X” is not enough on its own. If the body explains the human role, exact theorem, assumptions, and review status, the headline may be reasonable compression.

## 7. Causal hypotheses and testable implications

The existing Chen–Jia (2026) experiment shows that public evaluations respond to disclosure of AI's role in research and to explicit statements about retained human intellectual contribution. It does not test formal proof verification. The following are hypotheses for future testing:

- **H1 — Human-accountability visibility:** disclosure of named human review and responsibility increases trust relative to an otherwise identical AI-only disclosure.
- **H2 — Verification credential:** adding a credible formal-verification statement increases perceived reliability of the formal claim, but may not increase trust in the broader scientific conclusion unless semantic correspondence is also disclosed.
- **H3 — Scope comprehension:** explaining the difference between formal proof checking and source-claim correspondence improves participants' ability to identify what has been established.
- **H4 — Institutional mediation:** endorsement by a reputable university or scientific society may affect trust independently of the AI role and checker status.
- **H5 — Experience moderation:** prior AI use may moderate responses, but the direction and functional form should be tested rather than assumed.

A suitable factorial experiment, if later justified, would vary AI contribution (none / methodological / theoretical / proof generation), formal checking (absent / Lean-checked), human review (absent / named independent expert review), and institutional endorsement (absent / present). Outcomes should separately measure trust in the finding, trust in authors, perceived correctness, understanding of scope, perceived accountability, and willingness to rely on the result. This is a future option, not part of the current public-text phase.

## 8. Four-case fit

- **Riemann:** high checker reliability; semantic statement alignment reported by Lean/Mathlib; human understanding and conventional review remain separate. Tests whether public trust conflates these dimensions.
- **Waring:** AI generation and AI self-refereeing are disclosed; no formal certificate or independent review documented. Tests the social meaning of autonomous production/self-validation.
- **Navier–Stokes:** Lean checks formal statements, while an independent critique reports mismatch with some natural-language estimates. Tests the semantic-warrant link directly.
- **Erdős:** proof search and Lean checking are accompanied by human validation of formal statements and explicit review caveats. Provides a counter-case in which mediated authority is comparatively visible.

## 9. Provisional theoretical contribution

Hardwig explains the rational possibility and conditions of epistemic dependence. The proposed model adds an account of how a technical credential travels through institutions and communication to become public authority. Žižek adds a critical account of the symbolic function of this authority: how a society may invest in an image of final certainty, how collective labour can appear as an autonomous machine property, and how known limits may or may not be displaced in practice.

The model's contribution is not that all trust is ideological. It is a way to distinguish warranted mediated trust from cases where a bounded verification result is made to carry an unwarranted symbolic guarantee.
