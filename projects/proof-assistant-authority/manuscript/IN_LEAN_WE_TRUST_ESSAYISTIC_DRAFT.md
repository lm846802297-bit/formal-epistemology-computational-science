# In Lean We Trust? The Ideology of Machine-Checked Proofs in Science

**Project:** *In Lean We Trust?*  
**Version:** Essayistic philosophical draft  
**Evidence cut-off:** 27 November 2026  
**Genre:** Philosophical argument with comparative case analysis

## Abstract

What could be ideological about a correct proof? Lean’s kernel provides genuine, bounded warrant for a formal proposition under a specified environment. This article asks how such a local achievement can become a source of wider mathematical authority. Drawing on Slavoj Žižek’s critique of ideology, it develops the concept of the **ideological fetishism of formal verification** through five moments: real technical reliability; distributed epistemic labour; condensation into the credential “Lean-verified”; objectal displacement, through which network-generated authority appears to reside in the credential itself; and, conditionally, fetishistic disavowal, through which symbolic investment persists alongside acknowledged human and semantic mediation. Four cases—the Riemann hypothesis, Navier–Stokes, AlphaProof Nexus’s work on Erdős problems, and the Liquid Tensor Experiment—show contrasting configurations. AlphaProof Nexus provides a positive existence case: the research paper and an associated university account identify human problem selection, validation of formal statements against original conjectures, and mathematical exposition, while continuing to describe the agent as having “autonomously resolved” the problems. The analysis identifies a shift from operational autonomy in proof search to public attribution of the mathematical achievement to the machine. It argues that formal verification’s genuine reliability is not what ideology must explain away, but what it must explain: how a bounded technical guarantee becomes the material support for symbolic authority beyond the operation that produced it.

**Keywords:** philosophy of science; mathematical practice; ideology critique; formal verification; Lean; epistemic authority

---

## 1. The Paradox of a Verified Proof

What is ideological about a correct proof?

Imagine that a mathematical proposition has been formalized, a proof term has been constructed, and Lean’s kernel accepts it. There is no need to look for a hidden failure in the machine. The proof assistant has performed the task for which it was designed. Under the specified formal environment, the term has the required type. The result is reproducible, inspectable, and, in principle, independently checkable. Why, then, should we speak of ideology? Would this not confuse a genuine mathematical achievement with a social illusion?

The question becomes difficult only when we abandon a familiar conception of ideology. If ideology means false consciousness, then the answer seems immediate: there is nothing ideological about a correct proof. One either has a valid derivation or one does not. Once the relevant facts are established, the ideological appearance should disappear.

But this is precisely the point at which Žižek’s critique becomes relevant. Ideology cannot always be identified by asking whether an explicit proposition is true or false. A statement may be factually correct and nevertheless participate in an ideological relation through the position it occupies and the practice it helps sustain (Žižek, 1989, 1994). The question is not simply whether Lean’s verdict is correct. It is what this verdict is made to authorize.

Consider the difference between two statements:

> Lean’s kernel accepts a proof term for the formal proposition \(P^*\).

and

> The mathematical problem has been conclusively solved.

The first statement identifies a technical result. The second makes a claim about a mathematical achievement whose warrant may involve much more: the identity of \(P^*\) with the intended theorem, the adequacy of its definitions and assumptions, the relation between a formal artifact and a natural-language argument, and the status of the result within mathematical practice. The first does not automatically entail the second. Yet the public credential “Lean-verified” can travel between them, sometimes without the intervening relations being made visible.

The paradox is therefore not that a machine produces false certainty. It is that a machine may produce a genuine form of certainty, sharply bounded in its technical operation, while the credential associated with that achievement comes to signify something wider. The machine does not have to be unreliable for its authority to acquire an ideological function. On the contrary, its genuine reliability may be what makes the wider symbolic investment possible. A defective instrument could hardly serve as a convincing bearer of certainty. **The machine’s reliability is not what ideology must explain away. It is precisely what ideology must explain.** The ideological question begins not when the kernel fails, but when the genuine warrant of its operation becomes the material support for a symbolic authority that exceeds that operation.

This article asks how that transformation can occur. Its object is not Lean software in general, nor the psychological question of whether mathematicians trust machines. It is the public and institutional credential **“Lean-verified”**: the compact sign through which a complex formal and mathematical process becomes recognizable as a warrant for a result. The central hypothesis is that this credential may acquire an ideological function when the authority generated through a network of technical, semantic, and institutional relations appears to reside autonomously in the verification object itself.

The argument is not that formal verification is a deception, that mathematical truth is merely socially constructed, or that reliance on a proof assistant is irrational. A mathematician who relies on Lean for the task it actually performs may be entirely justified. Nor is every short description of a formal proof an instance of ideological distortion. The issue is more specific: under what conditions does a bounded technical credential become a symbolic guarantee of a wider mathematical claim, and what happens to the relations that connect the credential to that claim?

The question is worth asking because formal verification makes one part of mathematical warrant unusually visible. A proof may be extremely long, technically complex, and difficult for any individual mathematician to survey. Yet the result of kernel checking can be stated in a compact form. The complexity of the proof does not disappear; it becomes condensed in a portable credential. The word “verified” can then function as a point at which the otherwise distributed process of mathematical knowledge production seems to arrive at a final answer.

The following pages approach this problem through Žižek’s account of ideological fantasy and fetishism. Fantasy explains how a local check can stage the appearance of closure; fetishism explains how the authority generated by a network of relations can appear as an autonomous property of an object. Fetishistic disavowal then explains how this symbolic investment may persist even when the human and semantic conditions of verification are publicly acknowledged. The four cases trace these relations in different configurations, with AlphaProof Nexus providing the positive existence case for this final mechanism.

Four encounters with Lean formalization will help clarify the argument. They are not four interchangeable examples, nor do they constitute a representative sample of proof-assistant practice. The Riemann hypothesis case concerns the relation between formal certification, institutional authorization, and foundational criticism. Navier–Stokes raises the problem of correspondence between a formal declaration and a separate natural-language proof. Erdős problems investigated with AlphaProof Nexus reveal the importance of human statement validation and artifact provenance. The Liquid Tensor Experiment provides a counter-case in which collective mathematical labour and semantic scrutiny are made unusually visible.

The guiding question throughout is simple, although its answer is not: when a proof is verified, what exactly has been verified—and what, beyond that, is the credential being asked to guarantee?

## 2. The Limits of Formal Certainty

The first task is to resist two opposite mistakes. The first is to treat formal verification as if it were merely a ceremonial endorsement of work already completed elsewhere. The second is to treat kernel acceptance as if it settled every question that can be asked about a mathematical result. Both mistakes obscure the distinctive epistemic value of formal verification.

