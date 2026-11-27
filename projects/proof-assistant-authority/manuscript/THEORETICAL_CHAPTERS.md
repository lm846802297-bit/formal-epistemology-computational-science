# Theoretical chapters — In Lean We Trust?

**Subtitle:** The Ideology of Machine-Checked Proofs in Science  
**Status:** substantive working draft; source-checked conceptual structure, not final journal prose.  
**Theoretical centre:** Slavoj Žižek's critique of ideology, grounded in Marx and Lacan.

# 2. Ideological Fantasy and the Social Demand for Scientific Certainty

## 2.1 Scientific knowledge and the problem of social mediation

Modern scientific knowledge is not ordinarily available for direct inspection by everyone who relies on it. The public encounters scientific claims through a division of cognitive labour: researchers produce results; specialists assess methods and evidence; institutions organize review and accountability; and communicators translate technical claims into public forms. This dependence is not itself an epistemic defect. It is a structural condition of modern science.

The difficulty is that the social reach of scientific claims exceeds the circle of those able to evaluate them directly. Citizens must often make decisions on the basis of claims whose evidential grounds they cannot personally reproduce. The question is therefore not simply whether a claim is true, but how its reliability becomes publicly legible to people who cannot independently inspect its production.

Lean enters this situation as a distinctive technical practice. It converts a proof into a formal object and checks whether that object establishes a specified proposition within a formal environment. This is a genuine achievement. The philosophical question begins when this bounded achievement circulates as a public sign of scientific reliability: what does the sign come to mean, and what social expectations are attached to it?

## 2.2 Žižek: ideology is not simply a false belief

In *The Sublime Object of Ideology*, Žižek rejects an account of ideology limited to mistaken representations that could be corrected by supplying more accurate information. Ideology is also bound up with the symbolic and fantasmatic coordinates through which social reality is organized and made livable. Fantasy does not merely decorate an already complete reality; it helps structure how subjects relate to social antagonisms, gaps, and inconsistencies.

This point matters for the study of formal verification. The argument is not that the public falsely believes Lean proves empirical facts, nor that people are simply ignorant of formal methods. Rather, a public representation of machine checking may help organize the relation between society and the opacity of specialized knowledge. It can stage a scene in which a complex claim appears to pass through a reproducible procedure and emerge as certified.

Fantasy here should not be reduced to wishful thinking, optimism about technology, or a conscious desire for absolute certainty. It concerns the narrative and practical coordinates through which a social demand for reliable knowledge is given a recognizable form.

## 2.3 The fantasy of verification

We propose the term **ideological fantasy of verification** for the possibility that a bounded formal check is represented as if it closed the uncertainty of scientific knowledge more generally.

The kernel's verdict is precise: a proof term is accepted for a formal proposition under specified definitions, axioms, libraries, and computational assumptions. Yet public narratives may move from this local result to broader formulations such as “the problem is solved,” “the result is certain,” or “the machine has verified the science.” Whether such formulations are warranted depends on additional relations: whether the formal proposition captures the intended claim, whether the hypotheses are appropriate, what the result contributes, and what forms of expert and institutional assessment have occurred.

The fantasy does not need to deny the real success of the kernel. On the contrary, its force may depend on that success. A genuine and reproducible check can serve as the material support for a wider image of certainty. The ideological question is whether the formal guarantee is allowed to stand for a guarantee at levels it does not itself reach.

## 2.4 Why a technical guarantee is socially attractive

Formal verification has features that make it publicly legible: it is reproducible, rule-governed, machine-checkable, and apparently less dependent on an individual reader's judgment than an informal proof. These properties can make it an attractive credential in a society where scientific claims are difficult to inspect directly.

At least four functions should be distinguished:

1. **Cognitive legibility:** a complicated process is represented by a concise verdict such as “Lean-verified.”
2. **Procedural reassurance:** a public audience is shown that a specified checking procedure has been carried out.
3. **Institutional legitimation:** organizations can point to a formal artifact as evidence of rigor and accountability.
4. **Symbolic closure:** the language of verification may suggest that a question has been settled, even when semantic, interpretive, or institutional questions remain open.

The first three functions can be legitimate. The fourth becomes ideologically significant when the symbolic closure exceeds the actual warrant. The paper must therefore distinguish a warranted public credential from its possible enlargement.

## 2.5 The fantasy is tested, not presumed

