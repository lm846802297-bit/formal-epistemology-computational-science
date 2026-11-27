# Disciplinary Positioning and Conceptual Boundaries

**Project:** *In Lean We Trust? The Ideology of Machine-Checked Proofs in Science*  
**Date:** 27 November 2026  
**Status:** controlling scope and disciplinary-positioning memo. Read together with `REVISED_THEORETICAL_FRAMEWORK.md`.

## 1. Disciplinary location

The most accurate disciplinary description is:

**Philosophy of Science, specifically a critical social- and political-epistemological analysis of scientific knowledge production, using Žižek's critique of ideology.**

The project has four levels of classification:

1. **Primary field — Philosophy of Science.** The object is the epistemic and institutional role of formal verification in contemporary mathematical and scientific knowledge production.
2. **Closest subfield — Social Epistemology of Science.** The project examines distributed epistemic labour, expert dependence, institutional recognition, and the social practices through which claims become accepted as knowledge. The Stanford Encyclopedia of Philosophy characterizes social epistemology in terms of the epistemic effects of social interactions, practices, norms, systems, and collective agents.
3. **Critical orientation — Political Epistemology / Ideology Critique.** The project asks how scientific authority is symbolically organized and how ideological representations of knowledge and certainty operate. Omodeo's *Political Epistemology: The Problem of Ideology in Science Studies* is a relevant disciplinary precedent, although its historical and hegemonic programme is broader than this paper's specific object.
4. **Theoretical method — Žižekian Critique of Ideology.** Žižek supplies the central concepts and explanatory framework: ideological fantasy, fetishism, and disavowal.

Philosophy of Technology and Science and Technology Studies (STS) are adjacent fields. They help situate technical systems within social practices, but they are not the paper's primary disciplinary home.

This is not primarily:
- **Formal Epistemology:** despite the phrase “formal verification,” the paper does not use mathematical or logical models to analyse epistemic justification.
- **Philosophy of Mathematics:** mathematical proof is the principal empirical setting, but the central question concerns the social-symbolic function of formal verification, not the ontology of mathematical objects or the nature of mathematical truth.
- **Philosophy of AI / AI Ethics:** the paper does not ask whether AI is conscious, generally intelligent, or morally responsible.
- **A general sociology of public trust:** population-level trust and causal effects are not the principal dependent variables.

A concise description for abstracts, journal submissions, and academic profiles is:

> **A Žižekian critique of ideology in the social epistemology of scientific knowledge production.**

A more specific description is:

> **A critical social and political epistemology of formal verification in contemporary mathematical science.**

## 2. Why social and political epistemology are both relevant

Social epistemology supplies the field-level question: how do social practices, expert relations, institutions, and divisions of cognitive labour contribute to the production and warrant of knowledge?

Political epistemology supplies the critical question: how are scientific knowledge and its authority embedded in ideological, cultural, and institutional arrangements?

The paper occupies the intersection. It does not adopt a strong constructivist or relativist thesis that scientific truth is merely a product of social power. It accepts the reality of mathematical validity and the genuine technical reliability of Lean's kernel. It investigates how that bounded warrant is represented, mediated, and sometimes enlarged within scientific authority.

Hardwig remains useful as a normative baseline for justified epistemic dependence. His role is to help distinguish warranted reliance on experts and technical systems from the ideological enlargement of a technical credential. He is not a second core theory.

## 3. Why Žižek is the central theoretical framework

The paper is an application of Žižek's critique of ideology, not a general survey of Marx, Lacan, and Hardwig.

The three principal concepts have distinct analytical functions:

### 3.1 Ideological fantasy — the scene of closure

Fantasy structures the scene through which a social practice appears coherent. In this project, the hypothesis is that the formal-verification event can be represented as the point at which scientific uncertainty reaches closure: a complex process culminates in the apparently simple verdict “verified.”

The issue is not that Lean literally claims to verify empirical reality. It is whether the certainty achieved at the formal level is made to symbolize closure at semantic, mathematical, institutional, or scientific levels that the kernel does not itself settle.

### 3.2 Fetishism — the objectal condensation of collective labour

