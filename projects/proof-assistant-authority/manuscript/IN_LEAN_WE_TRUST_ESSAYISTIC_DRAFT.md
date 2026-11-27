# In Lean We Trust? The Ideology of Machine-Checked Proofs in Science

**Project:** *In Lean We Trust?*  
**Version:** Essayistic philosophical draft  
**Evidence cut-off:** 27 November 2026  
**Genre:** Philosophical argument with comparative case analysis

## Abstract

What could be ideological about a correct proof? Lean’s kernel provides genuine and bounded warrant for a specified formal proposition under a specified environment. The question is how this local technical achievement can become a bearer of wider mathematical authority. Drawing on Slavoj Žižek’s critique of ideology, this article reconstructs a five-moment mechanism: real technical reliability; distributed epistemic labour; the condensation of that labour into the portable credential “Lean-verified”; the objectal displacement through which network-generated authority appears to reside autonomously in the credential; and, conditionally, fetishistic disavowal through which symbolic investment can reproduce that authority after its limits are known. The article develops this account as the **ideological fetishism of formal verification**. Four encounters with Lean—the Riemann hypothesis, Navier–Stokes, Erdős problems investigated with AlphaProof Nexus, and the Liquid Tensor Experiment—trace contrasting configurations of certification, semantic mediation, and institutional recognition. The cases show that the first four moments can be identified in different combinations, while the fifth requires a more demanding conjunction of acknowledged limits and continued investment beyond them. AlphaProof Nexus offers the clearest borderline case: its account of autonomous proof search coexists with explicit human validation of the formal statements. The Liquid Tensor Experiment, by contrast, shows how semantic scrutiny can interrupt the displacement of authority into the machine credential. The article thus explains how a genuine technical warrant may acquire a symbolic surplus, while distinguishing fetishistic disavowal from rational reliance on a well-specified formal check.

**Keywords:** philosophy of science; philosophy of mathematical practice; social epistemology; political epistemology; Slavoj Žižek; ideology critique; formal verification; Lean; fetishism; mathematical proof

---

## 1. The Paradox of a Verified Proof

What is ideological about a correct proof?

Imagine that a mathematical proposition has been formalized, a proof term has been constructed, and Lean’s kernel accepts it. There is no need to look for a hidden failure in the machine. The proof assistant has performed the task for which it was designed. Under the specified formal environment, the term has the required type. The result is reproducible, inspectable, and, in principle, independently checkable. Why, then, should we speak of ideology? Would this not confuse a genuine mathematical achievement with a social illusion?

The question becomes difficult only when we abandon a familiar conception of ideology. If ideology means false consciousness, then the answer seems immediate: there is nothing ideological about a correct proof. One either has a valid derivation or one does not. Once the relevant facts are established, the ideological appearance should disappear.

But this is precisely the point at which Žižek’s critique becomes relevant. Ideology cannot always be identified by asking whether an explicit proposition is true or false. A statement may be factually correct and nevertheless participate in an ideological relation through the position it occupies and the practice it helps sustain (Žižek 1989; 1994). The question is not simply whether Lean’s verdict is correct. It is what this verdict is made to authorize.

Consider the difference between two statements:

> Lean’s kernel accepts a proof term for the formal proposition \(P^*\).

and

> The mathematical problem has been conclusively solved.

The first statement identifies a technical result. The second makes a claim about a mathematical achievement whose warrant may involve much more: the identity of \(P^*\) with the intended theorem, the adequacy of its definitions and assumptions, the relation between a formal artifact and a natural-language argument, and the status of the result within mathematical practice. The first does not automatically entail the second. Yet the public credential “Lean-verified” can travel between them, sometimes without the intervening relations being made visible.

The paradox is therefore not that a machine produces false certainty. It is that a machine may produce a genuine form of certainty, sharply bounded in its technical operation, while the credential associated with that achievement comes to signify something wider. The machine does not have to be unreliable for its authority to acquire an ideological function. On the contrary, its genuine reliability may be what makes the wider symbolic investment possible. A defective instrument could hardly serve as a convincing bearer of certainty.

This article asks how that transformation can occur. Its object is not Lean software in general, nor the psychological question of whether mathematicians trust machines. It is the public and institutional credential **“Lean-verified”**: the compact sign through which a complex formal and mathematical process becomes recognizable as a warrant for a result. The central hypothesis is that this credential may acquire an ideological function when the authority generated through a network of technical, semantic, and institutional relations appears to reside autonomously in the verification object itself.

The argument is not that formal verification is a deception, that mathematical truth is merely socially constructed, or that reliance on a proof assistant is irrational. A mathematician who relies on Lean for the task it actually performs may be entirely justified. Nor is every short description of a formal proof an instance of ideological distortion. The issue is more specific: under what conditions does a bounded technical credential become a symbolic guarantee of a wider mathematical claim, and what happens to the relations that connect the credential to that claim?

The question is worth asking because formal verification makes one part of mathematical warrant unusually visible. A proof may be extremely long, technically complex, and difficult for any individual mathematician to survey. Yet the result of kernel checking can be stated in a compact form. The complexity of the proof does not disappear; it becomes condensed in a portable credential. The word “verified” can then function as a point at which the otherwise distributed process of mathematical knowledge production seems to arrive at a final answer.

The following pages approach this problem through Žižek’s account of ideological fantasy and fetishism. The former helps explain how a local check can stage the appearance of closure; the latter helps explain how the authority generated by a network of relations can appear as an autonomous property of an object. Disavowal will enter only as a secondary possibility: it may help explain why symbolic investment persists even when limitations are acknowledged, but it is not necessary for every instance of fetishistic displacement.

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