Lean is a proof assistant based on dependent type theory. A proposition is represented as a formal type, and a proof is represented by a term inhabiting that type. The kernel checks whether the term has the required type relative to a specified formal environment, including definitions, axioms, imported libraries, and the trusted implementation. Schematically,

\[
\operatorname{KernelAccepts}(t : P^* \mid \Gamma)
\]

states that the proof term \(t\) is accepted as a proof of the formal proposition \(P^*\) under the environment \(\Gamma\).

This is a substantial achievement. It provides a highly reliable check of derivational validity relative to the formal system. It can exclude many classes of derivational error, support replay of proof artifacts, and allow independent implementations to check the exported proof. The fact that a proof was generated by an opaque AI system does not by itself remove this warrant. Duede and Davey (2025), for example, argue that a transparent proof checker can provide genuine mathematical knowledge even when the process that generated the proof is opaque. The check is not merely a performance staged for an audience. It does real epistemic work.

The question is what follows from that work.

Let \(P\) denote the intended mathematical claim and \(P^*\) the formal proposition submitted to Lean. Kernel acceptance establishes that a proof term proves \(P^*\) under \(\Gamma\). It does not, by that operation alone, establish the relation

\[
P \longleftrightarrow P^*.
\]

This relation concerns the adequacy of the formal specification: does the formal proposition express the mathematical claim that researchers intend to establish? It may be checked with great care. Definitions can be inspected, source statements compared, and the formalization scrutinized by mathematicians. In some settings, parts of the specification relation can themselves be formalized. The point is not that this relation is mysterious or impossible to establish. It is that checking a proof term and checking the adequacy of the proposition being proved are distinct epistemic tasks.

This distinction is now central to the philosophy of mathematical warrant. Vallverdú’s Locus Thesis argues that properties such as reliability, surveyability, transferability, and explanatory power should be assigned to components of a warrant architecture, rather than indiscriminately predicated of a proof as a whole (Vallverdú, 2026). Kallel and El Louadi (2026) similarly distinguish derivational validity, representational fidelity, and epistemic significance. They argue that the abundance of machine-checked proofs does not remove the need for human adjudication; it changes where that adjudication is required.

The present article adopts this component-based account. It does not claim originality for the distinction between a formal proposition, a proof object, a checking procedure, a trusted base, and the intended mathematical claim. Nor does it claim that the gap between formal and informal mathematics is unbridgeable. The relevant point is more modest and more consequential: the warrant supplied by a kernel check is one component of a wider architecture, and the authority of the whole cannot simply be read off from the reliability of that component.

The same caution applies to the social organization of mathematics. A mathematician cannot personally reproduce every piece of software, inspect every library dependency, and independently reconstruct every proof used in a large formalization. Nor should this be expected. Scientific knowledge depends on a division of epistemic labour. Hardwig’s account of epistemic dependence explains why reliance on experts can be rational even when the person relying on them cannot personally reproduce their evidence (Hardwig, 1985). De Millo et al. (1979) likewise emphasize that mathematical proof operates within social processes of criticism, communication, and acceptance.

There is nothing ideological merely in relying on Lean, trusting a competent formalizer, or accepting a well-documented institutional review. Such reliance can be rational. A journal may reasonably require a formal artifact; a mathematician may reasonably rely on independent kernel checking; a reader may reasonably trust experts who have compared a formal proposition with its intended statement.

This is where the problem becomes more precise. Social mediation is not ideology; distributed labour is not fetishism; institutional recognition is not automatically a distortion. The ideological question arises when the credential associated with one component of the warrant architecture comes to appear as if it contains the authority of the whole. The kernel’s reliability gives the credential its genuine technical warrant. The symbolic problem begins when that local warrant becomes the visible bearer of a certainty sustained by relations extending beyond the check itself. **The reality of the technical achievement is therefore the starting point of the ideology critique, not an objection that the critique must overcome.**

## 3. Žižek and the Ideological Structure of Verification

### 3.1 Ideology beyond false consciousness

In “The Spectre of Ideology,” Žižek shifts the question of ideology away from the simple opposition between true and false beliefs (Žižek, 1994). The ideological function of a proposition cannot be read directly from its truth value. A statement may be factually correct and nevertheless participate in an ideological relation through the position it occupies and the practice it helps sustain. What matters is not only whether a statement is true, but how its truth is mobilized within a social order.

“Lean checked this proof” may be entirely accurate. Its philosophical significance emerges when this true statement becomes the point through which a wider mathematical claim is authorized. The credential can remain attached to the formal proposition and the conditions under which it was checked; it can also travel as if it carried the authority of the entire mathematical result. The same technical fact can therefore occupy different positions within the production of knowledge.

Žižek’s account directs attention beyond explicit discourse. In “The Spectre of Ideology,” he distinguishes ideology as doctrine, its material externality in practices and institutions, and its more elusive spontaneous operation within social reality (Žižek, 1994, pp. 9–10). Applied to formal verification, this means that the credential must be studied across the settings in which it acquires force: the repository in which a proof is checked, the paper that reports it, the institution that recognizes it, and the practices through which mathematical credibility is distributed. Ideology is not simply a mistaken sentence about a machine. It concerns the relation between what is said, what is materially done, and what becomes authoritative.

### 3.2 Ideological fantasy: the scene in which uncertainty appears to end

In *The Sublime Object of Ideology*, fantasy is not merely a false image concealing an otherwise complete reality. It supplies the coordinates through which reality is experienced and sustains the appearance of coherence where a constitutive gap remains (Žižek, 1989, pp. 28–31). Fantasy organizes the scene in which a practice becomes intelligible and an incomplete relation can appear whole.

The relevant limit in formal verification is the non-identity between the formal object that is checked and the intended mathematical claim to which it is connected. Let \(P\) be the intended claim and \(P^*\) the formal proposition. The kernel may establish with extraordinary precision that a proof term \(t\) inhabits \(P^*\) under a specified environment \(\Gamma\). The relation between \(P\) and \(P^*\) is a distinct specification relation. It can be scrutinized, formalized in part, checked by experts, and made highly reliable. The point is that this work remains conceptually distinct from the kernel's acceptance of \(t : P^*\).

This is a question of non-totalizability, not an unbridgeable gulf. The specification relation may be rigorously established; the different components of warrant may be connected without becoming the same operation. The ideological possibility arises when the local verdict is staged as the point at which the wider work of specification, interpretation, and institutional assessment appears already complete.

The fantasy of formal verification is therefore a scene of closure. The certificate seems to settle not only whether \(t\) proves \(P^*\), but also whether \(P^*\) is the intended theorem, whether the assumptions are appropriate, whether the result has the significance attributed to it, and whether the mathematical dispute is over. The fantasy does not have to appear as the explicit belief that Lean can prove everything. Its operation is subtler: the visible completion of one task gives the appearance that the whole chain of warrant has reached completion.