The paper's proposed extension, **the ideological fetishism of formal verification**, applies the Marxian and Žižekian structure of fetishism to a specific epistemic object.

The reliability of a formal result depends on a network of relations: theorem selection, mathematical formulation, formalization, definitions, libraries, software maintenance, kernel checking, semantic comparison, expert scrutiny, institutional recognition, and communication.

The fetishistic hypothesis is that the authority generated through this network can appear as an autonomous property of the machine. The machine becomes the visible object that seems to contain the guarantee, while the collective epistemic labour and relations that make the check meaningful recede from view.

This is a structural analogy with commodity fetishism, not a claim that Lean is a commodity in Marx's technical economic sense.

### 3.3 Disavowal — the persistence of symbolic investment

Disavowal addresses the possibility that the limits of verification are known, yet the technical credential continues to sustain a broader symbolic guarantee.

Jack Black's distinction between cynical and fetishistic disavowal is retained:
- **Fetishistic disavowal:** the limitation can be acknowledged while the fetish object continues to sustain the broader attachment.
- **Cynical disavowal:** a manipulative distance obscures the gap between what an actor knows and what they do.

Neither form may be inferred from a single headline, a vague discrepancy, or the mere fact that a researcher trusts Lean. The evidence must establish the relevant relation between knowledge of the limitation and continued practice.

### 3.4 How the three concepts relate

The three concepts are not a deterministic sequence and should not be treated as unrelated boxes.

- **Fantasy** describes the scene or promise of final certainty.
- **Fetishism** describes how that promise is condensed into the apparently autonomous authority of the technical object.
- **Disavowal** explains how the investment may persist despite acknowledged limitations.

They are mutually reinforcing analytical dimensions of one possible ideological operation.

Marx and Lacan are theoretical sources internal to Žižek's framework. They should not be presented as parallel, co-equal explanatory frameworks. Hardwig remains the normative comparator.

## 4. The central mechanism

The paper distinguishes four analytically separate levels:

1. **Technical warrant:** Lean's kernel checks that a proof term has the required type for a specified formal proposition in a specified environment.
2. **Semantic mediation:** human mathematical judgement connects the formal proposition to the intended theorem or scientific claim.
3. **Institutional mediation:** experts, research groups, journals, universities, and mathematical communities assess correctness, significance, provenance, and acceptance.
4. **Public representation:** institutional announcements and media accounts describe what the result establishes.

The central transition is therefore not automatic:

\[
\text{Local formal warrant}
\;\not\Rightarrow\;
\text{unrestricted scientific certainty}.
\]

The ideological hypothesis concerns the contingent transition:

\[
\begin{aligned}
&\text{Genuine, bounded technical reliability}\\
&\quad+\text{semantic and institutional mediation}\\
&\quad+\text{symbolic/public representation}\\
&\longrightarrow
\text{possible broader guarantee of certainty}.
\end{aligned}
\]

Fetishism becomes a defensible interpretation when the collective relations that produce and interpret the verification appear as an intrinsic, autonomous authority of the machine, and the formal credential is made to perform more epistemic work than its warrant supports.

## 5. Normative distinction: warranted reliance is not fetishism

The paper must preserve the following distinction:

- A researcher may rationally trust Lean to check a formal proof under a specified environment.
- A non-specialist may rationally rely on expert testimony about a machine-checked result.
- An institution may accurately use “Lean-verified” as shorthand for a precisely identified formal proposition.

None of these is, by itself, ideological fetishism.

The critical diagnosis requires an additional mechanism: the formal credential is represented or used as an autonomous guarantee beyond its scope, while the human, semantic, and institutional relations that support its meaning are displaced.

This distinction prevents the paper from treating all trust, all technical reliance, or all scientific authority as ideology.

## 6. Literature and originality boundaries

The following works define the current boundary:

- **Social epistemology:** the Stanford Encyclopedia of Philosophy entry “Social Epistemology” (substantive revision 2024) provides the field-level account of social practices, institutions, and collective agents in knowledge production.
- **Political epistemology:** Pietro Daniel Omodeo, *Political Epistemology: The Problem of Ideology in Science Studies* (Springer, 2019), analyses ideological dimensions of disciplinary discourses on science and the cultural-political conditions of scientific knowledge. It is a broad disciplinary precedent, not an analysis of Lean.
- **Žižek and technology:** Daniel Hourigan, *The Phantasmatic Subject of Technology: Slavoj Žižek, Techne, and the Abyss* (PhD thesis, Griffith University, 2009), directly applies Žižek to technological fetishization, fantasy, and knowledge production. We therefore do not claim to be the first Žižekian critique of technology.
- **Žižek's ideology theory:** Matthew Flisfeder, “There is no metalanguage; or, Truth has the structure of a fiction” (2023), is a contemporary guide to Žižek's Hegelian-Lacanian critique of ideology, fetishism, and disavowal.
- **Disavowal:** Jack Black (2025) distinguishes cynical from fetishistic disavowal. The distinction refines our evidence criteria; it is not our original contribution.
- **Technical epistemic warrant:** Eamon Duede and Kevin Davey (2025), “A Priori Knowledge in an Era of Computational Opacity,” *Philosophy of Science* 92(5), 1394–1404, argue that transparent proof-checkers can provide genuine a priori mathematical knowledge from outputs generated by opaque AI systems. This is an important normative counterweight: the paper does not deny the epistemic value of proof-checking.
- **Formal/semantic adjudication:** Maher Kallel and Mohamed El Louadi (2026), “Verification Abundance, Adjudication Scarcity,” arXiv:2608.28997, distinguish derivational validity, representational fidelity, and epistemic significance. This is close prior work and must be credited; those distinctions are not claimed as original here.
- **Cultural analysis of proof assistants:** Carola Manolino and Cécile Ouvrier-Buffet (2026), “Proof Assistants at the interplay of mathematical cultures,” Research Square preprint, analyse proof assistants as cultural artifacts in higher education. Their educational setting differs from our focus on research authority and scientific communication, but rules out a broad claim that proof assistants have not been studied as cultural practices.
- **Terminological collision:** Kristoffer Ahlstrom-Vij, “Esoteric Reliabilism,” *Episteme* 18(4) (2021), 603–623, uses the phrase “epistemic fetishism” for treating heuristics as fundamental epistemic norms. This is a different concept from our Marxian-Žižekian account of fetishistic displacement. We should consistently use the full phrase **“ideological fetishism of formal verification”** and must not claim to have invented the bare expression “epistemic fetishism.”

**Defensible originality claim:** this paper develops a Žižekian account of how the genuine but bounded warrant of Lean verification can acquire a broader symbolic function in contemporary mathematical and scientific knowledge production; how collective epistemic labour can be displaced into the apparent autonomous authority of the machine; and how that investment may persist despite acknowledged limits.

The paper does not claim to be the first study of technology fetishism, the first social epistemology of proof assistants, the first account of formal/semantic mismatch, or the first use of the phrase “epistemic fetishism.”

## 7. Empirical scope and stopping rule

The four primary Lean cases remain:
1. Riemann hypothesis — technical certification, expert-community authorization, and AI-mediated exposition.
2. Navier–Stokes — formal validity and disputed correspondence with a separate natural-language proof.
3. Erdős / AlphaProof Nexus — formal proof search, statement identity, human validation, and institutional mediation.
4. Liquid Tensor Experiment — visible collective labour and semantic checks as a counter-case.

Waring/GPT may be mentioned only as a brief contrast; it is not a primary Lean case.

The paper does not become a population-level study of trust in AI. It does not infer unconscious motives or audience beliefs from public texts. The evidence supports claims about artifacts, representations, and documented practices; claims about audience uptake require separate audience data.

## 8. Acceptance criteria for this positioning

- The paper is explicitly located in philosophy of science, with a critical social/political-epistemological orientation.
- Žižek is the central theory; Marx and Lacan are theoretical sources within that framework; Hardwig is a normative comparator.
- The technical reliability of Lean is treated as real and bounded.
- Fantasy, fetishism, and disavowal are conceptually distinct and empirically testable.
- The term “epistemic fetishism” is distinguished from Ahlstrom-Vij's different use.
- Prior work on Žižek and technology, proof-assistant epistemology, and cultural practices of proof is acknowledged.
- The four Lean cases and the central question remain unchanged.