This distinction is now central to the philosophy of mathematical warrant. Vallverdú’s Locus Thesis argues that properties such as reliability, surveyability, transferability, and explanatory power should be assigned to components of a warrant architecture, rather than indiscriminately predicated of a proof as a whole (Vallverdú 2026). Kallel and El Louadi (2026) similarly distinguish derivational validity, representational fidelity, and epistemic significance. They argue that the abundance of machine-checked proofs does not remove the need for human adjudication; it changes where that adjudication is required.

The present article adopts this component-based account. It does not claim originality for the distinction between a formal proposition, a proof object, a checking procedure, a trusted base, and the intended mathematical claim. Nor does it claim that the gap between formal and informal mathematics is unbridgeable. The relevant point is more modest and more consequential: the warrant supplied by a kernel check is one component of a wider architecture, and the authority of the whole cannot simply be read off from the reliability of that component.

The same caution applies to the social organization of mathematics. A mathematician cannot personally reproduce every piece of software, inspect every library dependency, and independently reconstruct every proof used in a large formalization. Nor should this be expected. Scientific knowledge depends on a division of epistemic labour. Hardwig’s account of epistemic dependence explains why reliance on experts can be rational even when the person relying on them cannot personally reproduce their evidence (Hardwig 1985). De Millo, Lipton, and Perlis (1979) likewise emphasize that mathematical proof operates within social processes of criticism, communication, and acceptance.

There is nothing ideological merely in relying on Lean, trusting a competent formalizer, or accepting a well-documented institutional review. Such reliance can be rational. A journal may reasonably require a formal artifact; a mathematician may reasonably rely on independent kernel checking; a reader may reasonably trust experts who have compared a formal proposition with its intended statement.

This is where the problem becomes more precise. Social mediation is not ideology. Distributed labour is not fetishism. Institutional recognition is not automatically a distortion. The ideological question arises only when the credential associated with one component of the warrant architecture is made to appear as if it contains the authority of the whole. The problem is not that the machine checks something. It is that the result of this check may become the visible bearer of a certainty that depends on relations extending beyond the check itself.

## 3. Žižek and the Ideological Structure of Verification

### 3.1 Ideology beyond false consciousness

In “The Spectre of Ideology,” Žižek shifts the question of ideology away from the simple opposition between true and false beliefs (Žižek 1994). The ideological function of a proposition cannot be read directly from its truth value. A statement may be factually correct and nevertheless participate in an ideological relation through the position it occupies and the practice it helps sustain. What matters is not only whether a statement is true, but how its truth is mobilized within a social order.

“Lean checked this proof” may be entirely accurate. Its philosophical significance emerges when this true statement becomes the point through which a wider mathematical claim is authorized. The credential can remain attached to the formal proposition and the conditions under which it was checked; it can also travel as if it carried the authority of the entire mathematical result. The same technical fact can therefore occupy different positions within the production of knowledge.

Žižek’s account directs attention beyond explicit discourse. In “The Spectre of Ideology,” he distinguishes ideology as doctrine, its material externality in practices and institutions, and its more elusive spontaneous operation within social reality (Žižek 1994, 9–10). Applied to formal verification, this means that the credential must be studied across the settings in which it acquires force: the repository in which a proof is checked, the paper that reports it, the institution that recognizes it, and the practices through which mathematical credibility is distributed. Ideology is not simply a mistaken sentence about a machine. It concerns the relation between what is said, what is materially done, and what becomes authoritative.

### 3.2 Ideological fantasy: the scene in which uncertainty appears to end

In *The Sublime Object of Ideology*, fantasy is not merely a false image concealing an otherwise complete reality. It supplies the coordinates through which reality is experienced and sustains the appearance of coherence where a constitutive gap remains (Žižek 1989, 28–31). Fantasy organizes the scene in which a practice becomes intelligible and an incomplete relation can appear whole.

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

The more decisive theoretical move comes from Marx’s account of commodity fetishism. In *Capital*, Volume I, Chapter 1, Section 4, Marx analyzes how relations among producers assume the appearance of relations among things. Žižek’s discussion emphasizes how an effect generated by a network of relations can appear as an immediate property of an object (Žižek 1989, 19–20).

The analogy with formal verification is structural. Mathematical truth is not produced by collective labour in the same way that commodities are produced, and Lean is not a commodity in Marx’s technical economic sense. The relevant structure is the appearance of a relation-dependent authority as an intrinsic property of an object.

The authority of a Lean-verified result depends on a network: the problem is selected and formulated; definitions and assumptions are chosen; the intended theorem is represented formally; a proof object is constructed; libraries and software infrastructure are maintained; the kernel checks the proof term; experts examine the specification relation; institutions and mathematical communities assess the result’s status. These activities contribute different forms of warrant. Their combined authority is what allows the formal artifact to count as a proof of a particular mathematical claim.

The fetishistic possibility appears when the authority generated through this network seems to reside autonomously in the verification credential itself. The credential appears not merely to report that one component of the proof process has succeeded, but to contain the authority of the whole. The relation is inverted: the network makes the credential meaningful, yet the credential appears as the source that certifies the network.

Fantasy and fetishism therefore do different work. Fantasy supplies the scene in which the local check appears to close the wider question. Fetishism gives this appearance an objectal form: the closure seems to reside in the credential itself. The first concerns the staging of completeness; the second concerns the apparent location of the authority that completeness promises. They reinforce one another, but they are not interchangeable.

### 3.4 Disavowal and the persistence of symbolic investment

Žižek’s discussion of cynical ideology draws on Peter Sloterdijk’s critique of cynical reason (Sloterdijk 1987; Žižek 1989, ch. 1). The familiar formula that subjects know what they are doing and nevertheless continue to do it should not be presented as Žižek’s original coinage. What matters for the present argument is the distinction between cynical and fetishistic disavowal, developed in recent work by Kuldova (2019) and Black (2025, 118–119).

