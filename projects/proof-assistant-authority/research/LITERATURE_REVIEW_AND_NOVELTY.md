# Literature review and originality boundary

**Project:** *In Lean We Trust? The Ideology of Machine-Checked Proofs in Science*  
**Date:** 27 November 2026  
**Status:** first formal literature synthesis; primary sources and full-text locators inspected for the central works. This is a research-stage review, not the final manuscript bibliography.

## 1. The precise question and contribution

The paper asks: **How does Lean-based machine verification acquire a symbolic function as a guarantee of scientific certainty in contemporary society, and what ideological work does this guarantee perform?**

The originality claim is specifically Žižekian. The paper applies Žižek's account of ideological fantasy, fetishism, and the barred Big Other to the social life of Lean verification. It does not claim to have discovered (i) that formal proof checking is distinct from semantic correspondence, (ii) that mathematical proof acceptance has social dimensions, (iii) that non-experts depend rationally on experts, or (iv) that public trust in science has multiple determinants. These are established in prior literature.

The proposed term **epistemic fetishism of formal verification** is our own analytic extension. It describes a possible representational process in which collective epistemic labour and institutional relations appear as an autonomous property of Lean. It is not a term coined by Marx, Lacan, or Žižek.

## 2. Žižek: the primary theoretical centre

### 2.1 *The Sublime Object of Ideology* (1989)

Slavoj Žižek, *The Sublime Object of Ideology* (London: Verso, 1989; consulted Verso text with printed pagination).

Relevant locations:
- Chapter 1, “How Did Marx Invent the Symptom?”, pp. 1–56.
- Commodity fetishism and the effect of a social network appearing as a property of an element: pp. 19–20.
- Cynical reason and its relation to ideology: pp. 24–27. Žižek discusses Peter Sloterdijk's formula and does not originate the formula himself.
- “Ideological fantasy”: pp. 28–31, especially p. 30. The illusion is not simply a false conscious belief; it can be the illusion structuring social activity itself.
- Big Other as symbolic order and the contrast between a complete and barred/inconsistent Other: pp. 78–80.
- Big Other as symbolic network beyond empirical others: pp. 102–105.
- The ideological guarantee of meaning, in which an element embodying a lack is perceived as transcendent plenitude: pp. 109–110.
- The barred/inconsistent Other and fantasy as screen: pp. 136–138.

**Use in this paper:**
1. Fantasy explains how the visible act of verification may stage the closure of scientific uncertainty.
2. Fetishism explains how the social efficacy of a network can appear to reside in one object or technical element.
3. The barred Big Other explains why a society can invest a technical credential with the function of a final guarantee even though no symbolic order can supply a complete guarantee.

**Limits:** fantasy is not simply wishful thinking; fetishism is not mere admiration of technology; the Big Other is not an institution, a machine, or an omniscient agent. The three concepts must not be collapsed.

### 2.2 “The Spectre of Ideology” (1994)

Slavoj Žižek, “The Spectre of Ideology,” in *Mapping Ideology*, ed. Slavoj Žižek (London: Verso, 1994), pp. 1–33. The discussion of the ideology concept and the possibility that factually accurate content can function ideologically appears at pp. 8–9.

**Use:** prevents a simplistic true/false conception of ideology. A statement about Lean can be technically true and still have an ideological function depending on how it is related to a subject position and a social relation. The paper must analyze the function and framing of a true technical result, not allege that the proof itself is false.

**Attribution correction:** Althusser's “Ideology and Ideological State Apparatuses” is a separate chapter in *Mapping Ideology* (beginning p. 100). Do not attribute Althusser's exact thesis about material practices to Žižek as if it were Žižek's own text. Žižek's introduction reframes and extends the discussion of ideology beyond explicit doctrine.

## 3. Marx: the source of the fetishism analogy

Karl Marx, *Capital*, vol. I, Chapter 1, Section 4, “The Fetishism of Commodities and the Secret Thereof.”

Marx's account concerns the historically specific commodity form under capitalism: the social character of labour appears as an objective property of its products, and relations among producers appear as relations among things. The section's stable locator is Chapter 1, §4; page numbers vary substantially among English editions.