The distinction can be written schematically:

\[
\operatorname{KernelAccepts}(t : P^* \mid \Gamma)
\]

is a technical result. But

\[
\operatorname{KernelAccepts}(t : P^* \mid \Gamma)
\Rightarrow
\text{the wider mathematical claim is fully settled}
\]

is not a consequence of kernel acceptance alone.

Why is this scene compelling? Formal verification makes one part of mathematical warrant unusually visible. A proof may depend on extensive libraries, complex formalization, and years of technical work, while the result of checking can be communicated in a compact and reproducible form. The word “verified” gives a heterogeneous process a single point of presentation. Fantasy names the way this local completion can appear as the completion of the whole.

### 3.3 Fetishism: when the relation appears as a property of the object

The more decisive theoretical move comes from Marx’s account of commodity fetishism. In *Capital*, Volume I, Chapter 1, Section 4, Marx analyzes how relations among producers assume the appearance of relations among things. Žižek’s discussion emphasizes how an effect generated by a network of relations can appear as an immediate property of an object (Žižek, 1989, pp. 19–20).

The analogy with formal verification is structural. Mathematical truth is not produced by collective labour in the same way that commodities are produced, and Lean is not a commodity in Marx’s technical economic sense. The relevant structure is the appearance of a relation-dependent authority as an intrinsic property of an object.

The authority of a Lean-verified result depends on a network: the problem is selected and formulated; definitions and assumptions are chosen; the intended theorem is represented formally; a proof object is constructed; libraries and software infrastructure are maintained; the kernel checks the proof term; experts examine the specification relation; institutions and mathematical communities assess the result’s status. These activities contribute different forms of warrant. Their combined authority is what allows the formal artifact to count as a proof of a particular mathematical claim.

The fetishistic possibility appears when the authority generated through this network seems to reside autonomously in the verification credential itself. The credential appears not merely to report that one component of the proof process has succeeded, but to contain the authority of the whole. The relation is inverted: the network makes the credential meaningful, yet the credential appears as the source that certifies the network.

Fantasy and fetishism therefore do different work. Fantasy supplies the scene in which the local check appears to close the wider question. Fetishism gives this appearance an objectal form: the closure seems to reside in the credential itself. The first concerns the staging of completeness; the second concerns the apparent location of the authority that completeness promises. They reinforce one another, but they are not interchangeable.

### 3.4 Fetishistic disavowal and the persistence of symbolic investment

The primary theoretical basis for fetishistic disavowal is already present in *The Sublime Object of Ideology*. Žižek invokes the formula “I know very well, but still” in his discussion of money as a fetish object (Žižek, 1989, pp. 12–13). He returns to the same problem in the analysis of commodity fetishism: individuals know that money is an expression of social relations, yet in their actual social activity they act as if money were the immediate embodiment of wealth (Žižek, 1989, pp. 28–30). They are, in Žižek’s phrase, “fetishists in practice, not in theory.” The decisive point is that the illusion is not simply a false proposition held in consciousness. It is embodied in the form of social activity itself. Žižek further describes belief as externalized in effective procedures: the social object can appear to “believe” in place of the subjects who use it (Žižek, 1989, pp. 31–32).

This account must be distinguished from the discussion of cynical reason that follows Žižek’s engagement with Sloterdijk (Žižek, 1989, pp. 24–27). Cynical ideology concerns the subject’s awareness of the distance between an ideological mask and social reality, while continuing to insist on the mask. Fetishistic disavowal is more specific to the present argument: acknowledged knowledge does not dissolve the practical investment embodied in the object and the social procedure through which it functions. Black (2025, 118–119) and Kuldova (2019) help clarify the distinction between cynical and fetishistic forms of disavowal, but the central structure is not imported into Žižek from this later literature; it is grounded in his own analysis of commodity fetishism and the objectivity of belief.

Applied to formal verification, the relevant knowledge is the publicly acknowledged human and semantic mediation through which a checked formal proposition becomes a mathematical achievement. This includes selecting a problem, supplying a formal target, validating that target against the original conjecture, interpreting the result, and producing a mathematical exposition. Fetishistic disavowal becomes visible when these conditions are acknowledged within a publication or institutional communication chain, while the machine nevertheless remains the apparent autonomous subject of the achievement in that same chain.

This is not equivalent to rational epistemic dependence. A mathematician who knows that Lean checks a proof term for \(P^*\) under \(\Gamma\), and relies on it for precisely that task, is not engaged in disavowal. Nor is a claim of autonomous proof search necessarily a claim of autonomous mathematical validation. The relevant question is how a narrower operational truth functions in public representation. When the agent’s autonomy in proof search becomes the public sign of the whole mathematical achievement, while the same communication chain acknowledges the human work that interprets and validates that achievement, operational autonomy and symbolic autonomy occupy different registers.

The AlphaProof Nexus case makes this structure visible. The research paper reports expert validation of the correspondence between Lean statements and original Erdős conjectures; its author-contribution statement identifies human roles in selecting problems, validating generated solutions, and writing natural-language proofs. The associated Aarhus University account likewise identifies human problem selection, solution validation, and exposition, yet retains the description of the agent as having “autonomously resolved” the problems. Human mediation is not hidden. Its public acknowledgement coexists with the continued representation of the machine as the apparent bearer of the achievement. The fifth moment is therefore not the persistence of a mistaken belief that the machine literally works alone. It is the persistence of symbolic investment in machine autonomy within a public practice that simultaneously acknowledges the human relations sustaining the result.

Disavowal is not necessary for the initial emergence of objectal displacement. It explains how the symbolic authority of the credential may be reproduced despite the visibility of the relations that sustain it. The public record can establish this structure of representation and practice; it does not establish private or unconscious motives. The analysis concerns the public organization of knowledge and authority, not a speculative diagnosis of individual psychology.


## 4. The Machine as a Fetish Object

How does the credential “Lean-verified” acquire authority beyond the technical operation it records? The answer is not that a machine suddenly becomes an object of irrational admiration, nor that a community simply mistakes a technical procedure for something it is not. The process is more interesting: a real technical achievement is produced through distributed labour, condensed into a portable sign, and then made to carry a symbolic authority that appears to belong to the sign itself.

The formation and reproduction of the epistemic fetish can be reconstructed through five connected moments. They are analytically ordered, not a rigid chronology. The first two provide the material conditions; the third gives the achievement a portable form; the fourth marks the specifically fetishistic conversion; and the fifth explains how that authority may be reproduced after its human and semantic conditions are acknowledged. The fifth moment is a feedback mechanism, not a necessary stage through which every use of Lean must pass.