Cynical disavowal maintains a distance between what an actor knows and what the actor publicly or practically does, often by obscuring that distance. Fetishistic disavowal has a different structure. The subject can acknowledge both the objective state of affairs and the way in which the object nevertheless continues to appear and function. Knowledge does not simply dissolve the investment. The subject knows, and nonetheless continues.

In the context of formal verification, the relevant formula is not that mathematicians mistakenly believe Lean proves more than it does. A researcher may know perfectly well that the kernel checks a proof term for \(P^*\) under \(\Gamma\), and that the relation between \(P^*\) and the intended claim \(P\) is a distinct task. The question is whether this knowledge changes the practical and symbolic use of the credential. A researcher who relies on Lean for precisely the proposition it checks is engaged in rational epistemic dependence. The fetishistic possibility appears when the same credential continues to function as a broader sign of mathematical closure or authority, despite explicit knowledge that its technical warrant is narrower.

Disavowal therefore explains the persistence of symbolic investment, rather than the initial production of the credential. It is not necessary for every instance of objectal displacement. It becomes important when the credential continues to organize recognition and action after its limits have been acknowledged. The point is not necessarily conscious deception or hypocrisy. It is a split between what is known about the warrant and what the credential continues to make possible in practice.

The Lacanian idea that there is no complete Big Other and no “Other of the Other” provides a background to this argument (Lacan 2019, ch. XVI; Žižek 1989, Part II). No final symbolic authority guarantees the consistency of the entire order from outside it. The significance for formal verification is not that mathematical proof lacks foundations, but that the credential may be invested with the function of a final guarantee even when its technical scope is explicitly understood.

## 4. The Machine as a Fetish Object

How does the credential “Lean-verified” acquire authority beyond the technical operation it records? The answer is not that a machine suddenly becomes an object of irrational admiration, nor that a community simply mistakes a technical procedure for something it is not. The process is more interesting: a real technical achievement is produced through distributed labour, condensed into a portable sign, and then made to carry a symbolic authority that appears to belong to the sign itself.

The formation and reproduction of the epistemic fetish can be reconstructed through five connected moments. They are analytically ordered, not a rigid chronology. The first two provide the material conditions; the third gives the achievement a portable form; the fourth marks the specifically fetishistic conversion; and the fifth explains how that authority may be reproduced after its limits are known. The fifth moment is therefore a feedback mechanism, not a necessary stage through which every use of Lean must pass.

**First, the check has real technical efficacy.** Lean’s kernel does not merely symbolize reliability. It checks whether a proof term has the required type for a specified formal proposition under a specified environment. The result can be replayed, inspected, and, in appropriate settings, checked independently. This is the material basis of the credential’s credibility. The ideological function of formal verification does not arise because the machine fails to do its job. It becomes possible because the machine genuinely does something valuable. Its reliability is not an illusion that must be exposed; it is the real achievement around which a wider symbolic investment can gather.

**Second, the achievement is produced through distributed epistemic labour.** The formal result depends on more than the kernel. A mathematical problem must be selected and formulated; definitions and assumptions must be chosen; the intended claim must be represented as a formal proposition; a proof must be found and encoded; libraries and software tools must be developed and maintained; the trusted environment must be specified; the formal statement must be compared with the intended theorem; and the result must be interpreted and assessed by mathematicians, reviewers, and institutions. These activities are distributed across people, technical systems, and organizations. They contribute different kinds of epistemic work, and no single component performs the whole task.

This distribution is not a defect in mathematical knowledge. It is a condition of contemporary mathematical practice. It means that the authority of a result is assembled across a network whose full operation may not be visible to any one participant. The result depends on relations of expertise, maintenance, interpretation, and institutional recognition. The technical check is one indispensable component within this larger arrangement. Whether these relations remain visible or recede from view becomes decisive later in the argument.

**Third, scientific communication condenses this distributed process into a credential.** A complex mathematical achievement must travel. It appears in an abstract, a paper title, a repository description, a journal announcement, a university news item, a conference presentation, or a media report. These forms cannot reproduce the entire history of formalization and review. They need a compact way to identify what has been accomplished. “Lean-verified” performs this communicative function. It condenses theorem formulation, formal specification, proof construction, kernel checking, and layers of human scrutiny into a single portable status.

Condensation is necessary for communication. It is not yet fetishism. A concise statement can preserve the scope of the check, and a credential can accurately summarize a complex process. The decisive question is what happens when the condensed sign begins to circulate as if it contained the authority of the relations that initially fixed its meaning.

**Fourth, the credential acquires symbolic authority through objectal displacement.** As “Lean-verified” moves across contexts, the exact formal proposition, environment, assumptions, dependencies, and specification relation may become less visible, while the credential itself remains. The sign travels more easily than the network that supports it. It can then appear not merely as a report that one component of a warrant architecture has succeeded, but as an autonomous guarantee of the result as a whole.

Here the relation is inverted. The network makes the credential meaningful, yet the credential appears as the source that certifies the network. Authority generated through mathematical judgement, formalization, software infrastructure, checking, and institutional assessment seems to reside in the machine-certified object. The local warrant of the kernel is thereby given a symbolic surplus: “Lean-verified” can come to signify not only that a formal proposition has been checked, but that the wider mathematical claim is secure, settled, and institutionally authoritative. This is the specifically fetishistic moment. The object appears to possess, as its own property, an authority that in fact depends on the relations that produced and interpreted it.

Three questions help distinguish this displacement from ordinary shorthand. **Scope extension** asks whether the credential is made to warrant more than the checked proposition and its documented relation to the intended claim. **Objectal displacement** asks whether the authority generated through the network appears to reside autonomously in the credential. **Social efficacy** asks whether this representation has a recognizable role in legitimation, recognition, credibility allocation, or institutional practice. A short announcement may condense a complex process without extending its scope; a visible credential may circulate without being treated as self-sufficient; and a symbolic representation may appear without having a discernible practical effect. The fetishistic diagnosis concerns their conjunction, not any one feature in isolation.

