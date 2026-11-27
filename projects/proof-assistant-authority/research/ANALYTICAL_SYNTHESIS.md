# Analytical synthesis and provisional propositions

**Project:** *In Lean We Trust? The Ideology of Machine-Checked Proofs in Science*  
**Cut-off:** 27 November 2026  
**Status:** provisional analytic memo; not a final interpretation.

## 1. Central research problem

The paper is not a study of whether machines deserve trust, nor a study limited to whether mathematicians trust Lean. It investigates how contemporary society establishes and recognizes the authority of scientific knowledge when AI systems participate in producing claims and machine-verification systems provide visible forms of technical certification.

The guiding question is:

**How does machine verification become a publicly legible symbol of scientific reliability, and what ideological functions does this symbol perform in contemporary society?**

The relevant social chain is:

**AI-assisted production → formal or technical checking → expert and institutional appraisal → public communication → audience interpretation.**

No step entails the next automatically. A machine-checked theorem does not automatically produce public trust; public trust does not automatically imply ideological capture.

## 2. Four objects of trust

The cases suggest that “trust in AI science” is too coarse a category. At least four objects must be distinguished:

1. **Discovery trust:** confidence that an AI system can find useful conjectures, arguments, or proof strategies.
2. **Checker trust:** confidence that a proof assistant correctly checks a formal proof of a specified proposition.
3. **Correspondence trust:** confidence that the formal proposition and proof faithfully represent the intended mathematical or scientific claim.
4. **Institutional/communicative trust:** confidence that experts, universities, companies, journals, and media accurately assess and communicate what has been established.

Public audiences may trust one object while distrusting another. For example, they may trust Lean's kernel but distrust an AI-generated research claim; trust a mathematician while remaining unsure about a formal artifact; or trust science institutions while disapproving of extensive AI involvement.

## 3. Three distinct epistemic achievements

The four cases make it necessary to separate:

- **Technical verification:** a formal proof term is accepted for a formal statement under specified definitions and axioms.
- **Mathematical understanding:** human mathematicians can reconstruct, explain, and assess why the argument works and how it contributes to the subject.
- **Social recognition:** experts, institutions, journals, prize bodies, and public audiences treat the result as an established contribution.

These dimensions can support one another, but they are not equivalent. The Riemann case is especially clear: extensive machine checking can coexist with the absence of a complete human read-through. The Navier–Stokes case shows that kernel validity of a formal object does not establish that a separate natural-language proof has been faithfully translated. The Waring preprint shows that AI attribution and self-refereeing do not amount to independent review. AlphaProof Nexus shows how formal proof search can be integrated with human validation of the statement being proved.

## 4. Provisional propositions to test

### Proposition 1 — Machine verification as a public credential
Machine verification can function as a visible credential of reliability in public communication, but its meaning depends on how the statement, assumptions, and scope are represented.

**Evidence to test:** headlines, press releases, project pages, and whether they identify the precise object checked.

### Proposition 2 — Trust is mediated, not simply transferred
Public confidence in machine-checked science may be mediated by trust in named experts, universities, companies, research communities, and journals. It should not be assumed that the public directly trusts the machine.

**Evidence to test:** public survey experiments that vary AI disclosure and human oversight; public statements that foreground or background human contribution.

### Proposition 3 — Visibility of human labour affects legitimacy
When the human contribution, review process, and accountability structure are visible, audiences may evaluate AI-assisted research differently than when the system is presented as an autonomous knowledge producer.

**Evidence to test:** Chen and Jia (2026), N=806 survey experiment; compare disclosure conditions and their findings with the four public cases.

### Proposition 4 — Formal correctness does not settle semantic correspondence
The public meaning of “machine-verified” can exceed the formal achievement if the semantic relation between the formal statement and the intended scientific claim is not established.

**Evidence to test:** Navier–Stokes written paper vs pinned Lean commit; Riemann Mathlib statement vs announcement; AlphaProof formal statements vs historical conjectures.

### Proposition 5 — Epistemic fetishism is a possible, not automatic, diagnosis
A Žižekian account of fetishism is plausible when collective epistemic labour and institutional conditions appear as an autonomous property of the machine. It is not established merely because a machine is praised or trusted.

**Evidence to test:** recurring patterns in which expert work, theorem selection, semantic translation, and review disappear from public narratives while machine authority is foregrounded.

### Proposition 6 — Public ambivalence can coexist with technical confidence
People may accept that machine checking is technically reliable while remaining sceptical of AI's role in generating research, its effects on human authorship, or the accountability of institutions.