**First, the check has real technical efficacy.** Lean’s kernel does not merely symbolize reliability. It checks whether a proof term has the required type for a specified formal proposition under a specified environment. The result can be replayed, inspected, and, in appropriate settings, checked independently. This is the material basis of the credential’s credibility. The ideological function of formal verification does not arise because the machine fails to do its job. It becomes possible because the machine genuinely does something valuable. Its reliability is not an illusion that must be exposed; it is the real achievement around which a wider symbolic investment can gather.

**Second, the achievement is produced through distributed epistemic labour.** The formal result depends on more than the kernel. A mathematical problem must be selected and formulated; definitions and assumptions must be chosen; the intended claim must be represented as a formal proposition; a proof must be found and encoded; libraries and software tools must be developed and maintained; the trusted environment must be specified; the formal statement must be compared with the intended theorem; and the result must be interpreted and assessed by mathematicians, reviewers, and institutions. These activities are distributed across people, technical systems, and organizations. They contribute different kinds of epistemic work, and no single component performs the whole task.

This distribution is not a defect in mathematical knowledge. It is a condition of contemporary mathematical practice. It means that the authority of a result is assembled across a network whose full operation may not be visible to any one participant. The result depends on relations of expertise, maintenance, interpretation, and institutional recognition. The technical check is one indispensable component within this larger arrangement. Whether these relations remain visible or recede from view becomes decisive later in the argument.

**Third, scientific communication condenses this distributed process into a credential.** A complex mathematical achievement must travel. It appears in an abstract, a paper title, a repository description, a journal announcement, a university news item, a conference presentation, or a media report. These forms cannot reproduce the entire history of formalization and review. They need a compact way to identify what has been accomplished. “Lean-verified” performs this communicative function. It condenses theorem formulation, formal specification, proof construction, kernel checking, and layers of human scrutiny into a single portable status.

Condensation is necessary for communication. It is not yet fetishism. A concise statement can preserve the scope of the check, and a credential can accurately summarize a complex process. The decisive question is what happens when the condensed sign begins to circulate as if it contained the authority of the relations that initially fixed its meaning.

**Fourth, the credential acquires symbolic authority through objectal displacement.** As “Lean-verified” moves across contexts, the exact formal proposition, environment, assumptions, dependencies, and specification relation may become less visible, while the credential itself remains. The sign travels more easily than the network that supports it. It can then appear not merely as a report that one component of a warrant architecture has succeeded, but as an autonomous guarantee of the result as a whole.

Here the relation is inverted. The network makes the credential meaningful, yet the credential appears as the source that certifies the network. Authority generated through mathematical judgement, formalization, software infrastructure, checking, and institutional assessment seems to reside in the machine-certified object. The local warrant of the kernel is thereby given a symbolic surplus: “Lean-verified” can come to signify not only that a formal proposition has been checked, but that the wider mathematical claim is secure, settled, and institutionally authoritative. This is the specifically fetishistic moment. The object appears to possess, as its own property, an authority that in fact depends on the relations that produced and interpreted it.

Three questions help distinguish this displacement from ordinary shorthand. **Scope extension** asks whether the credential is made to warrant more than the checked proposition and its documented relation to the intended claim. **Objectal displacement** asks whether the authority generated through the network appears to reside autonomously in the credential. **Social efficacy** asks whether this representation has a recognizable role in legitimation, recognition, credibility allocation, or institutional practice. A short announcement may condense a complex process without extending its scope; a visible credential may circulate without being treated as self-sufficient; and a symbolic representation may appear without having a discernible practical effect. The fetishistic diagnosis concerns their conjunction, not any one feature in isolation.

**Fifth, fetishistic disavowal can reproduce this authority through the public acknowledgement of mediation.** Žižek’s account does not require subjects to be theoretically ignorant of the social relations behind the fetish. The relevant structure is practical: acknowledged knowledge coexists with a social form that continues to organize action as if the object itself embodied the authority generated by those relations. In the present case, the fifth moment appears when a publication or institutional communication chain explicitly identifies the human and semantic work that qualifies the machine’s contribution, yet continues to present the machine as the apparent autonomous bearer of the whole mathematical achievement.

The distinction can be stated schematically:

\[
\text{acknowledged human/semantic mediation}
+
\text{continued autonomous-machine framing}
\]

This is the relevant structure of fetishistic disavowal in public representation. The actor need not confess that its own wording overstates the technical warrant, and the analysis does not depend on attributing conscious deception. What matters is that the wider autonomous-machine reading remains available in context and continues to organize the public description of the achievement. A claim carefully restricted to autonomous proof search is not, by itself, fetishistic. The effect appears when this operational autonomy becomes the public sign of the whole achievement, while the same communication chain acknowledges the human work of problem selection, statement validation, interpretation, or exposition.

This is not the same as cynical disavowal. Cynicism may conceal or manipulate the distance between knowledge and action. Fetishistic disavowal can openly acknowledge mediation while continuing to invest the machine with the symbolic position of autonomous mathematical authority. The knowledge of human contribution and the investment in machine autonomy occupy different registers. In Žižek’s terms, the belief is not simply hidden inside an individual consciousness; it is also embodied in the public procedure through which the achievement is named, attributed, and recognized.

The five moments can therefore be represented as a formation process with a conditional feedback loop:

\[
\begin{aligned}
&\text{Real technical reliability}
+\text{Distributed epistemic labour}\\
&\qquad\longrightarrow\text{Credential condensation}\\
&\qquad\longrightarrow\text{Objectal displacement}\\
&\qquad\longrightarrow\text{Symbolic authority},
\end{aligned}
\]

\[
\underbrace{\text{Acknowledged human/semantic mediation}
+\text{continued autonomous-machine framing}}_{\text{Fetishistic disavowal}}
\quad\circlearrowleft\quad
\text{reproduction of symbolic authority}.
\]

This is not a mechanical law, nor does every use of a formal verification system pass through each moment in the same way. The first four moments explain how a bounded technical achievement can become an object of wider epistemic authority. The fifth explains how that authority may be reproduced despite explicit knowledge of the human and semantic relations that sustain it. The machine’s reliability remains real throughout this process. What changes is the symbolic work that its credential is made to perform.

The fetish, then, is not simply the machine, and it is not a false belief about the machine. It is the credential through which the authority of a distributed epistemic network appears to be contained in a single object. Fetishistic disavowal explains one way this appearance is reproduced: not by concealing human mediation, but by allowing acknowledged mediation to coexist with the machine’s continued appearance as the autonomous bearer of mathematical authority. AlphaProof Nexus supplies the article’s positive existence case for this fifth moment.

The central philosophical finding follows: **the ideological fetishism of formal verification does not require the concealment of human mediation. It can operate through the very public acknowledgement of that mediation, while the machine continues to function as the apparent autonomous bearer of mathematical authority.**


## 5. Four Encounters with Formal Verification