**Fifth, fetishistic disavowal can reproduce this authority despite knowledge of its limits.** This moment requires more than awareness that Lean has a technical scope. A mathematician may know that the kernel checks a proof term for \(P^*\) under \(\Gamma\), and rely on it for precisely that task. This is rational epistemic dependence, not disavowal. The stronger structure appears when an actor or institution recognizes that the credential is being asked to warrant more than the check establishes, yet continues to mobilize it in that broader role.

The distinction can be stated schematically:

\[
\text{knowledge of the boundary}
+
\text{continued investment beyond the boundary}
\]

is the relevant structure of fetishistic disavowal. In a public case, the two elements must be linked: the same actor or institutional communication chain must acknowledge the precise limitation and continue to use the credential as a wider sign of mathematical closure or authority. A generic statement that AI systems can make mistakes is not enough. Nor is a technical qualification followed by a claim that is independently supported by expert semantic review. If the relation between \(P^*\) and the intended claim \(P\) has been separately established, the broader claim may be warranted by the whole network rather than fetishistically attributed to the kernel.

This is not the same as cynical disavowal. Cynicism may conceal or manipulate the distance between knowledge and action. Fetishistic disavowal can openly acknowledge the limitation while continuing to act through the symbolic object that appears to overcome it. The subject knows not only that the check is local, but that the credential continues to function as a wider guarantee; nevertheless, the investment persists. The knowledge of the limit and the investment in the object occupy different registers.

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
\underbrace{\text{Acknowledged boundary}
+\text{continued investment beyond it}}_{\text{Fetishistic disavowal}}
\quad\circlearrowleft\quad
\text{reproduction of symbolic authority}.
\]

This is not a mechanical law, nor does every use of a formal verification system pass through each moment in the same way. The first four moments explain how a bounded technical achievement can become an object of wider epistemic authority. The fifth explains how that authority may be reproduced despite explicit knowledge of its limits. The machine’s reliability remains real throughout this process. What changes is the symbolic work that its credential is made to perform.

The fetish, then, is not simply the machine, and it is not a false belief about the machine. It is the credential through which the authority of a distributed epistemic network appears to be contained in a single object. Fetishistic disavowal is one possible way this appearance is sustained, not a condition that must be presumed whenever a machine-checked proof is trusted.

## 5. Four Encounters with Formal Verification

The following cases are not a representative survey of Lean use, nor are they matched controls. They expose different relations between a formal artifact and the mathematical claim associated with it. Each is examined through the five moments: what the checker actually establishes; how the result depends on distributed labour; how the achievement is condensed into a credential; where authority appears to reside; and whether acknowledged limits coexist with continued investment beyond them.

### 5.1 The Riemann Hypothesis: a credential whose warrant remains visible

On 20 November 2026, Levent Alpöge released a note and a large Lean development concerning the Riemann hypothesis (Alpöge 2026). The Lean FRO and Mathlib Initiative issued a joint statement on 21 November expressing “full confidence” in the proof and stating that the community certified both the statement and the proof (Lean FRO and Mathlib Initiative 2026).

The first moment is unusually strong. The formal development compiles; the exported proof is accepted by Lean’s kernel and independent checkers; and Sutherland’s report records 175,187 compiling modules, independent kernel replay, and statement comparisons (Sutherland 2026a). The second moment is equally visible. The result depends on Mathlib, formalization work, expert review of the theorem statement, community compilation, independent checker implementations, and further mathematical exposition. The joint statement does not conceal these contributions. It identifies them as the basis of its certification.

The third moment appears in the public credential “Lean verification of the Riemann Hypothesis” and in the statement’s declaration of “full confidence.” The fourth moment is therefore present as institutional condensation: a complex network of checking and expert assessment is made communicable through the status of a certified Lean proof. Yet the same statement enumerates the distinct grounds of certification. It says that experts vetted the Mathlib statement, that independent tools confirmed the theorem proved in the archive is exactly that statement, and that multiple checkers accepted the exported proof. The authority is attached to the credential, but its basis remains visibly distributed. The statement does not present kernel acceptance as the sole source of the broader mathematical judgement.

A substantial exposition appeared on 26 November. The rh-lean-roadmap project provides a 497-page main text, 963 pages of longer proofs, a 122-page index, and a short roadmap. Its documentation states that several AI models generated the exposition from the Lean source and cross-checked it (rh-lean-roadmap 2026). This is a readable, AI-mediated mathematical account, not a conventional independently authored paper. The joint statement itself looks forward to further mathematical work explaining the new ideas. That continuing need for explanation does not negate the certification; it distinguishes formal warrant from mathematical understanding.

Parker Emmerson’s non-peer-reviewed preprint of 24 November challenges the foundational interpretation of what the certification establishes (Emmerson 2026). It grants the existence of the Lean derivation and reported checks but disputes what follows from them. This is a public challenge to the meaning of the certification, not evidence that the certifying institutions had acknowledged an unresolved defect and continued to use the credential as an overextended guarantee.

The fifth moment is not established here. The certifying statement explicitly addresses the relation between the formal proposition and the intended theorem through expert vetting and independent comparison. Its “full confidence” is presented as the conclusion of a composite process, not as a claim that the kernel alone settles every foundational question. The Riemann case therefore shows powerful institutional authorization and credential condensation, while also showing how visible mediation can prevent the credential from appearing as an autonomous source of authority.

### 5.2 Navier–Stokes: the association of a formal certificate with a public solution claim

