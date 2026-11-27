# The Žižekian model of the ideological fetishism of formal verification

**Project:** *In Lean We Trust?*  
**Date:** 27 November 2026  
**Status:** Controlling model after anonymous referee revision. The object is the public/institutional credential “Lean-verified,” not Lean software in general. The model is conditional and must be tested against counter-evidence.

## 1. Central question and hypothesis

**Central question**

> Under what conditions does the genuine but bounded warrant of Lean verification acquire an ideological function as an apparently self-sufficient guarantee of broader mathematical authority?

**Central hypothesis**

The ideological fetishism of formal verification is the objectal displacement through which the socially and semantically mediated authority of a machine-checked result appears to reside autonomously in the credential “Lean-verified,” allowing the warrant of a bounded formal check to stand for a wider mathematical claim.

This is a proposed Žižekian extension. It is not a diagnosis presumed true of every Lean project.

## 2. The technical baseline: adopt, do not reinvent, warrant architecture

Lean checks whether a proof term has the required type for a specified formal proposition under a specified formal environment. This is genuine technical warrant.

The study adopts, rather than claims as original, the component-based analysis of mathematical warrant developed by Vallverdú (2026) and the distinctions among derivational validity, representational fidelity, and epistemic significance developed by Kallel and El Louadi (2026).

For each case, record:
- intended mathematical claim;
- formal proposition;
- proof object and provenance;
- checking procedure and trusted base;
- axioms, definitions, libraries, and dependencies;
- specification relation between the intended claim and formal proposition;
- allocation of human and computational epistemic functions;
- independent replication or checking routes;
- institutional and public representation.

The kernel’s acceptance of a proof term establishes derivational validity relative to the specified formal environment. It does not, by itself, establish every relation between the formal proposition and the intended mathematical claim. This is not a defect in Lean. It is a distinction between components of the warrant architecture.

## 3. The constitutive gap

Let P be the intended mathematical claim and P* the formal proposition checked by Lean. Kernel acceptance warrants a proof of P* under a specified environment. The relation P ↔ P* is a specification relation and requires its own audit.

This relation can be rigorously assessed through mathematical interpretation, source comparison, formal specification review, independent expert scrutiny, and further formalization where appropriate. The point is not that semantic correspondence is impossible to establish. The point is that checking the proof term and checking the specification relation are different epistemic tasks.

The structural tension relevant to this paper is therefore not “certainty versus uncertainty” in general. It is the non-identity between a formal object and the intended mathematical claim, combined with the practical demand for portable and communicable warrants. A formal certificate can be made to appear as if it closes this relation by itself.

## 4. Derivation from Žižek’s primary texts

### 4.1 Ideology beyond false consciousness

Žižek’s “The Spectre of Ideology” challenges the reduction of ideology to false propositions or distorted representations (Žižek 1994). A proposition may be factually correct and still participate in an ideological relation through the position it occupies and the practice it helps sustain.

Application: “Lean checked this proof” may be entirely accurate. The ideological question is what this statement is made to authorize and whether the credential is made to stand for a wider claim than the formal proposition and documented specification relation warrant.

This does not mean that every true statement is ideological. Nor does it mean that every form of institutional legitimation is fetishistic.

### 4.2 Ideological fantasy: the scene of closure

In *The Sublime Object of Ideology*, fantasy is not merely a false image concealing a complete reality. It provides coordinates through which social reality is experienced and helps sustain an appearance of coherence where a constitutive gap remains (Žižek 1989, 28–31).

The relevant limit in formal verification is not an unbridgeable gap between mathematics and formalization. The specification relation between an intended claim \(P\) and a formal proposition \(P^*\) can be carefully established, and in some settings parts of it can themselves be formalized. The point is that this relation is a distinct epistemic task from checking a proof term for \(P^*\). No single local operation can, merely by being reliable at its own task, serve as the warrant for every other task in the chain.

Application: the local kernel verdict may be staged as the point at which the wider work of specification, interpretation, and institutional assessment appears already complete. Fantasy names this scene of closure. It does not eliminate the specification relation; it makes the labour of establishing that relation appear to have been absorbed into the visible verdict.

Fantasy is not synonymous with rhetorical exaggeration. Its operation must be connected to a social practice or institutional representation that organizes the meaning of the credential.

### 4.3 Fetishism and the formation of the verification credential