The four encounters bring different relations between a formal artifact and its associated mathematical claim into view. Read together, they trace the five moments: the checker’s actual achievement; the distributed labour that makes the result meaningful; the condensation of this work into a public credential; the location of the authority attributed to that credential; and the persistence of symbolic investment alongside acknowledged human and semantic mediation.

### 5.1 The Riemann Hypothesis: a credential whose warrant remains visible

On 20 November 2026, Levent Alpöge released a note and a large Lean development concerning the Riemann hypothesis (Alpöge, 2026). The Lean FRO and Mathlib Initiative issued a joint statement on 21 November expressing “full confidence” in the proof and stating that the community certified both the statement and the proof (Lean FRO & Mathlib Initiative, 2026).

The first moment is unusually strong. The formal development compiles; the exported proof is accepted by Lean’s kernel and independent checkers; and Sutherland’s report records 175,187 compiling modules, independent kernel replay, and statement comparisons (Sutherland, 2026a). The second moment is equally visible. The result depends on Mathlib, formalization work, expert review of the theorem statement, community compilation, independent checker implementations, and further mathematical exposition. The joint statement does not conceal these contributions. It identifies them as the basis of its certification. The formal definition used in Mathlib is documented in the library reference (Mathlib Documentation, 2026).

The third moment appears in the public credential “Lean verification of the Riemann Hypothesis” and in the statement’s declaration of “full confidence.” The fourth moment is therefore present as institutional condensation: a complex network of checking and expert assessment is made communicable through the status of a certified Lean proof. Yet the same statement enumerates the distinct grounds of certification. It says that experts vetted the Mathlib statement, that independent tools confirmed the theorem proved in the archive is exactly that statement, and that multiple checkers accepted the exported proof. The authority is attached to the credential, but its basis remains visibly distributed. The statement does not present kernel acceptance as the sole source of the broader mathematical judgement.

A substantial exposition appeared on 26 November. The rh-lean-roadmap project provides a 497-page main text, 963 pages of longer proofs, a 122-page index, and a short roadmap. Its documentation states that several AI models generated the exposition from the Lean source and cross-checked it (rh-lean-roadmap, 2026). This is a readable, AI-mediated mathematical account, not a conventional independently authored paper. The joint statement itself looks forward to further mathematical work explaining the new ideas. That continuing need for explanation does not negate the certification; it distinguishes formal warrant from mathematical understanding.

Parker Emmerson’s non-peer-reviewed preprint of 24 November challenges the foundational interpretation of what the certification establishes (Emmerson, 2026). It grants the existence of the Lean derivation and reported checks but disputes what follows from them. This is a public challenge to the meaning of the certification, not evidence that the certifying institutions had acknowledged an unresolved defect and continued to use the credential as an overextended guarantee.

Riemann therefore displays powerful institutional authorization through a visibly composite warrant. The credential condenses the work of the kernel, independent checkers, expert vetting, and theorem comparison, while the certifying statement keeps these relations in view. Its significance for the comparison is to show that institutional authority can be strong without being represented as the autonomous property of the machine.

### 5.2 Navier–Stokes: the association of a formal certificate with a public solution claim

On 8 September 2026, OpenAI announced a result concerning the Navier–Stokes existence and smoothness problem, presenting an analytical write-up together with a Lean formalization (OpenAI, 2026a). The announcement states that the system produced a proof of finite-time singularity formation for a three-dimensional incompressible fluid with smooth external forcing and finite energy, and says that the result establishes alternatives C and D of the official Millennium Prize formulation. It also reports that Lean formalization and verification took an additional seventeen hours after the agents had arrived at their resolution. The public repository describes itself as containing Lean formalizations of the results presented in the two OpenAI papers (OpenAI, 2026b).

The first moment is genuine: the Lean artifacts are formal proof objects checked in the specified environment. The second moment is unusually extensive. OpenAI describes a multi-agent process involving approximately 10,000 concurrent agents, the consolidation of intermediate results, mathematical and AI research work, and a separate formalization phase. The third moment is visible in the announcement’s compact presentation of a “solution” accompanied by a Lean formalization and in the repository’s description of “Lean certificates accompanying” the results.

The relation between the fourth moment and the public claim is more delicate. Bastounis et al. (2026) identify differences between parts of the natural-language proof and the corresponding Lean declarations, including an inverse-estimate discrepancy in Lemma 8.6 and a different pressure-flux estimate and proof route. Their point concerns correspondence between the written argument and the formalized argument. It does not establish that Lean’s kernel failed, that the formal theorem is false, or that the Navier–Stokes result itself is false. A separate public audit of the formal statement explains that the Lean declarations for alternatives C and D are copied from the Clay formulation and that the paper’s Theorem 1.1 is connected to those alternatives by a formal bridge (Cotton, 2026). Thus theorem-statement correspondence and proof-route correspondence must not be conflated: the former concerns what theorem is established; the latter concerns whether the formal proof reproduces the argument in the written paper.

OpenAI’s announcement presents both a write-up and a formalization, while the independent critique makes the relation between these artifacts publicly salient. The case therefore locates a crucial point in the formation mechanism: a formal credential can travel alongside a high-profile mathematical claim, while the relation between the checked declaration and the written proof remains a distinct object of scrutiny. It clarifies the difference between the association of a credential with a solution claim and the stronger public representation of the machine as the autonomous bearer of the entire achievement.

### 5.3 Erdős problems and AlphaProof Nexus: the public attribution of autonomous mathematical achievement

Tsoukalas and colleagues report that their full-featured AlphaProof Nexus agent “autonomously resolved 9 of 353 open Erdős problems” (Tsoukalas et al., 2026, Abstract). Table 1 repeats the formulation, describing the entries as “open problems ... autonomously resolved by our full-featured agent.” The denominator is important: the evaluation ran over 353 formalized statements in the Formal Conjectures repository, not over an independently assembled list of 353 informal problems. The nine results are therefore nine solved formal statements associated with Erdős problems; the paper itself notes variants among the entries and identifies one variant that was not posed by Erdős himself.

The paper also describes the human and semantic work that makes these results count as solutions to mathematical problems. Section 3 states that, after each Erdős solve, experts on the team validated that the Lean statement faithfully captured the original conjecture. The author-contribution statement identifies human roles in selecting problems, validating generated solutions, and writing natural-language proofs. The Discussion presents future mathematical research as a human–machine partnership (Tsoukalas et al., 2026, Sections 1, 3, 6, and Author Contributions). Aarhus University’s institutional report makes this mediation particularly visible: it identifies Gergely Bérczi as the first research mathematician to work with the system, and says that his role included identifying suitable problems, validating the system’s solutions, and co-writing the natural-language versions of the proofs. Yet the university’s headline and opening description continue to say that AlphaProof Nexus “has autonomously resolved” long-standing open problems (Behrend, 2026).