On 8 September 2026, OpenAI announced a result concerning the Navier–Stokes existence and smoothness problem, presenting an analytical write-up together with a Lean formalization (OpenAI 2026a). The announcement states that the system produced a proof of finite-time singularity formation for a three-dimensional incompressible fluid with smooth external forcing and finite energy, and says that the result establishes alternatives C and D of the official Millennium Prize formulation. It also reports that Lean formalization and verification took an additional seventeen hours after the agents had arrived at their resolution. The public repository describes itself as containing Lean formalizations of the results presented in the two OpenAI papers (OpenAI 2026b).

The first moment is genuine: the Lean artifacts are formal proof objects checked in the specified environment. The second moment is unusually extensive. OpenAI describes a multi-agent process involving approximately 10,000 concurrent agents, the consolidation of intermediate results, mathematical and AI research work, and a separate formalization phase. The third moment is visible in the announcement’s compact presentation of a “solution” accompanied by a Lean formalization and in the repository’s description of “Lean certificates accompanying” the results.

The relation between the fourth moment and the public claim is more delicate. Bastounis, Circelli, and Hansen (2026) identify differences between parts of the natural-language proof and the corresponding Lean declarations, including an inverse-estimate discrepancy in Lemma 8.6 and a different pressure-flux estimate and proof route. Their point concerns correspondence between the written argument and the formalized argument. It does not establish that Lean’s kernel failed, that the formal theorem is false, or that the Navier–Stokes result itself is false. A separate public audit of the formal statement explains that the Lean declarations for alternatives C and D are copied from the Clay formulation and that the paper’s Theorem 1.1 is connected to those alternatives by a formal bridge (Cotton 2026). Thus theorem-statement correspondence and proof-route correspondence must not be conflated: the former concerns what theorem is established; the latter concerns whether the formal proof reproduces the argument in the written paper.

OpenAI’s announcement presents both a write-up and a formalization. It does not explicitly say that Lean alone verifies every step of the natural-language paper. The independent critique makes the distinction between a checked formal proof and the argument in the write-up publicly salient, but it is authored by a different group. The public record examined here does not show OpenAI acknowledging the specific proof-correspondence critique and then continuing to use the Lean credential as a guarantee that the written argument itself has been checked.

Navier–Stokes is therefore an important case of credential association and possible scope ambiguity, not a demonstrated instance of fetishistic disavowal. The announcement allows the formal certificate to travel alongside a high-profile mathematical claim; the separate artifacts and the later critique make the relation between them a matter for scrutiny. The fifth moment, however, cannot be inferred by transferring the critics’ knowledge to the institution they criticize.

### 5.3 Erdős problems and AlphaProof Nexus: autonomy alongside acknowledged mediation

Tsoukalas and colleagues report that AlphaProof Nexus resolved nine of 353 formalized Erdős problems and produced proofs for 44 of 492 OEIS conjectures attempted (Tsoukalas et al. 2026). The *Science* article explicitly acknowledges that LLM-generated natural-language proofs can contain subtle errors and require expert review. It presents Lean-based formal proof generation as a way to check every logical step. More importantly, it states that after each Erdős problem was solved, experts on the team validated that the Lean statement faithfully captured the original conjecture. For the OEIS tasks, the authors describe test lemmas designed to guard against misformalization and a manual review of the 44 conjectures judged correctly formalized and previously unproven.

The first moment is the real checking of formal proof terms. The second is explicit: the agent’s proof search operates through subagents, language models, Lean, AlphaProof, evolutionary search, mathematical libraries, and human validation. The third appears in the abstract’s claim that the agent “autonomously resolved” nine open Erdős problems and in its description of the results as evidence for “autonomous mathematical discovery.” The same article, however, makes the human statement-validation process visible.

This is the clearest public co-presence of acknowledged mediation and autonomy language among the four cases. It is therefore the strongest candidate for examining the fifth moment. The authors know that formal proof search alone does not settle whether a formal statement captures the original conjecture; they report an expert check of precisely that relation. Yet the abstract continues to describe the results as autonomously resolved.

The interpretation turns on what “autonomous” means. If it means that the agent autonomously searched for and generated proof terms, the description is compatible with subsequent expert validation of the statements. If it is read as claiming that the entire epistemic achievement—from problem interpretation through semantic validation to mathematical recognition—was autonomous, the public framing carries a wider symbolic force than the documented workflow supports. The paper’s own account supplies the qualification, so the stronger reading cannot simply be attributed to the authors as their intended claim. The case is consequently a genuine borderline instance: explicit knowledge and continued autonomy language coexist, but whether the language exceeds the stated division of labour remains open to interpretation.

A source-level audit also identifies link and provenance issues for several published artifacts (Erdős Problems Research Library 2026). These concern the identity and traceability of particular formal files, not kernel failure or the invalidity of all reported results. They reinforce the importance of connecting each public claim to the exact statement and artifact that supports it.

AlphaProof Nexus thus shows how a credential can be condensed into a narrative of autonomous discovery even while the publication records the human work required to validate its meaning. It is the most promising case for testing fetishistic disavowal, but the distinction between autonomous proof search and autonomous epistemic authority must remain explicit. The two are not identical.

### 5.4 The Liquid Tensor Experiment: acknowledged limits answered by semantic work

The Liquid Tensor Experiment was completed in July 2022. Its public announcement states that the main theorem of liquid vector spaces had been formally verified in Lean and lists the mathematical, formalization, technical, library, and institutional contributions on which the project relied (Mathlib Community 2022).

The first moment is the completed Lean proof. The second is especially visible: the project depended on a large collective effort, Mathlib, mathematical guidance from Peter Scholze, and contributions from specialists in homological algebra, condensed mathematics, and formalization. The third appears in the public announcement that the experiment had been completed and that the main theorem had been formally verified.