The object analyzed here is the public/institutional credential “Lean-verified,” not Lean software in general. Its authority depends on theorem formulation, formal specification, proof construction, libraries, kernel and toolchain maintenance, semantic comparison, expert scrutiny, institutional recognition, and public explanation. These relations do not create mathematical truth in the same way that labour produces commodities. They produce, maintain, check, interpret, and authorize the artifacts and relations through which a formal result is connected to an intended claim.

The formation and reproduction of the epistemic fetish can be reconstructed through five connected moments. This is a Žižekian extension developed for formal verification, not a sequence stated by Žižek himself. The moments are analytically ordered, not a rigid chronology:

1. **Real technical reliability.** The kernel performs a genuine checking operation. It accepts a proof term for a specified formal proposition under a specified environment. Reproducibility and independent checking make this warrant materially credible.
2. **Distributed epistemic labour.** The result depends on problem selection, mathematical formulation, formal specification, proof construction, libraries, software maintenance, trusted infrastructure, semantic comparison, expert assessment, and institutional recognition. These are differentiated contributions distributed across people and systems.
3. **Credential condensation.** Scientific communication condenses this heterogeneous process into the portable status “Lean-verified.” The credential allows a complex result to travel through abstracts, papers, institutional statements, repositories, and public accounts.
4. **Objectal displacement and symbolic authority.** As the credential circulates, the exact proposition, environment, assumptions, dependencies, and specification relation may become less visible while the credential remains. Authority generated through the network appears to reside autonomously in the machine-certified object. The local warrant acquires a symbolic surplus: the credential can signify that the wider mathematical claim is secure or settled.
5. **Fetishistic disavowal and reproduction.** This is a conditional feedback mechanism, not a necessary stage in every case. It occurs when an actor or institution explicitly acknowledges the human, semantic, or technical conditions that limit the credential’s warrant, yet continues to mobilize an autonomous or broader public representation of the credential. The actor need not confess that its own wording overreaches. The disavowal is located in the public practice that holds acknowledged mediation together with continued investment in the credential as the apparent bearer of the whole achievement.

The first two moments are enabling conditions; the third gives the achievement a portable form; the fourth is the specifically fetishistic conversion; and the fifth explains how that authority may be sustained after awareness. Condensation alone is not fetishism, and distributed labour does not automatically become invisible. Nor does awareness of the kernel’s scope by itself establish disavowal. The relevant knowledge is the publicly acknowledged human or semantic mediation that qualifies the machine’s contribution. Fetishistic disavowal appears when this acknowledgement coexists in the same communication chain with a continued autonomous-machine representation of the whole achievement. The actor need not explicitly acknowledge that its own wording overreaches.

The sequence can be represented as a formation process with a conditional feedback loop:

\[
\text{Real reliability}+\text{Distributed labour}
\longrightarrow
\text{Credential condensation}
\longrightarrow
\text{Objectal displacement}
\longrightarrow
\text{Symbolic authority}.
\]

\[
\text{Acknowledged human/semantic mediation}+\text{continued autonomous-machine framing}
\longrightarrow
\text{Fetishistic disavowal}
\circlearrowleft
\text{reproduction of symbolic authority}.
\]

The relation is inverted: the network makes the credential meaningful, yet the credential appears as the source that certifies the network. This is the objectal displacement at the centre of the proposed concept.

### 4.4 Fetishistic disavowal and the persistence of symbolic investment

Žižek’s primary account is already explicit in *The Sublime Object of Ideology*. He introduces the formula “I know very well, but still” in his discussion of money as a fetish object (Žižek 1989, 12–13). He returns to the same structure in his analysis of commodity fetishism: individuals know that money expresses social relations, yet in their actual social activity they act as if money were the immediate embodiment of wealth (Žižek 1989, 28–30). They are “fetishists in practice, not in theory.” The illusion is not simply a false proposition in consciousness; it is embodied in the form of social activity. Žižek further describes belief as externalized in effective procedures, so that the social object can appear to “believe” in place of the subjects who use it (Žižek 1989, 31–32).

This structure must be distinguished from cynical reason. Žižek’s discussion of cynicism draws on Sloterdijk’s *Critique of Cynical Reason* and concerns the subject’s awareness of the distance between an ideological mask and social reality, while continuing to insist on the mask (Žižek 1989, 24–27). Fetishistic disavowal is more specific to the present argument: acknowledged knowledge does not dissolve the practical investment embodied in the object and the social procedure through which it functions. Kuldova (2019) and Black (2025, 118–119) clarify the distinction between cynical and fetishistic disavowal, but the central structure is grounded in Žižek’s own analysis of commodity fetishism and the objectivity of belief.

