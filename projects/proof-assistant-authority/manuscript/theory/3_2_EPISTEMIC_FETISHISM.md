# 3.2 From Commodity Fetishism to the Epistemic Fetishism of Formal Verification

**Status:** theory-chapter research draft; the central concept is the paper's proposed extension, not a term coined by Marx or Žižek.

## 1. The problem of the apparent autonomy of the machine

When a public account says that “Lean verified the proof,” it may state something perfectly accurate. Lean does check formal proof terms against formal propositions. The philosophical question is not whether this technical statement is true. It is how the authority associated with the check is socially produced, and whether that authority can come to appear as a self-contained property of the machine.

A Lean-checked theorem is the outcome of a distributed process. Researchers select a problem and formulate an intended claim. Mathematicians develop definitions and arguments. Formalizers encode the statement and proof. Library maintainers provide a large body of formalized mathematics. Software developers maintain the kernel, elaborator, compiler, and infrastructure. Experts assess whether the formal statement corresponds to the intended mathematics. Institutions and journals evaluate significance and responsibility. Communicators translate the result for wider audiences.

The reliability of the result depends on this network, although different participants contribute in different ways. The kernel's checking is real, but the kernel does not independently choose the problem, formulate its intended meaning, establish its novelty, or decide what the result means for a scientific field.

The proposed concept of **epistemic fetishism of formal verification** concerns the possible displacement through which the reliability produced by this network appears as an autonomous property of Lean itself.

## 2. Marx: the commodity form and the appearance of social relations

In *Capital*, Volume I, Chapter 1, Section 4, “The Fetishism of Commodities and the Secret Thereof,” Marx analyzes a historically specific form of social appearance. Under capitalist commodity production, the social character of labour appears as an objective property of the products of labour, while relations among producers appear as relations among things. The point is not merely that people forget the workers who made an object. The commodity form organizes the appearance of social relations in a particular way.

Žižek's discussion in *The Sublime Object of Ideology*, Chapter 1, pp. 19–20 of the 1989 Verso edition, emphasizes the structural dimension of this appearance: an effect produced by a network of relations can be misrecognized as an immediate property of one element within that network. The analysis therefore concerns the form through which a social relation becomes effective and appears.

The present paper borrows this structure, not Marx's entire theory of capitalist value. Lean is not a commodity in the technical Marxian sense, and formal verification is not exchange-value. The analogy is narrower: a collectively produced epistemic capacity may appear as if it were an intrinsic and autonomous property of a technical object.

## 3. The proposed extension: epistemic fetishism

**Epistemic fetishism of formal verification occurs when the socially produced reliability of a machine-checked result is represented as an autonomous property of the machine, while the human, semantic, and institutional relations that make the check relevant recede from view.**

The concept has four components:

1. **A real technical capacity:** Lean genuinely checks formal proof terms against formal propositions.
2. **A collective production network:** the result depends on theorem selection, formalization, libraries, software, expert interpretation, and institutional review.
3. **A representational displacement:** public or institutional discourse attributes the resulting authority primarily to the machine as if it possessed that authority independently.
4. **A scope consequence:** the machine's technical property may be treated as if it guaranteed a broader scientific claim than the formal artifact establishes.

The fourth component is important but not strictly necessary for every instance of fetishism. A representation can fetishize the machine's authority even while accurately describing the proposition checked. The stronger and more consequential case occurs when the autonomous machine image also carries a wider guarantee than the technical result warrants.

## 4. Why this is not simply a criticism of headlines

A headline that says “Lean verifies the theorem” is not, by itself, evidence of epistemic fetishism. It may be an accurate shorthand, especially if the accompanying text identifies the exact formal theorem, assumptions, human contributors, and review status. The concept requires more than the use of a machine-centred phrase.

The analysis must reconstruct the collective process and then compare it with the public representation. It must show which relations are necessary for the result's relevance and whether those relations are foregrounded, backgrounded, or omitted. It must also compare cases in which the human and institutional network is made visible.

This is why the Liquid Tensor Experiment is an important counter-case. Its completion announcement names the mathematicians, formalizers, Mathlib dependencies, and institutional support. Scholze's contemporaneous comments emphasize that his confidence arose from human mathematical interaction and scrutiny, not from the computer alone. Such a record may resist the autonomous-machine representation.

The Navier–Stokes case provides a different test. Lean's kernel may validly check the formal declarations, while an independent critique disputes whether some of those declarations faithfully correspond to the separate natural-language proof. If the public credential “Lean-verified” is allowed to stand for the correctness of the entire written paper, the technical authority of the kernel can displace the semantic and human work needed to establish that connection.

## 5. Four empirical indicators

The concept should be coded only where evidence supports the following sequence:

- **Network reconstruction:** identify the actual human, technical, and institutional relations on which the result depends.
- **Authority attribution:** determine which actors or objects are represented as the source of reliability.
- **Visibility of mediation:** establish whether theorem formulation, formalization, semantic validation, and review are visible or recede from view.
- **Scope of the public claim:** compare the claim made in public with the proposition and proof actually checked.

A strong instance would show that the public narrative presents Lean as an autonomous guarantor while obscuring necessary human and semantic mediation. A weak instance would simply mention Lean as one component of a transparent collaborative process.

## 6. The relation to Žižek

Žižek's account of fetishism is useful because it does not reduce ideology to an incorrect belief about an object. It asks how a social relation can appear in an object-form and how that appearance can organize practice. The proposed epistemic extension therefore shifts the analysis from “people overestimate the software” to “the social authority produced by a network is represented in the form of machine autonomy.”

The distinction is decisive. A user may know that a formalization required extensive human work and still rely on Lean for the limited checking task it performs. That is not automatically fetishism. The ideological question is whether the social representation of the result makes the machine appear to possess an independent guarantee that conceals the relations on which the guarantee depends.

## 7. Provisional thesis

**The epistemic fetishism of formal verification is not the worship of a machine and not the denial of its technical reliability. It is a form of social appearance in which the collective production of epistemic warrant is condensed into the seemingly autonomous authority of the checker.**

This is the paper's proposed conceptual extension. Its validity depends on whether the four Lean cases demonstrate a recurring representational structure rather than isolated rhetorical shorthand.