Adam Topaz’s subsequent discussion explicitly raises the semantic question: how can mathematicians be confident that the definitions introduced in Lean are correct? He notes that pathological definitions could make the theorem meaningless—for example, defining Ext to be identically zero. The project’s response was not to ignore this problem while continuing to invoke the certificate. It created an examples folder of sanity checks, designed to be readable by mathematicians with limited Lean experience, so that they could inspect the definitions and gain reasonable confidence that the formal statement captured the intended mathematics (Topaz 2022).

This is a case in which the fourth moment is actively resisted. The credential remains important, but its authority is presented together with the semantic work that gives it meaning. The fifth moment is not established: acknowledged limits coexist with continued confidence, but the confidence follows additional scrutiny that addresses the identified problem. This is rational reliance on a broader warrant architecture, not fetishistic disavowal.

Liquid Tensor therefore provides a counter-practice. It shows that the condensation of collective labour into a formal verification credential need not result in the autonomous appearance of machine authority. The semantic relations can be made visible, inspected, and incorporated into the basis of confidence.

## 6. The Ideological Function of Mathematical Certainty

The four encounters show that the five-moment mechanism is not a sequence that every formalization project traverses in the same way. The first moment—the real efficacy of the check—is present throughout. The second—the distribution of epistemic labour—is equally pervasive, though its visibility differs. The third—the condensation of that labour into a portable credential—appears whenever a formal result is communicated beyond the immediate setting in which it was produced. The decisive variation concerns the fourth and fifth moments: whether the credential comes to appear as an autonomous bearer of authority, and whether that appearance is reproduced despite acknowledged limits.

The Riemann hypothesis case demonstrates that strong institutional authority need not be fetishistic. The Lean FRO and Mathlib Initiative issue a powerful certification, but the statement itself identifies expert vetting, exact comparison with the formal proposition, successful compilation, and independent proof checking. The credential condenses a substantial network, yet the network remains visible as the basis of the authority it carries. The case therefore distinguishes institutional force from objectal displacement.

Navier–Stokes reveals a different tension. OpenAI’s public announcement associates a Lean formalization with a high-profile mathematical solution claim, while an independent critique identifies differences between the formal proof and parts of the natural-language argument. The formal theorem’s relation to the Clay alternatives and the correspondence between proof routes are distinct questions. The public record supports analysis of credential association and possible scope ambiguity, but it does not show that OpenAI acknowledged the specific critique and continued to use Lean as a guarantee of the written argument. The case therefore illuminates the site at which objectal displacement might occur without supplying direct evidence of fetishistic disavowal.

AlphaProof Nexus provides the clearest borderline case. The same publication acknowledges the unreliability of natural-language outputs, records human validation of the correspondence between formal statements and original conjectures, and nevertheless describes the results as autonomous resolution and autonomous mathematical discovery. The autonomy claim may be read narrowly as referring to proof search, in which case it is compatible with later expert validation. Read more broadly as a claim about the autonomy of the entire epistemic achievement, it carries a symbolic surplus. The case shows how the fifth moment can become visible in public language, but also why the scope of the autonomy claim must be interpreted rather than presumed.

Liquid Tensor offers the counter-practice. Its participants explicitly recognize that formal definitions can be pathological and respond by making semantic sanity checks available to mathematicians. The continued confidence in the formal result is grounded in this additional work. Here knowledge of a limit does not coexist with an unqualified investment in the machine credential; it leads to further scrutiny of the relations that make the credential meaningful.

The comparison therefore yields a precise result. Public materials clearly document the real reliability of Lean, the distributed labour that sustains formal verification, and the condensation of that labour into portable credentials. They also reveal settings in which the credential acquires considerable institutional or symbolic authority. The fifth moment requires more: the same actor or institutional communication chain must acknowledge that the credential is being asked to warrant more than the check establishes and nevertheless continue to mobilize it in that broader role. AlphaProof Nexus approaches this condition most closely, but the meaning of “autonomous” remains open because the authors explicitly distinguish proof search from human validation of the formal statement. The other cases either make the warrant network visible, fail to establish actor-level continuity, or answer the acknowledged limitation through additional semantic work.

This result sharpens rather than weakens the theoretical contribution. Fetishistic disavowal is not another name for trusting a machine after learning how it works. Nor is every public claim of autonomous discovery a symptom of ideology. The concept identifies a more specific structure: a credential whose authority is known to exceed its technical warrant, yet whose wider symbolic function is maintained in practice. The five-moment mechanism explains how such an object can emerge and how its authority may be reproduced; the cases show the different conditions under which that reproduction is visible, contested, or interrupted.

The theoretical contribution lies in distinguishing the **warrant of a check** from the **authority of a credential**. The first concerns what the formal system establishes. The second concerns how that result is recognized, circulated, and made to count. A credential can report a real technical achievement while also becoming the bearer of a wider symbolic authority. The ideological question is how that surplus authority is produced: how the relations that sustain the check are condensed into an object that appears to possess its authority in itself, and how this appearance can be reproduced even when its limits are known.

This argument enters into conversation with recent work on mathematical warrant and AI-assisted proof. Vallverdú’s Locus Thesis provides a component-based account of mathematical warrant (Vallverdú 2026). Kallel and El Louadi (2026) distinguish derivational validity, representational fidelity, and epistemic significance, while examining the relation between abundant checking and human adjudication. López-Corona’s account of “studio mathematics” analyzes human-machine assemblages, provenance, agency, and responsibility in AI-assisted proof production (López-Corona 2026). These works clarify how mathematical warrant is distributed across technical and human practices. The present argument adds a Žižekian question about the form in which the authority generated through those practices appears and circulates.