Applied to formal verification, the relevant knowledge is the publicly acknowledged human and semantic mediation through which a checked formal proposition becomes a mathematical achievement. This includes selecting a problem, supplying a formal target, validating that target against the original conjecture, interpreting the result, and producing a mathematical exposition. Fetishistic disavowal becomes visible when these conditions are acknowledged within a publication or institutional communication chain, while the machine nevertheless remains the apparent autonomous subject of the achievement in that same chain.

This is not equivalent to rational epistemic dependence. A mathematician who knows that Lean checks a proof term for \(P^*\) under \(\Gamma\), and relies on it for precisely that task, is not engaged in disavowal. Nor is a claim of autonomous proof search necessarily a claim of autonomous mathematical validation. The relevant question is how a narrower operational truth functions in public representation. When the agent’s autonomy in proof search becomes the public sign of the whole mathematical achievement, while the same communication chain acknowledges the human work that interprets and validates that achievement, operational autonomy and symbolic autonomy occupy different registers.

The AlphaProof Nexus case makes this structure visible. The research paper reports expert validation of the correspondence between Lean statements and original Erdős conjectures; its author-contribution statement identifies human roles in selecting problems, validating generated solutions, and writing natural-language proofs. The associated Aarhus University account likewise identifies human problem selection, solution validation, and exposition, yet retains the description of the agent as having “autonomously resolved” the problems. Human mediation is not hidden. Its public acknowledgement coexists with the continued representation of the machine as the apparent bearer of the achievement.

The fifth-stage proposition is therefore not that participants secretly believe the machine literally works alone. It is that the public procedure of attribution continues to organize the achievement around the autonomous machine even while its human and semantic conditions are explicitly stated. The knowledge of mediation and the investment in machine autonomy occupy different registers. The public record supports an analysis of this representational practice; it does not establish private or unconscious motives.

A case-level diagnosis requires:
1. explicit acknowledgement of the human, semantic, or technical mediation relevant to the credential’s scope;
2. continued circulation, within the same communication chain, of an autonomous-machine representation with a plausible wider reading;
3. a recognizable public-authority or legitimating role for that representation;
4. a contextual reading in which the autonomy formulation is not exhausted by a narrowly technical description of proof search.

If a source clearly limits autonomy to proof search after a formal target is supplied, and the wider mathematical achievement is attributed to the human–machine network, the fifth moment is not established. The analysis concerns the public organization of authority, not a speculative diagnosis of individual psychology.


### 4.5 The missing guarantee

The Lacanian/Žižekian idea that there is no complete Big Other and no “Other of the Other” provides a structural background. It does not imply that mathematical proof is impossible or that standards are arbitrary. Lean is not the Big Other. The question is whether the credential is made to function as if it supplied a final guarantee of every level of mathematical knowledge. This is background, not a fourth co-equal mechanism.

## 5. Diagnostic architecture

The exact technical warrant is the baseline, not a discriminating indicator of ideology. A strong diagnosis requires three additional and analytically distinct conditions:

- **S — Scope extension:** a public or institutional representation extends either (a) the warrant attributed to a credential beyond the checked proposition and its documented specification relation (**warrant-scope extension, S_w**), or (b) the agency attributed to a machine from a bounded operation, such as autonomous proof search, to the broader achievement of resolving a mathematical problem (**agency-attribution extension, S_a**). The precise shift in scope must be identified. S_a does not imply that the mathematical result is false or that the formal proof lacks warrant.
- **O — Objectal displacement:** the credential or machine is represented or practically treated as the self-sufficient bearer of wider authority or achievement, while the semantic, technical, or institutional relations that make it meaningful are subordinated or displaced. Omission alone is insufficient; the analysis must show how the public attribution locates agency or authority in the object.
- **E — Social efficacy:** the representation has a documented role in legitimation, recognition, credibility allocation, institutional action, or a repeated public practice. A single phrase without a recognizable public-authority function does not establish this condition.