The significance lies in the exact object of the public verb. The technical operation is autonomous formal proof search: once a formal target is available, the agent searches for and generates a Lean proof, and the compiler checks the resulting proof term. The public formulation does not merely say that the agent “autonomously generated Lean proofs” or “completed proof search for nine formal statements.” It says that the agent “autonomously resolved” open mathematical problems. The grammatical object of the verb is therefore the mathematical problem, not the proof term or formal declaration. The public description moves from an autonomous operation within the proof-production process to an attribution of the problem-level achievement to the agent.

This is not a claim that the nine mathematical results are false, that the Lean checks are defective, or that the experts failed to validate the formal statements. The paper explicitly reports that validation. The issue is the distribution of agency in the public account. Problem selection, the correspondence between formal statements and original conjectures, and the production of natural-language proofs are attributed to human researchers; the headline achievement—resolving the problems—is attributed to the autonomous agent. Human mediation is visible, but it is narratively positioned around the machine’s central act of resolution. The machine becomes the apparent autonomous subject of an achievement whose conditions the same communication chain acknowledges as distributed.

The word “autonomous” has a legitimate operational meaning here. The agent can search for and generate a proof without a mathematician constructing each proof step. The ideological effect does not depend on denying this fact. It arises when this narrower operational autonomy becomes the public sign of the whole mathematical achievement. The technical truth of autonomous proof search supports a broader symbolic attribution of autonomous mathematical discovery. The question is not whether the agent performed the proof search; it did. The question is why the public description makes the agent the autonomous resolver of the mathematical problems while simultaneously recording the human work through which the formal targets were selected, interpreted, validated, and explained.

The case can be assessed through the three diagnostic dimensions. **S — Scope extension (agency-attribution form):** the scope of agency attributed to the agent expands from autonomous proof search on formalized targets to autonomous resolution of the mathematical problems as a whole. This is not a claim that the mathematical results lack warrant; the expert validation of the formal statements is explicitly reported. The extension concerns who is publicly represented as having accomplished the result. **O — Objectal displacement:** the agent is the grammatical and symbolic bearer of “resolution,” while human contributions are acknowledged but positioned as selection, validation, and exposition around the machine’s central achievement. The distributed process thus appears publicly as the autonomous accomplishment of the machine. **E — Social efficacy:** this attribution appears in the *Science* abstract and Table 1 and in Aarhus University’s official headline and opening account. These are high-visibility research and institutional forms through which the achievement is announced and recognized. This establishes a public-authority function; it does not require a claim about what every reader believes or a causal claim about audience reception.

A narrower reading remains possible: “autonomously resolved” may be intended to describe the agent’s autonomous proof search after a formal target has been supplied. That reading accurately captures the system’s operational contribution. It does not exhaust the public function of the formulation, because the grammatical object remains the open mathematical problem and the same communication chain identifies the human work required to turn a formal proof into a mathematical result. The ideological analysis concerns this asymmetry of attribution, not the truth or falsity of the proof.

AlphaProof Nexus therefore supplies the article’s positive existence case. It shows how a genuine machine-checked result, produced through distributed human and computational labour, can be publicly attributed to the autonomous machine as the principal subject of mathematical achievement—even while the human and semantic mediation that qualifies this attribution is explicitly acknowledged.

### 5.4 The Liquid Tensor Experiment: acknowledged limits answered by semantic work

The Liquid Tensor Experiment was completed in July 2022. Its public announcement states that the main theorem of liquid vector spaces had been formally verified in Lean and lists the mathematical, formalization, technical, library, and institutional contributions on which the project relied (Mathlib Community, 2022).

The first moment is the completed Lean proof. The second is especially visible: the project depended on a large collective effort, Mathlib, mathematical guidance from Peter Scholze, and contributions from specialists in homological algebra, condensed mathematics, and formalization. The third appears in the public announcement that the experiment had been completed and that the main theorem had been formally verified.

Adam Topaz’s subsequent discussion explicitly raises the semantic question: how can mathematicians be confident that the definitions introduced in Lean are correct? He notes that pathological definitions could make the theorem meaningless—for example, defining Ext to be identically zero. The project’s response was not to ignore this problem while continuing to invoke the certificate. It created an examples folder of sanity checks, designed to be readable by mathematicians with limited Lean experience, so that they could inspect the definitions and gain reasonable confidence that the formal statement captured the intended mathematics (Topaz, 2022).

Liquid Tensor organizes confidence differently. The credential remains important, but its authority is presented together with the semantic work that gives it meaning. The acknowledged possibility of pathological definitions is answered through examples that mathematicians can inspect. The project thus provides a counter-practice in which semantic relations remain visible and are incorporated into the basis of confidence, rather than being condensed into an apparently self-sufficient machine guarantee.

## 6. The Ideological Function of Mathematical Certainty

The cases reveal that the authority of formal verification is neither located in the kernel alone nor detached from it. The kernel supplies a real technical warrant. The mathematical and institutional practices surrounding it make that warrant meaningful and allow it to travel. The ideological question concerns the transformation through which the authority of this wider network comes to appear as a property of the machine-certified object.

The first three moments establish the material and communicative conditions of this transformation. A formal proof is genuinely checked; its production depends on distributed epistemic labour; and scientific communication condenses this labour into a portable credential. These moments explain why “Lean-verified” is credible and why it can circulate. They do not, by themselves, amount to fetishism. The decisive transition occurs when the authority generated by the network appears to reside autonomously in the credential. Condensation makes the result portable; objectal displacement makes the portable sign appear to contain the authority of the whole.

The four encounters illuminate different sides of this transition. Riemann shows how a strong institutional credential can remain attached to a visibly composite warrant. Navier–Stokes makes the relation between a formal declaration and a public solution claim an explicit problem of interpretation. Liquid Tensor shows how semantic scrutiny can remain visible within the practice that supports confidence in a formal result. These cases clarify the conditions under which the credential’s authority is assembled, communicated, and kept connected to the work that sustains it.

AlphaProof Nexus establishes the existential claim concerning the fifth moment. The *Science* paper reports that experts validated the correspondence between Lean statements and original Erdős conjectures; its author-contribution statement records human roles in problem selection, validation of generated solutions, and writing natural-language proofs. Aarhus University’s institutional account likewise identifies human problem selection, solution validation, and exposition, yet retains the autonomous-resolution framing in its headline and opening description. The same public communication chain therefore acknowledges human and semantic mediation while continuing to present the machine as the apparent autonomous subject of the mathematical achievement.