The four Lean cases provide contrasting tests. The Riemann case asks whether extensive machine checking can be narrated as equivalent to human mathematical understanding. The Navier–Stokes case asks whether kernel acceptance can be treated as certification of a separate written proof despite a disputed correspondence. The Erdős case tests a workflow in which statement validation and expert review are explicitly described. The Liquid Tensor Experiment provides a historical case in which expert confidence was tied to human mathematical interaction as well as Lean.

Evidence for ideological fantasy would include recurring public formulations of verification as final closure, especially where the primary sources preserve unresolved semantic or interpretive conditions. Evidence against the hypothesis would include careful communication that states exactly what was checked and retains the role of human judgment. A single headline is not enough to establish an ideological mechanism.

## 2.6 Interim claim

Lean does not create the social demand for reliable knowledge, and its technical success should not be treated as an illusion. The hypothesis is that Lean can give this demand a visible technical form. A Žižekian analysis asks why this form can acquire the symbolic force of a guarantee and when that force exceeds the formal result.

# 3. From Marx's Commodity Fetishism to the Epistemic Fetishism of Lean

## 3.1 Marx: the social relation takes the form of a relation between things

In Chapter 1, Section 4 of *Capital*, Marx analyzes commodity fetishism as a feature of the social form of commodity production. The social character of labour appears not as a direct relation among producers, but as a relation among products. The commodity seems to possess value as a natural property, while the social relations that constitute value are obscured.

The point is not simply that people mistakenly admire objects. The appearance is generated by the organization of social practice itself. The commodity form makes social relations appear in an objectified form.

Žižek's use of fetishism is informed by this Marxian structure and by Lacanian disavowal. For the present paper, the important question is whether the authority of machine verification can similarly appear as a property of the machine, although it depends on a distributed social process.

## 3.2 The collective labour behind a Lean-checked result

A Lean-verified result is not produced by a kernel in isolation. Its epistemic force depends on a network of activities:

- researchers choose a problem and formulate the intended claim;
- mathematicians develop definitions, lemmas, and proof strategies;
- formalizers translate mathematical reasoning into a formal language;
- library contributors supply reusable definitions and theorems;
- Lean developers maintain the language, kernel, elaborator, compiler, and infrastructure;
- experts assess whether the formal statement corresponds to the intended mathematics;
- research communities assess novelty, significance, and relation to prior work;
- institutions and communicators establish how the result is presented and understood.

AI may participate in several of these tasks, but it does not remove the need to identify them. In some projects, human contribution is extensive and explicit; in others, the public narrative foregrounds the model or the proof assistant.

## 3.3 Epistemic fetishism of Lean verification

We propose **epistemic fetishism of Lean verification** as an analytic extension of the Marxian-Žižekian account of fetishism. It names a representational displacement in which the reliability produced by collective epistemic labour appears as an autonomous property of Lean itself.

The compressed statement “Lean verified the result” can be entirely accurate when it refers to a specified formal proposition. It becomes fetishistic only if the machine is represented as self-sufficient source of the broader authority, while the human, semantic, and institutional relations that make the check relevant recede from view.

This distinction is essential. Naming Lean as the checker is not fetishism. A headline is not fetishism simply because it is short. The analysis must show (i) the actual network of labour and mediation, (ii) how a public representation allocates authority, and (iii) whether necessary conditions of the check's relevance are displaced.

## 3.4 Why this is more than automation bias

Automation bias usually concerns a tendency to over-rely on automated outputs or to defer to them in decision-making. The proposed fetishism concept asks a different question. It examines how a social relation of knowledge production is represented as an intrinsic property of a technical object.

The distinction is between an individual's cognitive error and a socially organized appearance. A person may rationally rely on Lean because the kernel has a well-understood checking role. Fetishism becomes relevant when the authority of the wider knowledge network is condensed into the machine as if the machine independently generated the reliability attributed to the whole result.

## 3.5 The four Lean cases as contrasts

**Riemann:** the public phrase “Claude and Lean proved RH” can foreground machine agency. A complete analysis must restore the mathematician's direction, formalization work, Mathlib infrastructure, independent checker work, and the distinction between formal certification and human understanding. The extensive independent checking is real and should not be demystified away.

**Navier–Stokes:** this is the strongest candidate for analyzing fetishistic displacement. Lean's kernel may validly check the declarations in the repository, while the relation between those declarations and the natural-language paper is separately disputed. If the authority of the kernel is treated as sufficient to settle the source-text correspondence, the machine's local authority has been made to stand for a relation it does not itself establish.