**Evidence to test:** Chen and Jia (2026); Wellcome Global Monitor; public reactions to the Riemann and AlphaProof announcements.

## 5. Žižekian interpretation: hypotheses, not labels

- **Ideological fantasy:** machine verification may serve as an imagined guarantee that scientific uncertainty can be finally controlled. This should be tested by identifying what public narratives ask the checker to guarantee.
- **Fetishism:** the social and collective labour that makes verification meaningful may appear as an autonomous property of the machine. This requires evidence of representational displacement, not merely the use of a technical tool.
- **Cynical ideology/disavowal:** known limitations may coexist with practices that continue to rely on an enlarged image of machine authority. Public text alone cannot establish that individuals consciously know and disavow the limitation; the analysis should focus on documented institutional or communicative practices and avoid diagnosing motives.
- **Big Other / subject supposed to know:** the machine is not literally the Big Other or a psychoanalytic subject. The concept may help analyze how a knowing position is attributed within a wider symbolic order involving experts and institutions.

## 6. Case-by-case provisional interpretation

### Riemann hypothesis — Claude + Lean
Strong machine-checking evidence and multiple independent proof-checking reports coexist with the lack of a human-readable mathematical paper and the absence of a mathematician having read the complete proof through at the 26 November cut-off. This is a strong case for separating checker trust, statement correspondence, human understanding, and social acceptance. Public experts express excitement and guarded optimism, not unanimous acceptance.

### Waring's problem — GPT-6.2 Astra
The preprint explicitly attributes the work to GPT-6.2 Astra, says the authors rewrote it, and says the same model refereed it. It is unreviewed and has no Lean certificate documented. This case isolates AI authorship and self-assessment, but its public reception is still thin. It must not be treated as an established theorem.

### Navier–Stokes — OpenAI multi-agent discovery + Lean
The formal repository records valid Lean proofs of its formal statements, but an independent mathematical critique reports that some Lean estimates are weaker or differ from those in the natural-language paper. This is a direct semantic-correspondence problem, not evidence of a kernel failure or a refutation of the underlying theorem. It is the clearest case for distinguishing what was formally checked from what public audiences may infer was checked.

### Erdős problems — AlphaProof Nexus
The *Science* paper reports formal proofs and human validation of statement correspondence. Public expert reactions and a secondary audit raise questions about benchmark scope, historical novelty, and whether all formal statements match the original conjectures. This case is valuable precisely because technical proof checking, novelty, historical interpretation, and human understanding can diverge.

## 7. Research design implication

The first paper should combine:
- primary formal artifacts and exact theorem statements;
- AI-use disclosures and authors' own descriptions;
- institutional announcements and review records;
- independent media reports;
- expert commentary;
- bounded public-discussion samples;
- population survey and experiment results on trust in science and AI.

Do not claim that a particular announcement changed public trust without a causal design. The existing Chen–Jia experiment is directly relevant to AI disclosure in research but does not test proof assistants. A later experiment could manipulate (i) AI role, (ii) formal verification, (iii) human review, and (iv) institutional endorsement, but it is not required to complete the initial comparative textual study.

## 8. Current conclusion

The strongest current thesis is not that society blindly trusts machines. It is that machine verification can become one credential within a wider social order of scientific authority. The public may rely on the checker indirectly through experts and institutions, while simultaneously remaining ambivalent about AI authorship and human accountability.

The paper's original contribution should be to explain how the genuine technical reliability of a bounded checker is represented, mediated, and sometimes enlarged in the social production of scientific certainty—while also identifying cases in which trust is warranted and public communication preserves the limits of verification.

## 9. Results of the next research pass (27 November 2026)

### 9.1 Public-trust experiment

Chen and Jia (2026), *AI and Ethics* 6, article 223, DOI 10.1007/s43681-026-01039-w, provide a preregistered N=806 experiment with six disclosure conditions. Participants were shown a description of an academic paper and an AI-use statement, not an actual paper or proof. The sample was recruited through Prolific with demographic quotas matching U.S. gender, age, and ethnicity; it should not be described as a probability sample of the U.S. population.