Erfani (2026) examines ideological functions of AI systems, while Hourigan (2009) applies Žižek to technological fetishization and knowledge production. Omodeo (2019) develops a political epistemology of ideology in science studies. Against this background, the present article focuses on a specific object: the credential “Lean-verified.” Its contribution is to explain how the genuine warrant of formal checking can become a symbolic bearer of wider mathematical authority, and how fetishistic disavowal may sustain that authority even after its technical limits are understood. The phrase “epistemic fetishism” has also been used in a different analytic-epistemological sense by Ahlstrom-Vij (2021); the present article therefore uses the full expression “the ideological fetishism of formal verification” and does not claim to have coined the bare term.

The ideological function of mathematical certainty is not that certainty is false. Formal verification can provide a real and powerful form of certainty. Its significance lies in the way this certainty travels. A local technical guarantee becomes socially consequential when it is recognized, circulated, and used as a credential for a mathematical result. The same process that makes the credential useful also creates the possibility that its authority will exceed the warrant it records. The machine’s reliability supplies the material support for this symbolic authority; the credential gives it a portable form; and, under specific conditions, fetishistic disavowal can preserve its force after the boundary of the check is known.

## 7. Conclusion

How does the epistemic fetishism of formal verification arise? It does not begin with a false belief about an unreliable machine. It begins with a real technical achievement. Lean’s kernel checks proof terms against formal propositions under specified environments, and this genuine reliability gives the credential “Lean-verified” its initial force.

The authority of the credential is assembled through distributed epistemic labour. Mathematical formulation, formal specification, proof construction, library and software maintenance, kernel checking, semantic comparison, expert assessment, and institutional recognition contribute different forms of warrant. Scientific communication condenses this distributed process into a portable sign. As the credential circulates, the relations that gave it meaning can recede while the sign remains. The authority of the network may then appear to reside autonomously in the machine-certified object. This is the fetishistic displacement at the centre of the argument.

Fetishistic disavowal is a further possibility, not an inevitable final step. It explains how symbolic investment can be reproduced when an actor or institution recognizes that the credential is being asked to warrant more than the check establishes, yet continues to mobilize it in that broader role. Knowing the technical limits of Lean and relying on it for the proposition it actually checks is not disavowal. Nor is continued confidence fetishistic when the semantic relation has been separately established through expert scrutiny. The distinction turns on what the credential is made to guarantee after its boundary is known.

The four encounters reveal different configurations. Riemann shows how a strong institutional certification can remain grounded in visible expert review and independent checking. Navier–Stokes exposes the distinction between the theorem established by a formal artifact and the proof route presented in a natural-language account, without showing that the same institution acknowledged this distinction and continued to overstate the credential. AlphaProof Nexus provides the clearest borderline case: the publication acknowledges human validation of formal statements while retaining the language of autonomous mathematical discovery. Liquid Tensor shows how acknowledged semantic risks can be answered through public scrutiny rather than displaced into machine authority.

The article’s central contribution is the concept of the **ideological fetishism of formal verification**: the transformation through which the socially and semantically mediated authority of a machine-checked result appears to reside autonomously in the credential “Lean-verified.” The five-moment account explains its formation and possible reproduction: real reliability, distributed epistemic labour, credential condensation, objectal displacement, and, conditionally, fetishistic disavowal. The machine’s reliability is not what ideology must explain away. It is precisely what ideology must explain: how a real technical guarantee can become the material support for a symbolic authority that exceeds the operation which produced it.

The machine verifies a proposition. The philosophical question is what, beyond that proposition, we ask the credential to guarantee.

## References

Ahlstrom-Vij, Kristoffer. 2021. “Esoteric Reliabilism.” *Episteme* 18 (4): 603–623. https://doi.org/10.1017/epi.2019.39.

Alpöge, Levent. 2026. “The Riemann Hypothesis.” Research note and Lean archive, 20 November. https://alpo.ge/.

Bastounis, Alexander, Fabian Circelli, and Anders C. Hansen. 2026. “Navier–Stokes Lost in Translation: Why Lean Verification of AI Autoformalisation Does Not Guarantee Correct Natural Language Proofs.” arXiv:2610.08144. https://doi.org/10.48550/arXiv.2610.08144.

Black, Jack. 2025. “Examining the Mechanism of Disavowal and Its Two Forms: Cynical Disavowal and Fetishistic Disavowal.” *Theory & Psychology* 35 (1): 117–135. https://doi.org/10.1177/09593543241308199.

De Millo, Richard A., Richard J. Lipton, and Alan J. Perlis. 1979. “Social Processes and Proofs of Theorems and Programs.” *Communications of the ACM* 22 (5): 271–280. https://doi.org/10.1145/359104.359106.

Duede, Eamon, and Kevin Davey. 2025. “A Priori Knowledge in an Era of Computational Opacity: The Role of Artificial Intelligence in Mathematical Discovery.” *Philosophy of Science* 92 (5): 1394–1404. https://doi.org/10.1017/psa.2025.10160.

Emmerson, Parker. 2026. “Alpöge’s Certified Lean Derivation Does Not Prove the Riemann Hypothesis: Granting Every Check, the Hypothesis Follows from a Premise Stronger than Itself.” Preprints.org, posted 24 November 2026. https://doi.org/10.20944/preprints202611.2463.v1. Non-peer-reviewed preprint.

Erdős Problems Research Library. 2026. “Tsoukalas et al., Advancing Mathematics Research with AI-Driven Formal Proof Search: Artifact and Statement Audit.” Updated 13 October. https://erdosproblems.ai/wiki/library/additive_combinatorics/tsoukalas_2026_advancing_mathematics_research_ai_driven_formal_proof_search.

Erfani, Farhang. 2026. “Not ‘Just a Language Model’: AI’s Ideological Functions.” *AI & Society* 41: 869–881. https://doi.org/10.1007/s00146-025-02623-0.