**Erdős:** the *Science* paper describes the formalized benchmark, Lean checking, and human validation of statement correspondence. This visibility of mediation may resist a fetishistic reading, even if some headlines compress the workflow.

**Liquid Tensor:** the primary project record credits mathematicians, formalizers, Mathlib, and institutional support. Scholze's account emphasizes human mathematical interaction. This is a counter-case in which the collective basis of confidence remains visible.

## 3.6 Interim claim

The proposed concept does not accuse mathematicians of irrationality or deny the reliability of Lean. It identifies a possible social appearance: collective epistemic labour can be condensed into the machine as an apparently autonomous bearer of certainty. The case studies must determine where this appearance occurs and where public accounts resist it.

# 4. The Big Other Does Not Exist: Lean and the Demand for a Technical Guarantee

## 4.1 The Big Other is not a super-expert

In Lacanian theory, the Big Other is not a person, a machine, or a real institution that possesses complete knowledge. It names the symbolic locus of language, law, norms, and the presumed consistency of the social order. The formula that “there is no Other of the Other” denies the existence of a final meta-guarantor that could certify the symbolic order from outside.

Žižek uses this lack to explain why social practices can nevertheless function as if a complete guarantee were available. The point is not that people literally believe in an omniscient institution. It is that authority and meaning are organized through symbolic coordinates that are treated as if they ultimately hold.

Consequently, this paper must not claim that Lean is the Big Other. Lean is a technical system with a specific formal role. The relevant hypothesis is that Lean can be positioned as a visible credential within a symbolic order that seeks a guarantee of scientific knowledge.

## 4.2 The technical checker as a symbolic credential

Lean's kernel has a sharply delimited function. Given a formal proposition and a proof term, it checks whether the term has the required type in the formal environment. This is an unusually powerful and reproducible form of assurance.

Yet the public significance of a Lean result depends on questions beyond the kernel: whether the proposition expresses the intended theorem, whether the theorem's assumptions are appropriate, whether the result is novel, whether it has been understood, and how it bears on the scientific world. No checker can, by itself, answer all of these questions.

Lean may nevertheless be presented as a credential that condenses this wider process. Its output can be invoked as if the social order of scientific knowledge had found a technical point at which uncertainty is finally settled.

## 4.3 The paradox of the missing guarantor

The Big Other does not exist as a complete and consistent authority. There is no final institution, expert, proof assistant, or meta-system that can guarantee every link in the production and interpretation of scientific knowledge. Any further checker would itself depend on a formal specification, an implementation, a trust base, and human judgments about relevance.

This does not lead to relativism. It does not imply that all claims are equally uncertain or that formal verification is futile. It means that guarantees are local, situated, and mediated. Lean can provide a strong guarantee about a formal derivation without becoming a guarantee of the entire social and scientific process.

The ideological question is how a local guarantee can be made to function as if it were a final one. The symbolic force of the machine lies not in its omniscience but in its capacity to represent, in a visible and reproducible form, the possibility of a guarantee.

## 4.4 The subject-supposed-to-know and the attribution of authority

The subject-supposed-to-know is related to the Big Other but should not be collapsed into it. In Lacan's account of transference, knowledge is attributed to a position; the analyst is supposed to know. Applied cautiously, this concept can help analyze how a knowing position is attributed to experts, institutions, or technical systems.

Lean itself is not a psychoanalytic subject and does not know in the human sense. The question is whether public discourse attributes to Lean a position of epistemic authority: not simply that it checks a proof, but that it is treated as the place where the truth of a claim is settled.

The primary object of analysis is therefore the social attribution of knowledge, not the mental state of the software or the unconscious motives of individual users.

## 4.5 The four Lean cases

Riemann tests whether the checker becomes a symbolic guarantee when the formal proof is highly certified but not yet fully understood by mathematicians. Navier–Stokes tests whether the checker is treated as guarantor of a natural-language claim whose correspondence to the formal declarations is disputed. Erdős tests whether visible expert validation prevents Lean from being cast as a self-sufficient authority. Liquid Tensor tests whether the guarantee is instead located in a human-machine community of mathematical scrutiny.

These cases do not establish that the public uniformly treats Lean as a final authority. They allow the paper to identify the conditions under which such an attribution becomes plausible.

## 4.6 Interim claim

Lean is not the Big Other. It can, however, become one of the technical signs through which a scientific symbolic order stages the existence of a reliable guarantor. The ideological contradiction is that the formal checker offers a real but local guarantee, while the social demand may be for a complete guarantee that no system can provide.