The distinction between operational and symbolic autonomy is crucial. Operationally, the agent searches for and generates a proof of a formalized target without a mathematician constructing each proof step. Symbolically, “autonomously resolved open problems” functions as the public attribution of the mathematical achievement, including the selection and interpretation of the target, validation of its correspondence to the original conjecture, and production of an intelligible mathematical result. The sources identify human work in these latter tasks. The narrower truth of autonomous proof search thus becomes the support for a wider representation of autonomous mathematical discovery. The ideological effect lies in this coexistence: human mediation is publicly acknowledged, yet the machine remains the apparent bearer of the achievement.

The three diagnostic dimensions make the argument explicit. **Scope extension, in its agency-attribution form,** occurs when autonomy in formal proof search is publicly attributed as autonomy in resolving the mathematical problem itself. The point is not that the mathematical result lacks warrant: the paper reports expert validation of the correspondence between the formal statements and the original conjectures. The extension concerns the attribution of agency from one operation within the research process to the problem-level achievement. **Objectal displacement** occurs when the machine is presented as the autonomous subject and bearer of the achievement, while human problem selection, statement validation, and mathematical exposition are acknowledged but positioned around the machine’s central act of resolution. **Social efficacy** is visible in the role of this formulation in the *Science* abstract and table and in the university’s official headline and institutional report. The case therefore satisfies the article’s existential claim at the level of public institutional representation. This does not require a claim about the authors’ private intentions or the beliefs of every reader.

The fifth moment is therefore not a claim that participants are ignorant of the human work involved. It is the opposite. The case shows that acknowledgement does not necessarily dissolve symbolic investment. The machine’s autonomy at the level of proof search can remain the public image through which the whole achievement is represented. **The ideological fetishism of formal verification does not require the concealment of human mediation; it can operate through the very public acknowledgement of that mediation.** This is the article’s central philosophical finding, established as an existence claim rather than a claim about every formalization project.

The distinction between the **warrant of a check** and the **authority of a credential** provides the conceptual hinge. The warrant concerns what the formal system establishes. The credential’s authority concerns how that result is recognized, circulated, and made to count. The credential is grounded in a real technical achievement, but its symbolic authority is produced through the relations that connect the formal artifact to the intended mathematical claim and through the public forms in which the achievement is represented. The machine’s reliability supplies the material support for this authority; it does not by itself explain the authority’s wider social meaning.

This argument enters into conversation with recent work on mathematical warrant and AI-assisted proof. Vallverdú’s Locus Thesis provides a component-based account of mathematical warrant (Vallverdú, 2026). Kallel and El Louadi (2026) distinguish derivational validity, representational fidelity, and epistemic significance, while examining the relation between abundant checking and human adjudication. López-Corona’s account of “studio mathematics” analyzes human-machine assemblages, provenance, agency, and responsibility in AI-assisted proof production (López-Corona, 2026). These works clarify how mathematical warrant is distributed across technical and human practices. The present article adds a Žižekian account of how the authority generated through those practices can become condensed in a portable credential and continue to function as autonomous machine authority even when the human conditions of its production are visible.

Erfani (2026) examines ideological functions of AI systems, while Hourigan (2009) applies Žižek to technological fetishization and knowledge production. Omodeo (2019) develops a political epistemology of ideology in science studies. Against this background, the present article focuses on the specific credential “Lean-verified.” Its contribution is not the general claim that technology can become fetishized, nor the discovery that mathematical knowledge depends on collective labour. It is the reconstruction of a particular mechanism through which a genuinely reliable proof-checking operation becomes the material support for a wider symbolic authority: real technical reliability, distributed epistemic labour, credential condensation, objectal displacement, and the reproduction of symbolic investment through fetishistic disavowal. The phrase “epistemic fetishism” has also been used in a different analytic-epistemological sense by Ahlstrom-Vij (2021); the present article therefore uses the full expression “the ideological fetishism of formal verification” and does not claim to have coined the bare term.

The ideological function of mathematical certainty is not that certainty is false. Formal verification can provide a real and powerful form of certainty. The issue is how this certainty travels and what it is made to authorize. The machine’s reliability is not what ideology must explain away. It is precisely what ideology must explain: how a genuine, bounded technical guarantee becomes the material support for a symbolic authority that appears to exceed the operation which produced it.

## 7. Conclusion

How does the epistemic fetishism of formal verification arise? It begins with a real technical achievement. Lean’s kernel checks proof terms against formal propositions under specified environments. This genuine reliability gives the credential “Lean-verified” its initial force; without it, the credential would have no epistemic substance.

The authority of the credential is assembled through distributed epistemic labour. Mathematical formulation, formal specification, proof construction, library and software maintenance, kernel checking, semantic comparison, expert assessment, and institutional recognition contribute different forms of warrant. Scientific communication condenses this process into a portable sign. As the credential circulates, the relations that give it meaning can recede while the sign remains. Authority generated by the network then appears to reside autonomously in the machine-certified object. This is the fetishistic displacement at the centre of the argument.

AlphaProof Nexus shows how this authority can persist through the public acknowledgement of human mediation. The *Science* paper reports expert validation of the correspondence between Lean statements and original Erdős conjectures and records human contributions to problem selection, solution validation, and natural-language proofs. Aarhus University’s institutional account identifies the same human work, yet retains the description of the system as having autonomously resolved the problems. The machine remains the apparent public bearer of the achievement alongside an explicit account of the human work that makes the result meaningful; the issue is the attribution of agency, not the validity of the results. This is fetishistic disavowal as a structure of public representation: acknowledgement does not automatically dissolve symbolic investment.

The other cases clarify the range of the mechanism. Riemann shows how institutional certification can rest on a visibly composite warrant. Navier–Stokes exposes the significance of the relation between a checked formal declaration and the natural-language proof associated with it. Liquid Tensor shows how semantic scrutiny and collective mathematical labour can remain visible within a formalization project. Their differences make clear that the same technical reliability can enter distinct social and symbolic arrangements.

The article’s central contribution is the concept of the **ideological fetishism of formal verification**: the transformation through which the socially and semantically mediated authority of a machine-checked result appears to reside autonomously in the credential “Lean-verified.” The five-moment account explains how this transformation is formed and reproduced: real technical reliability, distributed epistemic labour, credential condensation, objectal displacement, and fetishistic disavowal. Its decisive philosophical finding is that the fetish does not depend on hiding the human relations that sustain the machine’s authority. It can persist through their public acknowledgement.

The machine’s reliability is not what ideology must explain away. It is precisely what ideology must explain: how a real technical guarantee becomes the material support for a symbolic authority that exceeds the operation which produced it.

The machine verifies a proposition. The philosophical question is what, beyond that proposition, we ask the credential to guarantee.

## Statements and Declarations

**Generative AI use.** ChatGPT (OpenAI; GPT-6.2) was used during preparation of this manuscript to assist with literature discovery, argument development, drafting, and revision. The author is responsible for the final manuscript and for verifying the accuracy of its claims, interpretations, and references.