Flisfeder, Matthew. 2023. “There Is No Metalanguage; or, Truth Has the Structure of a Fiction: The Žižekian System, between Post-Ideology and Post-Truth.” *Enrahonar* 70: 171–185. https://doi.org/10.5565/rev/enrahonar.1420.

Hardwig, John. 1985. “Epistemic Dependence.” *The Journal of Philosophy* 82 (7): 335–349. https://doi.org/10.2307/2026523.

Hourigan, Daniel. 2009. *The Phantasmatic Subject of Technology: Slavoj Žižek, Techne, and the Abyss*. PhD thesis, Griffith University. https://doi.org/10.25904/1912/3124.

Kallel, Maher, and Mohamed El Louadi. 2026. “Verification Abundance, Adjudication Scarcity: What Happens to Mathematical Knowledge When Proof Checking Becomes Free.” arXiv:2608.28997. https://doi.org/10.48550/arXiv.2608.28997.

Kuldova, Tereza. 2019. “Fetishism and the Problem of Disavowal.” *Qualitative Market Research: An International Journal* 22 (5): 766–780. https://doi.org/10.1108/QMR-12-2016-0125.

Lacan, Jacques. 2019. *Desire and Its Interpretation: The Seminar of Jacques Lacan, Book VI*. Edited by Jacques-Alain Miller. Translated by Bruce Fink. Cambridge: Polity. Chapter XVI, “There Is No Other of the Other.”

Lean FRO and Mathlib Initiative. 2026. “Lean Verification of the Riemann Hypothesis.” Joint statement, 21 November. https://leanprover-community.github.io/blog/posts/riemann-hypothesis/.

López-Corona, Oliver. 2026. “From Authorial Mathematics to Studio Mathematics: Ecobiontic Forms of Proof after Large Language Models.” arXiv:2608.22194. https://doi.org/10.48550/arXiv.2608.22194.

Mathlib Community. 2022. “Completion of the Liquid Tensor Experiment.” Lean Community Blog, 15 July. https://leanprover-community.github.io/blog/posts/lte-final/.

Mathlib Documentation. 2026. “Mathlib.NumberTheory.LSeries.RiemannZeta.” Definition of RiemannHypothesis. https://leanprover-community.github.io/mathlib4_docs/Mathlib/NumberTheory/LSeries/RiemannZeta.html.

Marx, Karl. 1976 [1867]. *Capital: A Critique of Political Economy*, vol. 1. Translated by Ben Fowkes. London: Penguin. Chapter 1, section 4, “The Fetishism of Commodities and the Secret Thereof.”

Omodeo, Pietro Daniel. 2019. *Political Epistemology: The Problem of Ideology in Science Studies*. Cham: Springer. https://doi.org/10.1007/978-3-030-23120-0.

OpenAI. 2026a. “On the Navier–Stokes Millennium Prize Problem.” 8 September. https://openai.com/index/navier-stokes-solution/.

OpenAI. 2026b. “NavierStokesAndEuler: Lean Certificates Accompanying Navier–Stokes and Euler Results.” GitHub repository. https://github.com/openai/NavierStokesAndEuler.

Cotton, Peter. 2026. “The Formal Statement.” *Navier–Stokes Guide*. Updated 24 September 2026. https://navier.microprediction.org/formal.html.

rh-lean-roadmap. 2026. *The Riemann Hypothesis and GRH for Dirichlet L-Functions: A Readable Account of the Lean Proof in Alpöge’s Archive*. Version 44. Zenodo, 26 November. https://doi.org/10.5281/zenodo.24562451.

Scholze, Peter. 2021. “Half a Year of the Liquid Tensor Experiment: Amazing Developments.” 5 June. https://xenaproject.wordpress.com/2021/06/05/half-a-year-of-the-liquid-tensor-experiment-amazing-developments/.

Sloterdijk, Peter. 1987. *Critique of Cynical Reason*. Translated by Michael Eldred. Minneapolis: University of Minnesota Press.

Sutherland, Andrew. 2026a. “Verification Files for the Lean Proof of the Riemann Hypothesis.” MIT. Last updated 25 November. https://math.mit.edu/~drew/grh/.

Sutherland, Andrew. 2026b. “Shorter Lean Proof of RH and GRH for Dirichlet L-Functions: Verification Files.” MIT. Last updated 26 November. https://math.mit.edu/~drew/shortgrh/.

Topaz, Adam. 2022. “Definitions in the Liquid Tensor Experiment.” Lean Community Blog, 14 October. https://leanprover-community.github.io/blog/posts/lte-examples/.

Tsoukalas, George, Anton Kovsharov, Sergey Shirobokov, Anja Surina, Moritz Firsching, Gergely Bérczi, Francisco J. R. Ruiz, Arun Suggala, Adam Zsolt Wagner, Eric Wieser, Lei Yu, Aja Huang, Miklós Z. Horváth, Andrew Ferraiuolo, Henryk Michalewski, Edward Lockhart, Codrut Grosu, Thomas Hubert, Matej Balog, Pushmeet Kohli, and Swarat Chaudhuri. 2026. “Advancing Mathematics Research with AI-Driven Formal Proof Search.” *Science* 394 (6820). https://doi.org/10.1126/science.aej2213. Preprint: arXiv:2605.22763.

Vallverdú, Jordi. 2026. “Where Does Mathematical Warrant Live? From the Four-Color Theorem to Mass-Released AI ‘Results’.” *Philosophies* 11 (6): 224. https://doi.org/10.3390/philosophies11060224.

Žižek, Slavoj. 1989. *The Sublime Object of Ideology*. London: Verso.

Žižek, Slavoj. 1994. “The Spectre of Ideology.” In *Mapping Ideology*, edited by Slavoj Žižek, 1–33. London: Verso.
