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
5. **Fetishistic disavowal and reproduction.** This is a conditional feedback mechanism, not a necessary stage in every case. It occurs when an actor or institution acknowledges that the credential is being asked to warrant more than the check establishes, yet continues to mobilize it in that broader role. The knowledge of the boundary and the investment beyond it coexist, allowing the credential’s symbolic authority to be reproduced.

The first two moments are enabling conditions; the third gives the achievement a portable form; the fourth is the specifically fetishistic conversion; and the fifth explains how that authority may be sustained after awareness. Condensation alone is not fetishism, and distributed labour does not automatically become invisible. Nor does awareness of the kernel’s scope by itself establish disavowal. The relevant knowledge must concern the mismatch between the credential’s actual warrant and the broader authority it is made to carry.

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
\text{Acknowledged boundary}+\text{continued investment beyond it}
\longrightarrow
\text{Fetishistic disavowal}
\circlearrowleft
\text{reproduction of symbolic authority}.
\]

The relation is inverted: the network makes the credential meaningful, yet the credential appears as the source that certifies the network. This is the objectal displacement at the centre of the proposed concept.

### 4.4 Fetishistic disavowal and the persistence of symbolic investment

Žižek’s discussion of cynical ideology draws on Sloterdijk’s critique of cynical reason (Žižek 1989, 24–27). Recent work distinguishes cynical disavowal from fetishistic disavowal (Kuldova 2019; Black 2025, 118–119). Cynical disavowal maintains a manipulative distance between knowledge and action. Fetishistic disavowal has a different structure: the subject can acknowledge the objective limitation and the subjective appearance through which the object continues to function, yet remain invested in it.

For this study, it is not enough that a participant knows that Lean checks a proof term for \(P^*\) under \(\Gamma\), while the relation between \(P^*\) and the intended claim \(P\) is a distinct task. That knowledge is compatible with rational reliance. The relevant structure appears when the same actor or institutional communication chain explicitly acknowledges a limitation that matters to the public claim, yet continues to circulate a credential or description that can reasonably be read as conferring wider authority.

The actor need not explicitly confess that its own wording overstates the technical warrant. Public evidence must, however, connect the acknowledged boundary and the wider representation within the same communication chain. The wider reading must remain genuinely available in context. A statement carefully limited to autonomous proof search, for example, is not automatically a claim of autonomous mathematical validation. Nor is a technical qualification followed by a broader claim fetishistic when expert semantic review has independently established the relation between \(P^*\) and the intended claim \(P\). In that case, the broader claim may be warranted by the whole network rather than attributed to the kernel alone.

A case-level diagnosis therefore requires:
1. explicit acknowledgement of the specific technical or semantic boundary relevant to the claim;
2. continued circulation of the same credential or an equivalent public representation with a plausible wider reading;
3. continuity within the same actor or institutional communication chain;
4. an unresolved scope tension and a recognizable practical or legitimating role.

If expert review or another independent procedure has established the semantic relation between the formal proposition and the intended theorem, a broader claim may be warranted by the combined network. That is not disavowal. A generic statement that AI systems can make mistakes is not enough to establish knowledge of the specific boundary at issue.

Disavowal is therefore not necessary for the initial emergence of objectal displacement. It is the mechanism through which that displacement can be reproduced despite awareness. The public record can establish an actor’s acknowledged qualification and subsequent representation or practice; it does not, by itself, establish unconscious motives. The analysis concerns the public structure of knowledge and investment, not a speculative diagnosis of private psychology.



### 4.5 The missing guarantee

The Lacanian/Žižekian idea that there is no complete Big Other and no “Other of the Other” provides a structural background. It does not imply that mathematical proof is impossible or that standards are arbitrary. Lean is not the Big Other. The question is whether the credential is made to function as if it supplied a final guarantee of every level of mathematical knowledge. This is background, not a fourth co-equal mechanism.

## 5. Diagnostic architecture

The exact technical warrant is the baseline, not a discriminating indicator of ideology. A strong diagnosis requires three additional and analytically distinct conditions:

- **S — Scope extension:** a public or institutional representation attributes to the credential a warrant broader than the checked proposition and documented specification relation. The precise inferential gap must be identified.
- **O — Objectal displacement:** the credential is represented or practically treated as a self-sufficient source of wider authority, while the semantic, technical, or institutional relations that make it meaningful are backgrounded or displaced. Omission alone is insufficient.
- **E — Social efficacy:** the representation has a documented role in legitimation, recognition, credibility allocation, institutional action, or a repeated practice. A single phrase without practical or institutional significance does not establish this condition.

The core diagnosis requires S ∧ O ∧ E. These conditions are analytically distinct: a scope mismatch does not by itself establish objectal displacement, and a representation of autonomous authority does not by itself establish a legitimating effect. The five-moment mechanism explains how the credential acquires authority and how it may be reproduced. Fetishistic disavowal is a conditional feedback mechanism, not a necessary fifth step in every case. It requires explicit acknowledgement of the specific boundary, continued circulation of a credential or description with a plausible wider reading in the same actor/institutional chain, an unresolved scope tension, and a recognizable legitimating or practical role. The actor need not explicitly confess that the wording overreaches.

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