**Funding.** [Author confirmation required before submission.]

**Competing interests.** [Author confirmation required before submission.]

## References

Ahlstrom-Vij, K. (2021). Esoteric reliabilism. *Episteme, 18*(4), 603–623. https://doi.org/10.1017/epi.2019.39

Alpöge, L. (2026, November 20). *The Riemann hypothesis* [Research note and Lean archive]. https://alpo.ge/

Bastounis, A., Circelli, F., & Hansen, A. C. (2026). *Navier–Stokes lost in translation: Why Lean verification of AI autoformalisation does not guarantee correct natural language proofs* [Preprint]. arXiv. https://doi.org/10.48550/arXiv.2610.08144

Behrend, M. (2026, October 23). *Aarhus mathematician co-authors Google DeepMind breakthrough on machine-verified proofs of open problems*. Aarhus University. https://math.au.dk/en/currently/news/news-item/artikel/gergely-deepmind

Black, J. (2025). Examining the mechanism of disavowal and its two forms: Cynical disavowal and fetishistic disavowal. *Theory & Psychology, 35*(1), 117–135. https://doi.org/10.1177/09593543241308199

Cotton, P. (2026, September 24). *The formal statement*. Navier–Stokes Guide. https://navier.microprediction.org/formal.html

De Millo, R. A., Lipton, R. J., & Perlis, A. J. (1979). Social processes and proofs of theorems and programs. *Communications of the ACM, 22*(5), 271–280. https://doi.org/10.1145/359104.359106

Duede, E., & Davey, K. (2025). A priori knowledge in an era of computational opacity: The role of artificial intelligence in mathematical discovery. *Philosophy of Science, 92*(5), 1394–1404. https://doi.org/10.1017/psa.2025.10160

Emmerson, P. (2026, November 24). *Alpöge’s certified Lean derivation does not prove the Riemann hypothesis: Granting every check, the hypothesis follows from a premise stronger than itself* [Preprint]. Preprints.org. https://doi.org/10.20944/preprints202611.2463.v1

Erfani, F. (2026). Not “just a language model”: AI’s ideological functions. *AI & Society, 41*, 869–881. https://doi.org/10.1007/s00146-025-02623-0

Hardwig, J. (1985). Epistemic dependence. *The Journal of Philosophy, 82*(7), 335–349. https://doi.org/10.2307/2026523

Hourigan, D. (2009). *The phantasmatic subject of technology: Slavoj Žižek, techne, and the abyss* [Doctoral dissertation, Griffith University]. https://doi.org/10.25904/1912/3124

Kallel, M., & El Louadi, M. (2026). *Verification abundance, adjudication scarcity: What happens to mathematical knowledge when proof checking becomes free* [Preprint]. arXiv. https://doi.org/10.48550/arXiv.2608.28997

Kuldova, T. (2019). Fetishism and the problem of disavowal. *Qualitative Market Research: An International Journal, 22*(5), 766–780. https://doi.org/10.1108/QMR-12-2016-0125

Lean FRO & Mathlib Initiative. (2026, November 21). *Lean verification of the Riemann hypothesis* [Joint statement]. https://leanprover-community.github.io/blog/posts/riemann-hypothesis/

López-Corona, O. (2026). *From authorial mathematics to studio mathematics: Ecobiontic forms of proof after large language models* [Preprint]. arXiv. https://doi.org/10.48550/arXiv.2608.22194

Marx, K. (1976). *Capital: A critique of political economy* (Vol. 1; B. Fowkes, Trans.). Penguin Books. (Original work published 1867)

Mathlib Community. (2022, July 15). *Completion of the Liquid Tensor Experiment*. Lean Community Blog. https://leanprover-community.github.io/blog/posts/lte-final/

Mathlib Documentation. (2026). *Mathlib.NumberTheory.LSeries.RiemannZeta: Definition of RiemannHypothesis*. Mathlib4 documentation. https://leanprover-community.github.io/mathlib4_docs/Mathlib/NumberTheory/LSeries/RiemannZeta.html

Omodeo, P. D. (2019). *Political epistemology: The problem of ideology in science studies*. Springer. https://doi.org/10.1007/978-3-030-23120-0

OpenAI. (2026a, September 8). *On the Navier–Stokes Millennium Prize problem*. https://openai.com/index/navier-stokes-solution/

OpenAI. (2026b). *NavierStokesAndEuler: Lean certificates accompanying Navier–Stokes and Euler results* [GitHub repository]. GitHub. https://github.com/openai/NavierStokesAndEuler

rh-lean-roadmap. (2026, November 26). *The Riemann hypothesis and GRH for Dirichlet L-functions: A readable account of the Lean proof in Alpöge’s archive* (Version 44) [Zenodo record]. https://doi.org/10.5281/zenodo.24562451

Scholze, P. (2021, June 5). *Half a year of the Liquid Tensor Experiment: Amazing developments*. Xena Project. https://xenaproject.wordpress.com/2021/06/05/half-a-year-of-the-liquid-tensor-experiment-amazing-developments/

Sloterdijk, P. (1987). *Critique of cynical reason* (M. Eldred, Trans.). University of Minnesota Press. (Original work published 1983)

Sutherland, A. (2026a, November 25). *Verification files for the Lean proof of the Riemann hypothesis*. Massachusetts Institute of Technology. https://math.mit.edu/~drew/grh/

Sutherland, A. (2026b, November 26). *Shorter Lean proof of RH and GRH for Dirichlet L-functions: Verification files*. Massachusetts Institute of Technology. https://math.mit.edu/~drew/shortgrh/

Topaz, A. (2022, October 14). *Definitions in the Liquid Tensor Experiment*. Lean Community Blog. https://leanprover-community.github.io/blog/posts/lte-examples/

Tsoukalas, G., Kovsharov, A., Shirobokov, S., Surina, A., Firsching, M., Bérczi, G., Ruiz, F. J. R., Suggala, A., Wagner, A. Z., Wieser, E., Yu, L., Huang, A., Horváth, M. Z., Ferraiuolo, A., Michalewski, H., Grosu, C., Lockhart, E., Hubert, T., Balog, M., . . . Chaudhuri, S. (2026). Advancing mathematics research with AI-driven formal proof search. *Science, 394*(6820), 234–239. https://doi.org/10.1126/science.aej2213

Vallverdú, J. (2026). Where does mathematical warrant live? From the Four-Color Theorem to mass-released AI “results”. *Philosophies, 11*(6), Article 224. https://doi.org/10.3390/philosophies11060224

Žižek, S. (1989). *The sublime object of ideology*. Verso.

Žižek, S. (1994). The spectre of ideology. In S. Žižek (Ed.), *Mapping ideology* (pp. 1–33). Verso.