**Use:** provides the structural analogy for the proposed epistemic fetishism. The reliability of a Lean-checked result is produced through relations among theorem authors, formalizers, library maintainers, kernel developers, expert readers, institutions, and communicators. A public representation may make that socially produced authority appear to be a self-contained property of the machine.

**Limit:** Lean verification is not a commodity in Marx's technical sense, and the paper does not claim that the formal proof system reproduces capitalist exchange-value. The analogy concerns the appearance of a collective social relation as a property of an object. The manuscript must explicitly defend this structural extension and preserve the historical specificity of Marx's concept.

## 4. Lacan: two distinct concepts and their proper locations

### 4.1 Subject-supposed-to-know

Jacques Lacan, *The Seminar, Book XI: The Four Fundamental Concepts of Psychoanalysis*, ed. Jacques-Alain Miller, trans. Alan Sheridan (New York: W. W. Norton, 1977; reissued 1998), Chapter XVIII, “Of the Subject Who Is Supposed to Know, of the First Dyad, and of the Good,” pp. 230–235. The formula “As soon as the subject who is supposed to know exists somewhere ... there is transference” appears on p. 232.

Lacan's discussion concerns the analyst's position in transference, the trust placed in the analyst, and the attribution of a knowing position. He explicitly notes that the analyst is not a god and cannot claim absolute knowledge.

**Use:** a restricted analogy for the attribution of a knowing position to an expert, institution, or technical credential. It cannot be generalized into a theory of all trust, and Lean is not a psychoanalytic subject.

### 4.2 “There is no Other of the Other”

Jacques Lacan, *Le Séminaire, Livre VI: Le désir et son interprétation* (Paris: La Martinière / Le Champ freudien, 2013), session of 8 April 1959, Chapter XVI, “There is no Other of the Other”; the corresponding French passage is cited at p. 108. In Cormac Gallagher's English working translation from unedited typescripts, the session date is 8 April 1959 and the passage occurs at typescript page 206. Bruce Fink's published English translation, *Desire and Its Interpretation* (Polity, 2019), includes Chapter XVI; the printed page for the exact passage has not yet been independently verified.

The passage says that no signifier in the Other can guarantee the truth or authenticate the signifying chain. This is the primary Lacanian source for the absence of a final symbolic guarantee.

**Important correction:** this formula is explicitly located in Seminar VI, session 8 April 1959, Chapter XVI. It must not be cited as if it originated in Seminar XVI or Seminar XX. Earlier internal notes assigning it to those seminars are superseded by this correction.

### 4.3 Relation between the two concepts

The subject-supposed-to-know is a transferential position attributed to a subject; the Big Other is the symbolic locus/order in which signifiers, norms, and recognition operate. The absence of an Other of the Other means that the symbolic order has no final external signifier guaranteeing its consistency. These concepts are related but not interchangeable.

**Application:** Lean may be positioned as a credential within a symbolic order that seeks a guarantee. It is neither the Big Other nor the subject-supposed-to-know. The paper's claim concerns the way Lean is symbolically positioned, not the ontology of the software.

## 5. Hardwig: rational epistemic dependence

John Hardwig, “Epistemic Dependence,” *The Journal of Philosophy* 82(7) (1985), 335–349.

Key arguments and page locations:
- pp. 335–338: a layperson's reason for believing p may consist in good reason to believe that an expert has good reasons for p; the layperson may not possess or understand the expert's evidence.
- pp. 338–340: expertise is grounded in sustained, prolonged, systematic inquiry; epistemic individualism is an unrealistic ideal in complex knowledge societies.
- pp. 340–343: chains of expert authority can be extended and refined; rational deference is sometimes appropriate, while conflicts of expert opinion and bad-faith or incompetent experts remain genuine problems.
- pp. 344–349: Hardwig considers whether knowledge can be held vicariously and whether the scientific community, rather than an isolated individual, may be the knower. His particle-physics example makes the collective division of epistemic labour explicit (pp. 346–349).

**What Hardwig already explains:** why ordinary people can rationally trust scientific claims they cannot personally verify; why even scientists depend on other experts; and why collective research can produce knowledge no individual possesses in full.

**What Hardwig does not set out to explain:** why one particular technical object becomes a symbolic embodiment of certainty, how collective epistemic labour may be fetishized as an autonomous machine property, or how a social order sustains the fantasy of a final guarantor.