The core diagnosis requires S ∧ O ∧ E. S may concern the scope of warrant or the scope of agency attribution; the two must not be conflated. A scope shift does not by itself establish objectal displacement, and a representation of autonomous authority does not by itself establish a legitimating effect. The five-moment mechanism explains how the credential acquires authority and how it may be reproduced. Fetishistic disavowal is a conditional feedback mechanism, not a necessary fifth step in every case. Its public-discourse form requires acknowledged human/semantic mediation, continued autonomous-machine framing within the same communication chain, and a recognizable public-authority or legitimating role. The wider autonomous reading must remain available in context; a statement restricted to proof-search autonomy is insufficient.

## 6. Three empirical planes

Following Žižek’s “The Spectre of Ideology” (1994, 9–10), the evidence is examined across:
1. **Discursive plane:** papers, technical reports, institutional statements, press releases, and media accounts.
2. **Material-institutional plane:** repositories, checking workflows, review procedures, publication practices, and institutional acts of recognition.
3. **Spontaneous-practical plane:** repeated practices in which a Lean credential is treated as a default warrant for broader claims.

The third plane requires evidence of repeated practice; it cannot be inferred from a single announcement. These are empirical planes, not additional ideological mechanisms.

## 7. Four-case design and current assessment

| Case | Analytical function | Current assessment |
|---|---|---|
| Riemann hypothesis | Formal certification, institutional authorization, AI-mediated exposition, and a public challenge to the meaning of the certification | Layered and contested authorization; objectal displacement not established |
| Navier–Stokes | Relation between Lean declarations and a separate natural-language proof | Strongest candidate for scope extension; objectal displacement and social efficacy remain unestablished |
| Erdős / AlphaProof Nexus | Human statement validation, benchmark scope, artifact provenance | Mixed case; no full fetishism diagnosis |
| Liquid Tensor Experiment | Explicit definition sanity checks and visible collective labour | Strong counter-case |

The cases are heterogeneous comparative configurations, not matched controls or a representative sample of Lean use. The current evidence does not establish S ∧ O ∧ E in any one case. The paper’s empirical claim must remain correspondingly bounded.

## 8. Rival explanations and falsification

The model is weakened or a case should be coded as warranted reliance, transparent mediation, ambiguity, or insufficient evidence when:
- the credential is confined to the exact formal proposition;
- the specification relation and assumptions are made explicit;
- human and institutional mediation remains visible;
- the checker is treated as one component in a wider assessment;
- apparent overstatement is ordinary shorthand whose context preserves scope;
- no institutional or practical effect is documented.

A scope mismatch does not automatically establish objectal displacement. Objectal displacement does not automatically establish social efficacy. These distinctions prevent double-counting one observation.

## 9. Originality boundary

The paper does not claim:
- a new taxonomy of proof-level warrant;
- the first distinction between derivational validity and semantic correspondence;
- the first social epistemology of proof assistants;
- the first Žižekian critique of technology;
- the first ideology critique of AI;
- that all reliance on Lean is irrational or ideological.

The proposed contribution is a Žižekian diagnostic account of how the genuine but bounded warrant of Lean verification may acquire a wider symbolic function through the credential “Lean-verified,” and of the conditions under which that credential becomes an objectal bearer of mathematical authority.

## 10. Core references

- Žižek, Slavoj. The Sublime Object of Ideology. London: Verso, 1989.
- Žižek, Slavoj. “The Spectre of Ideology.” In Mapping Ideology, edited by Slavoj Žižek, 1–33. London: Verso, 1994.
- Marx, Karl. Capital, vol. I, ch. 1, §4. 1976 [1867].
- Vallverdú, Jordi. “Where Does Mathematical Warrant Live?” Philosophies 11(6) (2026): 224. DOI: 10.3390/philosophies11060224.
- Kallel, Maher, and Mohamed El Louadi. “Verification Abundance, Adjudication Scarcity.” arXiv:2608.28997 (2026).
- López-Corona, Oliver. “From Authorial Mathematics to Studio Mathematics.” arXiv:2608.22194 (2026).
- Erfani, Farhang. “Not ‘Just a Language Model’: AI’s Ideological Functions.” AI & Society 41 (2026): 869–881.
- Hourigan, Daniel. The Phantasmatic Subject of Technology. PhD thesis, Griffith University, 2009.
- Hardwig, John. “Epistemic Dependence.” The Journal of Philosophy 82(7) (1985): 335–349.
- Black, Jack. “Examining the Mechanism of Disavowal and Its Two Forms.” Theory & Psychology 35(1) (2025): 117–135.
- Kuldova, Tereza Østbø. “Fetishism and the Problem of Disavowal.” Qualitative Market Research (2019).