# 5. Synthesis: the symbolic guarantee and the relocation of uncertainty

The three mechanisms form a connected but non-identical argument:

1. **Fantasy** explains why a visible verification procedure can stage the closure of uncertainty.
2. **Fetishism** explains how the collective labour that makes verification meaningful can appear as a property of the machine.
3. **The Big Other** explains why the machine can be positioned as a guarantor within a symbolic order, even though no final guarantor exists.

The central proposition is:

**Verification does not abolish uncertainty; it relocates uncertainty.**

Lean can sharply reduce uncertainty about whether a proof term establishes a specified formal proposition. It does not by itself settle semantic correspondence, the appropriateness of assumptions, mathematical understanding, novelty, institutional recognition, or public interpretation. The stronger the technical credential becomes, the more important these other forms of mediation may become.

The paper's original contribution is therefore not the familiar observation that formal proof checking has limits. It is a Žižekian account of how a bounded and genuinely reliable technical guarantee can acquire a wider symbolic function in society: it can support a fantasy of certainty, condense collective epistemic labour into a machine object, and occupy the place of a guarantor that the symbolic order cannot ultimately supply.
# References for the theoretical chapters

## Primary philosophical texts

- Lacan, Jacques. *The Seminar, Book XI: The Four Fundamental Concepts of Psychoanalysis*. Trans. Alan Sheridan. New York: W. W. Norton, 1977. Especially the sessions on transference and the subject supposed to know.
- Lacan, Jacques. “Proposition of 9 October 1967 on the Psychoanalyst of the School.” Use a scholarly edition/translation and verify pagination before final submission.
- Marx, Karl. *Capital: A Critique of Political Economy*, Vol. 1. Trans. Ben Fowkes. London: Penguin, 1976. Chapter 1, Section 4, “The Fetishism of the Commodity and Its Secret.”
- Žižek, Slavoj. *The Sublime Object of Ideology*. London: Verso, 1989. Especially the opening chapter on ideology and fantasy; check page references against the edition actually cited.
- Žižek, Slavoj, ed. *Mapping Ideology*. London: Verso, 1994. Especially Žižek's “The Spectre of Ideology.”
- Žižek, Slavoj. *The Plague of Fantasies*. London: Verso, 1997. Relevant for fantasy as a structuring frame rather than a merely imaginary supplement.

## Prior work that sets the novelty boundary

- De Millo, Richard A., Richard J. Lipton, and Alan J. Perlis. “Social Processes and Proofs of Theorems and Programs.” *Communications of the ACM* 22, no. 5 (1979): 271–280. https://doi.org/10.1145/359104.359106.
- Fetzer, James H. “Program Verification: The Very Idea.” *Communications of the ACM* 31, no. 9 (1988): 1048–1063. https://doi.org/10.1145/48529.48530.
- Hardwig, John. “Epistemic Dependence.” *The Journal of Philosophy* 82, no. 7 (1985): 335–349. https://www.jstor.org/stable/2026523.
- Kallel, Maher, and Mohamed El Louadi. “Verification Abundance, Adjudication Scarcity: What Happens to Mathematical Knowledge When Proof Checking Becomes Free.” arXiv:2608.28997 (2026). https://arxiv.org/abs/2608.28997.
- Iordanou, Kalypso, Antonis Antoniou, and Maura De Vos. “Public Trust in Science: A Systematic Literature Review.” *Journal of Academic Ethics* 24 (2026), article 56. https://doi.org/10.1007/s10805-026-09732-5.
- Hourigan, Daniel. *The Phantasmatic Subject of Technology: Slavoj Žižek, Techne, and the Abyss*. PhD thesis, Griffith University, 2009. https://doi.org/10.25904/1912/3124.

## Citation and conceptual checks before submission

1. Verify all quotations and page numbers directly against the cited editions of Marx, Lacan, and Žižek. The present draft paraphrases rather than quotes them.
2. Do not attribute the phrase “epistemic fetishism of Lean verification” to Žižek. It is the paper's proposed analytic extension of Marxian/Žižekian fetishism.
3. Do not write that Lean “is” the Big Other. The argument concerns its possible symbolic positioning as a credential within an order that seeks a guarantee.
4. Keep the distinction between the subject-supposed-to-know and the Big Other. The former concerns transference and attribution of knowledge; the latter names the symbolic locus/order.
5. Do not claim that the three mechanisms have been empirically demonstrated merely because the theoretical vocabulary has been applied. Each requires the case evidence specified in the preceding chapters.