**Role in this paper:** a normative baseline and a necessary alternative explanation. If a public audience trusts Lean because it has good reason to trust the relevant experts and institutions, this may be rational epistemic dependence, not ideological fetishism. Žižek must explain the additional symbolic function, not relabel justified reliance as ideology.

## 6. De Millo, Lipton, and Perlis: the social process of proof

Richard A. De Millo, Richard J. Lipton, and Alan J. Perlis, “Social Processes and Proofs of Theorems and Programs,” *Communications of the ACM* 22(5) (1979), 271–280.

Key arguments in the original paper (the accessible scan has internal pagination 202–211):
- journal pp. 275–278 (scan's internal pp. 206–209): mathematical theorems become believed through reading, refereeing, discussion, internalization, paraphrase, generalization, use, and connections to other results.
- journal pp. 278–280 (scan's internal pp. 209–211): the authors argue that proofs of real software specifications are often too long and specialized to undergo the social processes that make mathematical proofs believable.
- The paper distinguishes formal derivational correctness from the social assimilation of a proof by a community.

**What it already explains:** mathematical acceptance is not reducible to a formal derivation; communal scrutiny and assimilation play an epistemic role.

**What it does not establish for contemporary Lean:** it predates modern small-kernel proof assistants and does not directly analyze machine-checked proof terms, AI-generated mathematics, or public trust in Lean. Its claim that program proofs would not be read or socially assimilated should not be treated as a blanket refutation of modern proof assistants. Lean can provide a machine-checking guarantee without requiring a human to inspect every proof step; human mathematical understanding and social acceptance remain distinct questions.

**Role in this paper:** historical social-epistemological precursor and a counterweight to technological solutionism. Our contribution is not simply that proofs have social lives; it is the Žižekian account of the symbolic function that a visible checking procedure can acquire in society.

## 7. Fetzer: formal verification and representational correspondence

James H. Fetzer, “Program Verification: The Very Idea,” *Communications of the ACM* 31(9) (1988), 1048–1063.

Fetzer distinguishes formal relations among symbols from the relation between a formal representation and the causal object it is meant to represent. The argument concerns the gap between an algorithmic specification and actual program behaviour.

**Role in this paper:** conceptual background for the need to distinguish formal proof validity from the meaning and application of the formal statement. Do not transfer Fetzer's conclusion about program behaviour wholesale to pure mathematical theorem proving. The relevant analogy must be argued, not assumed.

## 8. Kallel and El Louadi: the closest 2026 prior contribution

Maher Kallel and Mohamed El Louadi, “Verification Abundance, Adjudication Scarcity: What Happens to Mathematical Knowledge When Proof Checking Becomes Free,” arXiv:2608.28997v1 (29 August 2026).

Key arguments:
- Section 2: the three-layer distinction (L1 derivational validity, L2 representational fidelity, L3 epistemic significance).
- Section 3: the argument about why L2 depends on expert judgement, including a grounding-regress argument and a reconstruction of the 1979–1988 De Millo/Fetzer debate.
- Section 4: a six-category taxonomy of representational mismatch.
- Section 5: measurements of the OpenAI ten-proofs corpus and the statement-audit surface.
- Section 6: the inversion from verification abundance to adjudication scarcity.
- Section 7: engineering responses and what they do not reach; Sections 8–9 discuss transfer and remedies.

**What it already explains:** the distinction between derivational validity, representational fidelity, and epistemic significance; the scarcity of qualified human adjudication; the fact that formal checking does not settle the intended meaning of the theorem.

**What is distinctive in its approach:** it treats the problem as an epistemic economy with different scaling behaviour and supplies an audit taxonomy and disclosure schema. This is a close and substantive prior contribution, not a peripheral citation.

**What remains open for our paper:** how Lean verification becomes a public and institutional symbol of scientific certainty; how this credential is framed by companies, universities, mathematical communities, and media; why it may attract the symbolic investment of a wider society; and how a Žižekian account of fantasy, fetishism, and the barred Big Other explains this social function.

**Critical engagement:** Kallel and El Louadi argue that L2 is not mechanizable in principle, drawing on Fetzer's grounding regress. We should acknowledge the force of their point about the need for some extra-formal grounding judgement, while distinguishing it from the stronger claim that tools can never assist semantic comparison or constrain interpretations. Their own taxonomy shows that human adjudication can be structured and supported by engineering. Our paper does not need to settle the general mechanizability thesis to develop its ideological argument.

## 9. Public trust research: empirical background, not our theory

Iordanou, Antoniou, and De Vos, “Public Trust in Science: A Systematic Literature Review,” *Journal of Academic Ethics* 24 (2026), article 56. DOI: https://doi.org/10.1007/s10805-026-09732-5.

The review synthesizes 124 empirical studies and organizes factors into receiver, message, and source categories. It emphasizes integrity, transparency, epistemic inclusion, prior beliefs, values, and communication channels. It defines public epistemic trust as reliance on scientific knowledge without first-hand access to the methods that produce it, while retaining the importance of warranted scepticism.

**Role:** establish the contemporary empirical landscape and prevent a simplistic account in which one technical signal alone explains public trust. The paper's originality is not a new general theory of public trust.

## 10. Comparative synthesis: what each literature contributes

| Literature | Main question answered | What it leaves for our project |
|---|---|---|
| Žižek | How fantasy and fetishistic forms organize social reality and the symbolic function of guarantees | Apply this to Lean's social authority and the desire for scientific certainty |
| Marx | How social relations of labour appear as properties/relations of things under commodity form | Structural analogy for collective epistemic labour appearing as machine autonomy |
| Lacan | How a knowing position is attributed in transference; why the symbolic order has no final guarantee | Carefully limited analysis of Lean's symbolic positioning |
| Hardwig | Why dependence on experts and communities can be rational | Why a particular technical credential acquires symbolic authority beyond warranted dependence |
| De Millo et al. | Why mathematical belief and acceptance involve social processes | How modern formal checking is represented as a public credential and potentially fetishized |
| Fetzer | Why formal verification does not itself establish the represented object's behaviour | Context for the formal/semantic distinction, not the main originality |
| Kallel & El Louadi | Why L1 checking does not settle L2 fidelity or L3 significance; adjudication scarcity | The public, symbolic, and ideological function of the verification credential |
| Public-trust research | Which sources, messages, and receiver factors shape trust in science | A Žižekian account of why a technical verification signal may serve as a symbolic guarantee |

## 11. Novelty statement for the manuscript

The defensible novelty claim is:

**This paper develops a Žižekian account of the social authority of Lean verification. It explains how a bounded and genuine technical guarantee can become a symbolic credential of scientific certainty; how collective epistemic labour may be represented as an autonomous property of the machine; and how this credential may support a fantasy of final guarantee within a symbolic order that, in Lacanian terms, has no final guarantor.**

The paper does not claim that all public trust is ideological, that Lean is unreliable, that formal/semantic distinctions are new, or that the social character of proof has not previously been studied. Its contribution is the specific ideological analysis of the public life of Lean verification.
## 12. Additional close literature on Žižek, technology, disavowal, and artificial epistemic authority

### 12.1 Matthew Flisfeder (2023): a direct guide to the Žižekian framework

Matthew Flisfeder, “There is no metalanguage; or, Truth has the structure of a fiction: The Žižekian system, between post-ideology and post-truth,” *Enrahonar* 70 (2023), 171–185. DOI: https://doi.org/10.5565/rev/enrahonar.1420.

This article is especially useful because its section structure directly covers the Big Other, the perverse form of cynical ideology, commodity fetishism as the material correlate of ideology, and truth's fictional structure. Flisfeder argues that apparent disbelief in the Big Other does not mean that its symbolic function has disappeared; its operation can persist beneath an explicit post-ideological stance. This helps our project avoid treating public actors' explicit caveats as proof that symbolic authority is absent.

**Role:** contemporary theoretical guide to Žižek, not an application to Lean or machine-checked proofs. Our contribution must be the specific application to the bounded epistemic warrant of proof assistants in scientific knowledge production.

### 12.2 Daniel Hourigan (2009): Žižekian critique of technology and knowledge-production

Daniel Hourigan, *The Phantasmatic Subject of Technology: Slavoj Žižek, Techne, and the Abyss*, PhD thesis, Griffith University (submitted 29 August 2008; repository record published 2009). DOI: https://doi.org/10.25904/1912/3124. Repository: https://research-repository.griffith.edu.au/handle/10072/365491.

Hourigan directly uses Žižek to examine technological fetishization, technological phantasia, the symbolic order of technicity, and the ideology of knowledge-production. The thesis argues that technology can be fetishized as an autonomous order that overdetermines the subject and covers over the contingency and social relations of knowledge-production.

**Novelty consequence:** we cannot claim to be the first to apply Žižek's ideology critique to technology, technological fetishism, or knowledge-production. Our distinction is narrower and more specific: the formal proof assistant as an epistemic apparatus; the difference between its exact kernel-level warrant and the broader scientific claims it may be made to authorize; and the role of theorem statements, proof artifacts, expert validation, and public communication in this process.

### 12.3 Jack Black (2025): distinguishing cynical and fetishistic disavowal

Jack Black, “Examining the Mechanism of Disavowal and Its Two Forms: Cynical Disavowal and Fetishistic Disavowal,” *Theory & Psychology* 35(1) (2025), 117–135. DOI: https://doi.org/10.1177/09593543241308199. Open full text: https://shura.shu.ac.uk/34730/.

Black argues that cynical disavowal and fetishistic disavowal should not be collapsed. Cynical disavowal maintains a manipulative distance and obscures the gap between belief and action; fetishistic disavowal can acknowledge the objective state of affairs while preserving the fetishistic attachment that manages the lack in the Other. Black explicitly discusses the way fetishistic disavowal can coexist with knowledge of the lack rather than simply conceal it.

**Role:** refine our coding of the paper's central phenomenon. If an actor states that Lean's verification is limited but continues to invest it with a wider guarantee, this should not automatically be coded as cynical ideology. Depending on the evidence, fetishistic disavowal may be the more precise hypothesis. Cynical disavowal requires evidence of a different relation between acknowledged knowledge, distance, and practice. The distinction should be tested rather than assumed.

### 12.4 Rico Hauswald (2025): artificial epistemic authorities

Rico Hauswald, “Artificial Epistemic Authorities,” *Social Epistemology* 39(6) (2025), 716–725. DOI: https://doi.org/10.1080/02691728.2025.2449602.

Hauswald asks whether AI systems can be epistemic authorities despite lacking beliefs and communicative intentions in the standard testimonial model. He proposes a functional account: subjects defer to an authority by treating suitable facts about it as reliable indicators of the truth of propositions. His account can accommodate AI systems as well as non-testimonial deference to scientific communities and institutions. He also identifies the identification problem (how to recognize reliable authorities) and the deference problem (what epistemic stance is appropriate).

**Role:** close social-epistemological comparator. It already addresses AI as epistemic authority and deference to groups/institutions. Our paper does not need to re-argue whether Lean or AI qualifies as an epistemic authority. Instead, it asks how a particular technical form of authority—formal verification—can be ideologically invested with a guarantee beyond its domain-specific warrant.

## 13. Revised novelty boundary

The additional literature makes the originality claim more precise:

- Not the first Žižekian critique of technology: Hourigan already provides a substantial Žižekian analysis of technological fetishization and knowledge-production.
- Not a new general theory of AI epistemic authority: Hauswald directly analyzes artificial epistemic authorities and non-testimonial deference.
- Not the first account of cynical or fetishistic disavowal: Black (2025) explicitly distinguishes these mechanisms.
- Not the first account of social trust in science, expert dependence, or the social acceptance of proof: Hardwig, De Millo et al., and the public-trust literature already address these topics.

**Our proposed contribution is the intersection:** a Žižekian analysis of formal proof verification as a specific epistemic and institutional practice in contemporary science. The paper explains how the kernel's genuine but bounded reliability may be transformed into a symbolic guarantee of broader scientific certainty; how the collective epistemic labour behind that reliability may be displaced into the apparent autonomy of the checker; and how fetishistic or cynical forms of disavowal may sustain this symbolic investment.

The four Lean cases are not merely examples of AI authority. They allow us to inspect the precise relation among (i) the proposition actually formalized, (ii) the proof artifact checked, (iii) the human and institutional work that connects it to an intended scientific claim, and (iv) the public authority attributed to “Lean-verified.” This artifact-level specificity is the empirical distinction of the project.