The experiment finds:
- the no-AI condition has the highest mean on all ten outcomes;
- the both-theoretical-and-methodological-AI condition has the lowest mean on the eight directional outcomes and lowest perceived ethicality;
- theory-only versus method-only AI differences are small and not statistically significant on the eight directional outcomes; perceived transparency is higher for method-only AI;
- clarifying that the authors retained theoretical framing, hypotheses, analyses, and interpretation improves several outcomes relative to a bare language-polishing disclosure;
- AI-use frequency moderates six of ten outcomes; self-reported AI knowledge and general trust in science do not significantly moderate effects.

This evidence supports the proposition that perceived human intellectual contribution and accountability matter to public evaluation. It does not establish how the public evaluates Lean verification or an AI-generated proof. The dedicated analysis is in CHEN_JIA_EXPERIMENT_ANALYSIS.md.

### 9.2 Revised case-level ideology assessment

The four-case matrix is now in CASE_IDEOLOGY_MATRIX.md. Its provisional result is deliberately differentiated:
- **Riemann:** a plausible fantasy of machine certification as a visible guarantee, but independent checker reliability is real and expert commentary explicitly distinguishes formal checking from human understanding. Fetishism is possible in some compressed headlines; cynical ideology is not established.
- **Waring:** an unusual AI-producer/AI-referee loop, but the preprint discloses author rewriting and lacks external verification. This is a case of attempted self-authorization, not evidence of public belief or cynical disavowal.
- **Navier–Stokes:** strongest candidate for epistemic fetishism at the level of representation, because valid Lean proofs of formal declarations can be made to stand for the correctness of a separate natural-language proof despite a documented semantic mismatch. The mismatch is not a kernel failure or refutation of the theorem.
- **Erdős:** counter-case in which the paper discloses denominators, human statement validation, and the need for expert review. Public expert reactions and a secondary audit add qualifications; not every use of formal verification is fetishistic.

No case presently establishes cynical ideology in the strict sense. That diagnosis would require evidence that relevant actors acknowledge a limitation and nevertheless continue to reproduce an enlarged guarantee in practice.

### 9.3 Proposed original model

THEORETICAL_MODEL.md develops the concept of **mediated verification authority**: the socially recognized authority that accrues to a scientific claim when a bounded technical check is interpreted through expert testimony, institutional endorsement, and public communication.

The model separates five stages:
1. knowledge production;
2. technical checking;
3. semantic and expert mediation;
4. institutional and communicative certification;
5. public interpretation and trust.

It also distinguishes four objects of trust: AI discovery, proof-checker reliability, semantic correspondence, and institutional/communicative reliability.

### 9.4 What Žižek adds beyond Hardwig

Hardwig explains why a layperson can rationally depend on experts and collective cognitive labour. He gives an account of the epistemic legitimacy of dependence, not a general explanation of why a society invests a particular technical object with the symbolic function of a final guarantee.

Žižek adds a different question: how does a social order stage and sustain its relation to uncertainty? Fantasy identifies the imagined guarantee; fetishism identifies how collective relations can appear as a property of an object; cynical disavowal asks whether acknowledged limits remain practically ineffective. These concepts do not replace Hardwig's normative account and should not be used to redescribe all trust as ideology.

The proposed contribution is therefore a two-part account:
- **Normative:** when is mediated reliance on machine verification warranted?
- **Critical:** when does the public or institutional representation of that reliance make the machine appear to guarantee more than the verified proposition warrants?

The present evidence supports the architecture of this model, but not yet a population-level causal claim that machine verification increases public trust.
 
## 10. Lean-centered scope decision (27 November 2026)

The empirical analysis is centered on Lean rather than distributed evenly across proof-assistant systems. The four primary cases are:
1. Riemann hypothesis — Claude-assisted discovery and Lean formal verification.
2. Navier–Stokes — OpenAI multi-agent discovery and Lean formalization, with a dispute about semantic correspondence to the written proof.
3. Erdős problems — AlphaProof Nexus proof search and Lean verification, with expert validation of formal statements.
4. Liquid Tensor Experiment — historical Lean case of formal checking and human mathematical scrutiny.

Waring/GPT-6.2 Astra is a contrast case only: it concerns AI-generated mathematical work without a Lean certificate documented at the cut-off. Coq, Isabelle/HOL, and HOL Light remain historical or conceptual comparators, not parallel case families.

This decision sharpens the paper's question. Rather than asking broadly whether proof assistants acquire authority, the paper asks how **Lean**, as a highly visible formal verification environment in current AI-assisted mathematics, becomes a public credential of scientific reliability. The wider social question remains unchanged: how ordinary audiences understand the relation among AI discovery, Lean checking, expert judgment, institutional recognition, and scientific truth.
