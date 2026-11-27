# In Lean We Trust? The Ideology of Machine-Checked Proofs in Science

**Project:** *In Lean We Trust?*  
**Version:** Essayistic philosophical draft  
**Evidence cut-off:** 27 November 2026  
**Genre:** Philosophical argument with comparative case analysis

## Abstract

What could be ideological about a correct proof? A proof assistant such as Lean provides a genuine and bounded form of mathematical warrant: its kernel checks whether a proof term has the required type for a specified formal proposition under a specified environment. The philosophical question begins when the public credential “Lean-verified” travels beyond that local result and acquires the appearance of a more comprehensive guarantee. Drawing primarily on Slavoj Žižek’s critique of ideology, this article develops the concept of the **ideological fetishism of formal verification**. It argues that ideological fantasy can stage a scene in which a local check appears to close a wider uncertainty, while fetishistic displacement allows authority generated through technical, semantic, and institutional relations to appear as an autonomous property of the verification credential. Disavowal is treated as a secondary possibility, not a necessary feature of the phenomenon. The argument is developed through four encounters with formal verification: the Riemann hypothesis, Navier–Stokes, Erdős problems investigated with AlphaProof Nexus, and the Liquid Tensor Experiment. These cases do not establish that Lean is inherently fetishistic; rather, they expose different configurations of formal warrant, semantic mediation, institutional authorization, and public representation. The article’s contribution is a Žižekian account of how a real but limited technical guarantee may become a symbolic bearer of broader mathematical authority.

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

In “The Spectre of Ideology,” Žižek challenges the assumption that ideology can be identified simply by the falsity of explicit beliefs (Žižek 1994). The ideological function of a proposition cannot be read directly from its truth value. A statement may be factually correct and nevertheless participate in an ideological relation through the position it occupies and the practice it helps sustain. This is not the claim that truth is reducible to power, or that every true statement is ideological. It is the more demanding claim that factual accuracy does not, by itself, settle the question of ideological function.

The distinction matters because the sentence “Lean checked this proof” may be perfectly true. The question is not whether the sentence is false, but what it is made to do. Does it identify a local technical achievement, or does it become a credential through which a much wider mathematical claim is authorized? Does it remain attached to the formal proposition and the conditions under which that proposition was checked, or does it travel as if it carried the authority of the entire mathematical result?

We should resist a familiar shortcut here. A short announcement is not ideological merely because it omits technical detail. An institution does not fetishize a machine simply by recognizing a successful proof check. And a reader is not irrational merely because they rely on an expert's account of a formal result. These may be ordinary and justified practices. The ideological question arises only when the credential is made to perform a function that cannot be explained by its explicit technical content alone.

This is why ideology critique must distinguish truth, compression, legitimation, and ideological operation. A true statement can be compressed without becoming misleading. A result can be institutionally recognized for good reasons. But a credential may also become the point through which the authority of a whole network is condensed and presented as if it belonged to one object. The last possibility is what requires explanation.

Žižek's account also prevents us from treating ideology as a matter of discourse alone. In “The Spectre of Ideology,” he distinguishes explicit doctrine, the materiality of ideological apparatuses, and the more elusive spontaneous operation of ideology within social reality (Žižek 1994, 9–10). Applied to formal verification, the analysis cannot stop at what a press release says. It must also ask how the credential is embedded in repositories, checking procedures, institutional endorsements, publication practices, and the routine allocation of mathematical credibility. If ideology is at work, it is not simply a mistaken sentence about a machine. It is a relation between what is said, what is materially done, and what becomes practically authoritative.

### 3.2 Ideological fantasy: the scene in which uncertainty appears to end

In *The Sublime Object of Ideology*, fantasy is not merely a false image that conceals an otherwise complete reality. It supplies the coordinates through which reality is experienced and helps sustain the appearance of coherence where a constitutive gap remains (Žižek 1989, 28–31). Fantasy does not simply tell a subject what to believe. It organizes the scene in which a practice becomes intelligible and in which an incomplete social relation can appear whole.

What is the relevant gap in formal verification? It is not a defect in Lean's kernel, nor a mysterious distance between mathematics and reality. It is the non-identity between the formal object that is checked and the intended mathematical claim to which it is connected. Let \(P\) be the intended claim and \(P^*\) the formal proposition. The kernel may establish, with extraordinary precision, that a proof term \(t\) inhabits \(P^*\) under a specified environment \(\Gamma\). The relation between \(P\) and \(P^*\), however, is a distinct specification relation. It can be scrutinized, formalized in part, checked by experts, and made highly reliable. What it cannot be is silently identified with the kernel's acceptance of \(t : P^*\).

This is a point about non-totalizability, not about an unbridgeable gulf. The specification relation may be well established. Its assumptions may be explicit. Its formalization may itself be checked. None of this implies that the original kernel check has somehow absorbed every other epistemic task into itself. The different components of warrant can be connected, and the connections can be rigorous, without becoming one and the same operation.

The fantasy of formal verification becomes possible when the kernel's local verdict is staged as the point at which this wider chain of questions appears to have been closed. The certificate seems to settle not only whether \(t\) proves \(P^*\), but also whether \(P^*\) is the intended theorem, whether the assumptions are appropriate, whether the result has the significance attributed to it, and whether the mathematical dispute is over. The fantasy does not have to appear as the explicit proposition “Lean can prove everything.” Its operation is subtler: the scene of verification gives the appearance that the work connecting the formal object to the wider claim has already been completed.

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

Why, then, is the scene of closure attractive? Because formal verification makes one part of mathematical warrant unusually visible. A proof may depend on an extensive library, a complex formalization, and years of technical work. The final checking result, by contrast, can be communicated in a compact and reproducible form. The word “verified” gives a heterogeneous process a single point of presentation. The fantasy is not that the proof term is unreal. It is that the local completion of one task can stand in for the completion of the whole.

This is also why fantasy cannot be reduced to rhetorical exaggeration. A headline that says “Lean proves the theorem” may be harmless shorthand when its context identifies the exact formal target and the relevant qualifications. Conversely, a technically accurate statement may still participate in a scene of closure if it is used to make the broader question appear settled. The analysis must therefore ask not only what a sentence says, but what kind of completion it stages.

### 3.3 Fetishism: when the relation appears as a property of the object

The more decisive theoretical move comes from Marx's account of commodity fetishism. In *Capital*, Volume I, Chapter 1, Section 4, Marx analyzes how relations among producers assume the appearance of relations among things. Žižek's discussion emphasizes the form through which an effect generated by a network of relations appears as an immediate property of an object (Žižek 1989, 19–20).

The analogy with formal verification must be drawn carefully. Mathematical truth is not produced by collective labour in the same way that commodities are produced. Nor is Lean a commodity in Marx's technical economic sense. The relevant structure is the appearance of a relation-dependent authority as an intrinsic property of an object.

The authority of a Lean-verified result depends on a network: the problem is selected and formulated; definitions and assumptions are chosen; the intended theorem is represented formally; a proof object is constructed; libraries and software infrastructure are maintained; the kernel checks the proof term; experts examine the specification relation; institutions and mathematical communities assess the result's status. These activities do not perform one undifferentiated act. They contribute different forms of warrant.

The fetishistic possibility appears when the authority generated through this network seems to reside autonomously in the verification credential itself. The credential then appears not merely to report that one component of the proof process has succeeded, but to contain the authority of the whole. The relation is inverted: the network makes the credential meaningful, yet the credential appears as the source that certifies the network.

This is more than the disappearance of human contributors from a press release. Their names may be listed and the process may still be organized around a credential that functions as a self-sufficient guarantee. Conversely, contributors may be omitted from a short announcement without any fetishistic effect, if the context makes the scope of the check clear. The relevant issue is not visibility alone. It is the attribution of authority: does the authority appear to arise from the relations that connect the formal artifact to the mathematical claim, or does it appear to be an autonomous property of the machine-certified object?

The credential “Lean-verified” is especially suited to this role because it is portable. It can move from a repository to an abstract, from an abstract to an institutional announcement, and from an announcement to a public account. In each movement, the original formal proposition may become less visible while the credential remains. What travels is no longer merely the information that a particular proof term inhabits a particular formal type. What travels may be a condensed sign of mathematical authority.

Fetishism, in this sense, does not mean that people mistakenly believe the machine has performed no human work. It means that the authority produced through a network of relations appears to belong to the object as such. The machine is not simply credited with labour it did not perform: it really did check the proof term. The displacement concerns the surplus of authority that can attach to this genuine achievement.

### 3.4 Disavowal and the persistence of symbolic investment

Žižek's discussion of cynical ideology draws on Peter Sloterdijk's critique of cynical reason (Sloterdijk 1987; Žižek 1989, ch. 1). The familiar formula that subjects know what they are doing and nevertheless continue to do it should not be presented as Žižek's original coinage. Later scholarship distinguishes cynical disavowal from fetishistic disavowal (Kuldova 2019; Black 2025).

For this article, disavowal is a secondary and conditional mechanism. A credential may acquire a fetishistic function without the available evidence showing that a particular actor explicitly acknowledged its limitations. Disavowal is a stronger claim: it concerns the persistence of a broader symbolic investment after the relevant limitation has been recognized.

The distinction matters because rational reliance is not disavowal. A mathematician may know perfectly well that Lean checks a formal proposition rather than the entire history of its formulation, and still rely on Lean for exactly that task. There is no contradiction here. A disavowal hypothesis becomes plausible only when the same actor or institutional communication chain acknowledges a precise limitation and nevertheless continues to use the credential as a broader guarantee, with no contextual qualification or correction that resolves the apparent discrepancy. Cynical disavowal requires stronger evidence of a strategic or manipulative relation between acknowledged knowledge and practice. Public wording alone cannot establish unconscious motives.

The Lacanian idea that there is no complete Big Other and no “Other of the Other” provides a background to this argument (Lacan 2019, ch. XVI; Žižek 1989, Part II). No final symbolic authority can guarantee the consistency of the entire order from outside it. This does not imply that mathematical proof is impossible or that standards are arbitrary. Lean is not the Big Other. The point is that the credential may be invested with the function of a final guarantee even though its actual warrant remains local and conditional.

## 4. The Machine as a Fetish Object

The machine does not become a fetish because it is powerful, reliable, or admired. Nor does it become a fetish simply because its operation is too complex for most users to inspect. The decisive question is different: how does an authority produced through a network of relations come to appear as if it were located in the object itself?

The credential “Lean-verified” is not an empty sign. It refers to a real event: a proof term has been checked against a formal proposition under a specified environment. This is precisely why the credential can carry authority. If the check were meaningless, it could not serve as a convincing guarantee. The fetishistic structure does not arise in spite of the machine's technical success; it may arise through the social use of that success.

The process involves a peculiar inversion. A formal verification credential is meaningful only because a network of practices has made it meaningful: mathematicians formulate the claim, formalizers specify it, libraries and tools support the proof, the kernel checks the term, experts assess the relation between the formal statement and the intended theorem, and institutions decide how the result should count. Yet once the credential circulates, it can appear as if the authority of this entire network originates in the machine. The network confers authority on the credential; the credential then appears to confer authority on the network.

This is the central paradox of the fetish object. It is at once the product of a relation and the apparent source of that relation's authority. The machine-certified object seems to stand outside the process that produced it, as if it could guarantee the process from a position of independence. The social relation does not vanish. It returns in an objectified form.

Three movements help clarify this transformation.

First, there is **condensation**. A heterogeneous set of epistemic activities is compressed into a portable credential. The distinction between theorem formulation, formal specification, kernel checking, semantic comparison, and institutional assessment may remain present in the actual research process, but the phrase “Lean-verified” makes the result communicable as a single status.

Second, there is **displacement**. The authority that depends on these relations appears to reside in the machine or its certificate. The object is no longer merely one component within a warrant architecture. It becomes the apparent bearer of the authority of the whole. This is the specifically fetishistic moment; omission of contributors or technical detail is not enough unless it contributes to this displacement.

Third, there is **circulation**. The credential can move across contexts while becoming detached from the exact proposition and environment to which it originally referred. In a repository, “verified” may refer to a named theorem and a reproducible proof artifact. In an institutional announcement, it may become a sign of certification. In public communication, it may be taken as a sign that a mathematical problem has been solved. The same word travels, but the scope of the claim can change.

These movements are not a mechanical sequence, and none is inevitable. Condensation is necessary for communication; displacement is not. A credential can circulate while retaining a precise reference to the formal proposition. An institution can celebrate a proof while explaining what the checker did and did not establish. The fetishistic effect appears only when the credential's portability allows its local warrant to be treated as a self-sufficient source of wider authority.

This also clarifies the difference between fetishism and ordinary technological opacity. A user need not understand the internal implementation of Lean to rely rationally on its kernel. The problem is not simply that the system is a black box to a particular reader. The problem is that the relations which make the credential epistemically meaningful are displaced, while the credential itself appears to possess the authority they collectively sustain. Opacity may facilitate this appearance, but it is not identical to it.

Nor is the fetishistic object simply “the machine.” Lean's kernel remains a real technical component with a defined function. The fetishized object is the credential through which the machine's local achievement is made to carry a broader social meaning. This is why the expression **the ideological fetishism of formal verification** is more precise than “machine worship.” We are not diagnosing an emotional attachment to technology. We are analyzing a form of authority in which a relation-dependent warrant appears as an autonomous property of an object.

The concept also adds something to a purely normative account of epistemic dependence. Hardwig helps explain why it can be rational to rely on experts whose evidence one cannot personally reproduce (Hardwig 1985). The present question is not whether such reliance is justified. It is how a specific credential can become the object through which a distributed community recognizes and communicates its own authority. The same credential can therefore be epistemically legitimate at one level and ideologically overburdened at another. Its local warrant remains real; its symbolic surplus is what requires analysis.

This distinction must govern the case studies. We should not call a result fetishistic merely because Lean is mentioned prominently, because an announcement is concise, or because a reader trusts a formal checker. We need to identify what the credential is made to warrant, whether its authority appears to reside autonomously in the object, and whether that representation has a recognizable role in legitimating the result. A mismatch between a paper and a formal declaration may reveal a specification problem; it does not, by itself, establish fetishism. The concept becomes meaningful only when it explains the conversion of a real technical achievement into a wider bearer of authority.

## 5. Four Encounters with Formal Verification

The following cases are not a representative survey of Lean use, nor are they matched controls. They were selected because they expose different relations between a formal artifact and the mathematical claim associated with it. Each encounter is read alongside its primary statements, technical records, and relevant independent scrutiny. The purpose is not to adjudicate the underlying mathematics of every result. It is to ask what the Lean credential is made to warrant, what relations remain visible, and what the available evidence permits us to conclude.

### 5.1 The Riemann Hypothesis: certification and the limits of institutional closure

On 20 November 2026, Levent Alpöge released a note and a large Lean development concerning the Riemann hypothesis (Alpöge 2026). The Lean FRO and Mathlib Initiative issued a joint statement on 21 November expressing “full confidence” in the proof and stating that the community certified both the statement and the proof (Lean FRO and Mathlib Initiative 2026).

The formal statement itself matters. Mathlib’s definition of the Riemann hypothesis asserts that every zero of the formalized zeta function, excluding the trivial negative even zeros and the point \(s=1\), has real part \(1/2\) (Mathlib Documentation 2026). The exclusion of \(s=1\) is part of the formal definition because the classical zeta function has a pole there, while the formalized function assigns a value at that point. The formal object is therefore not simply a phrase copied from a textbook. It is a specific mathematical statement within a formal library.

The joint statement describes several forms of scrutiny: expert vetting of the Mathlib statement, successful compilation of the archive, comparison of the proved theorem with the Mathlib statement by two independent tools, and acceptance of the exported proof by Lean’s kernel and independent checkers. Andrew Sutherland’s verification report records 175,187 compiling modules in the original archive, kernel replay, independent checker runs, and statement comparisons (Sutherland 2026a). A shorter rewrite appeared on 25 November and has a separate verification record; it is a distinct artifact and should not be conflated with the original archive (Sutherland 2026b).

A substantial exposition also appeared on 26 November. The rh-lean-roadmap project provides a 497-page main text, 963 pages of longer proofs, a 122-page index, and a short roadmap. Its documentation states that several AI models generated the exposition from the Lean source and cross-checked it (rh-lean-roadmap 2026). This is a readable, AI-mediated mathematical account. It is not a conventional independently authored paper, nor does its existence prove that every mathematician has independently read and accepted every argument.

The case became more complicated when Parker Emmerson posted a non-peer-reviewed preprint on 24 November arguing that the certified derivation does not prove the Riemann hypothesis in several senses (Emmerson 2026). The preprint grants the existence of the Lean derivation and the reported checks, but challenges what follows from them. In particular, it treats the consistency of the formal rules as a further premise or “sponsor” and argues that this is stronger than the hypothesis. The official Lean FRO/Mathlib statement, for its part, says that the independent checkers have formal soundness proofs relative to set theory. The disagreement therefore concerns not whether the kernel accepted the proof term, but how the foundational conditions and formal statement should be interpreted.

This article does not adjudicate Emmerson’s mathematical or logical argument. Its status as a non-peer-reviewed preprint must remain explicit. It is evidence of a public foundational challenge, not proof that the Lean kernel failed or that the Riemann hypothesis is false. Conversely, the institutional statement is evidence of a substantial certification process, not a demonstration that every foundational and interpretive question has been settled.

What does the case show? It shows that several forms of authority coexist: kernel checking, independent checking, expert assessment of the formal statement, institutional certification, AI-mediated exposition, and foundational criticism. The official statement makes much of the human and institutional mediation visible. The public challenge, meanwhile, demonstrates that certification does not terminate every dispute about what has been proved.

The Riemann case is therefore not strong evidence of fetishistic displacement. The credential has considerable institutional force, but the process behind it is unusually visible. It is more useful as a case of layered and contested authorization: the machine check is real, the institutional certification is real, and the meaning of that certification remains open to philosophical and mathematical interpretation.

### 5.2 Navier–Stokes: a formal proof and the proof it is said to represent

On 8 September 2026, OpenAI announced a result concerning the Navier–Stokes existence and smoothness problem, presenting an analytical proof together with a Lean formalization (OpenAI 2026). The announcement concerns finite-time singularity formation for a three-dimensional incompressible fluid with smooth external forcing and finite energy, and claims to establish statements C and D of the official Millennium Prize formulation.

An independent analysis by Bastounis, Circelli, and Hansen (2026) examines the relation between the natural-language paper and the Lean formalization. Their central distinction is important: compiling a Lean proof of a formal statement is not the same as establishing that the formalization is a semantically faithful translation of the original mathematical text. Their audit identifies, among other things, a discrepancy in Lemma 8.6. The natural-language proof uses \(m+4\) input derivatives in an inverse estimate, whereas the corresponding Lean declaration requires \(m+5\). They also identify a difference in the pressure-flux estimate and proof route.

These discrepancies concern the relation between the written proof and the formal artifact. They do not establish a failure of Lean’s kernel. Nor do they prove that the underlying Navier–Stokes theorem is false. The kernel may correctly check a proof term for the formal proposition encoded in the repository while the correspondence between that proposition and the separate natural-language argument remains disputed.

This case makes the distinction between derivational validity and specification fidelity unusually concrete. The issue is not whether Lean has checked something. It is whether the thing checked is precisely the mathematical claim that the public account associates with it.

It is tempting to treat this as a clear example of ideological fetishism: a formal certificate appears beside a claim to have solved a Millennium Prize problem, while the relation between the formal declarations and the written proof is contested. But the evidence requires a more careful judgement. OpenAI’s announcement presents both a write-up and a formalization; it does not explicitly state that Lean alone verifies every step of the natural-language paper. The discrepancy is a serious reason to inspect the specification relation, but it is not by itself proof that the institution or its audience treated the credential as an autonomous guarantee.

Navier–Stokes is therefore the strongest candidate for scope extension among the four cases, but the full diagnosis remains unestablished. The case reveals the exact place where a machine-checked formal object and a broader mathematical claim can come apart. Whether the credential then functions as an autonomous bearer of authority requires additional evidence about its representation and legitimating effect.

### 5.3 Erdős problems and AlphaProof Nexus: the return of human validation

Tsoukalas and colleagues report that AlphaProof Nexus resolved nine of 353 open Erdős problems represented in the Formal Conjectures repository and produced 44 proofs among 492 OEIS conjectures attempted (Tsoukalas et al. 2026). These denominators describe the formalized benchmark and the attempted OEIS statements, not all open Erdős problems. The system combines language-model proof search with Lean checking. The *Science* paper also reports human validation of the correspondence between the nine solved Lean statements and the original conjectures.

This workflow is important because it makes the division of epistemic labour relatively explicit. The AI system searches for proof strategies; Lean checks formal proof terms; human experts assess whether the formal statements capture the intended conjectures. The machine is not simply presented as an autonomous mathematician whose output is self-authenticating.

A source-level audit nevertheless identifies several provenance and statement-link issues (Erdős Problems Research Library 2026). For problem #26, the top-level linked Lean target differs from the upper-density theorem described in the prose, although an auxiliary pointwise lemma in the same file is strong enough to establish the prose result. For #741(i), the linked file proves an exact-density counterexample, while the upper-density theorem exists separately in the Formal Conjectures repository. For #741(ii), the cited link points to a file for another problem. These findings concern the identity and provenance of particular artifacts. They do not show that Lean accepted an invalid proof, that all nine results are invalid, or that the relevant formal proofs do not exist elsewhere.

The case therefore reveals a distinction between a paper’s report of human statement validation and the traceability of each published artifact. The existence of human validation does not make every repository link self-authenticating. Conversely, a wrong or variant link does not refute the theorem. The precise question is whether the artifact cited as the formal proof is the artifact that establishes the claim described in the paper.

AlphaProof Nexus is not a clean counter-case, but neither is it a demonstrated instance of fetishism. It shows how a public credential can depend on the continuing work of statement comparison, version control, and provenance. It also shows why “Lean-verified” cannot be treated as a substitute for identifying which theorem, in which file, at which commit, was actually checked.

### 5.4 The Liquid Tensor Experiment: a counter-example to autonomous machine authority

The Liquid Tensor Experiment provides a different configuration. Completed in July 2022, the project formalized a major theorem concerning the vanishing of higher Ext groups for specified condensed real vector spaces (Mathlib Community 2022). Its public record identifies mathematical, formalization, technical, library, and institutional contributors. The formal result is presented as a collective undertaking, not as an autonomous achievement of the proof assistant.

More importantly, Adam Topaz’s subsequent discussion explicitly raises the semantic problem: how can mathematicians be confident that the definitions introduced in Lean are correct? A formal definition could be pathological—for example, it could make Ext identically zero. The project responded by creating an examples folder containing sanity checks designed to be readable by mathematicians with limited Lean experience, allowing them to inspect the definitions and gain reasonable confidence that the formal statement captured the intended mathematics (Topaz 2022). Peter Scholze’s account also emphasizes mathematical interaction and scrutiny (Scholze 2021).

This is not merely a project that happens to acknowledge human contributors. It makes the semantic validity of its definitions an explicit object of public scrutiny. The formal certificate remains embedded in a visible network of mathematical interpretation and technical work.

Liquid Tensor is therefore a genuine counter-case to any claim that formal verification is inherently fetishistic. It does not prove that every participant understood every definition, nor does it establish a controlled causal relation between transparency and trust. It does show that the authority of a proof assistant can be presented as one component of a broader, inspectable epistemic practice. The machine check does not need to appear as an autonomous guarantee.

## 6. The Ideological Function of Mathematical Certainty

The four encounters do not show that formal verification is inherently ideological. They show something more difficult to state and more important to preserve: the same technical achievement can occupy different positions within the social life of mathematical knowledge. A kernel check can remain a carefully bounded component of a wider warrant. It can also become a portable credential through which a wider claim is authorized. The difference is not located in the machine alone. It lies in the relation between the machine's actual function and the authority that is made to circulate in its name.

Modern mathematics depends on forms of knowledge that no single participant can survey in their entirety. Proofs may rely on extensive libraries, complex software, specialized formalization, and distributed expert judgement. This division of epistemic labour is not a crisis to be overcome. It is one of the conditions of contemporary mathematical practice. The difficulty is that the more distributed the production of knowledge becomes, the more important it is to have ways of making its results portable. A credential such as “Lean-verified” performs precisely this function. It allows a result to travel beyond the immediate group that constructed and checked it.

Here lies the ambivalence. The credential is useful because it compresses a complex achievement into a form that others can recognize. It is potentially ideological for the same reason. Its portability can detach it from the precise proposition, environment, and specification relation that gave it its original warrant. The credential can then be asked to perform two tasks at once: to report that a formal proof has been checked, and to certify that the wider mathematical claim is settled. The first task belongs to the kernel. The second requires a broader network of mathematical interpretation and institutional judgement.

The ideological function of mathematical certainty is therefore not simply that people believe in a false guarantee. It is that a real local guarantee can become the bearer of a wider promise. The machine's technical success supplies the material support for this promise; the symbolic credential allows it to circulate. The result is not a choice between genuine reliability and ideological illusion. The two can coexist at different levels of the same practice.

The four cases clarify the conditions under which this conversion may or may not occur.

The Riemann hypothesis case shows how formal checking, independent verification, expert assessment of the formal statement, institutional certification, and AI-mediated exposition can converge in a highly visible event. The Lean FRO/Mathlib statement expresses full confidence in the proof, while the subsequent Emmerson preprint challenges the foundational interpretation of what the certification establishes. The case is not a straightforward instance of fetishistic displacement: the official account makes several forms of mediation explicit, and the later challenge demonstrates that institutional certification does not eliminate interpretive dispute. What it reveals is that the authority of a formal certificate is itself an object of public negotiation.

Navier–Stokes brings the problem into sharper focus. The discrepancy between the natural-language proof and the Lean declarations raises a precise question about specification fidelity. A proof term may be correctly checked for the formal statement while the relation between that statement and the written argument remains disputed. This makes the case the strongest candidate for scope extension. Yet the discrepancy alone does not prove that the Lean credential was treated as an autonomous guarantee. The announcement presents both a write-up and a formalization; further evidence is needed before we can claim that the certificate itself performed an independent legitimating function. The case therefore exposes the site at which fetishistic displacement could occur without allowing us to declare that it has already been established.

The Erdős / AlphaProof Nexus case reveals a different configuration. The published account reports human validation of the correspondence between formal statements and original conjectures. At the same time, source-level provenance issues show why the identity of a cited formal artifact cannot be taken for granted. This is not evidence that the machine's proof search is invalid, nor that all reported results are wrong. It demonstrates that the public credential depends on a chain of statement selection, formalization, validation, and artifact traceability. The case complicates any narrative in which the machine appears as a self-sufficient source of mathematical discovery.

Liquid Tensor provides the counter-case. Here, the project made collective mathematical labour and the correctness of formal definitions explicit objects of scrutiny. Topaz's sanity checks were designed to make the definitions inspectable by mathematicians who were not necessarily experienced Lean users. The result is not a world without reliance on the machine; it is a practice in which reliance is accompanied by visible semantic work. The credential remains embedded in a wider process rather than appearing as the autonomous source of its authority.

The comparison yields an important negative result: none of the four cases, on the evidence presently available, establishes the full conjunction of scope extension, objectal displacement, and social efficacy. This does not make the cases philosophically irrelevant. It means that they do not license a universal diagnosis. Riemann shows layered authorization; Navier–Stokes reveals a concrete specification problem; Erdős highlights validation and provenance; Liquid Tensor demonstrates a counter-practice of semantic transparency. Together they clarify what would have to be shown before the concept of ideological fetishism could be applied without overstatement.

The theoretical contribution lies in the distinction between the **warrant of a check** and the **authority of a credential**. The first concerns what the formal system establishes. The second concerns how that result is recognized, circulated, and made to count. The credential can be epistemically legitimate because it reports a real check, while becoming ideologically overburdened when it is treated as if the local warrant were sufficient for the wider claim. This is not a contradiction. It is the very structure that the concept is designed to explain.

This argument also clarifies the relation to recent work. Vallverdú's Locus Thesis provides a detailed component-based account of mathematical warrant (Vallverdú 2026). Kallel and El Louadi (2026) distinguish derivational validity, representational fidelity, and epistemic significance, and explain why abundant checking does not remove the need for human adjudication. López-Corona's account of “studio mathematics” examines the human-machine assemblages, provenance, agency, and responsibility involved in AI-assisted proof production (López-Corona 2026). These works establish important parts of the epistemic and institutional landscape. The present article does not claim to have discovered the distributed character of mathematical labour or the need to distinguish different warrant components. It asks how the authority generated through those components may become condensed in a portable technical credential.

Erfani (2026) directly examines ideological functions of AI systems, while Hourigan (2009) applies Žižek to technological fetishization and knowledge production. Omodeo (2019) develops a broader political epistemology of ideology in science studies. The contribution here is narrower than these general projects: it identifies the Lean-verification credential as a specific object through which the symbolic authority of mathematical proof may be condensed, displaced, and circulated. The phrase “epistemic fetishism” has also been used in a different analytic-epistemological sense by Ahlstrom-Vij (2021); the present article therefore uses the full expression “the ideological fetishism of formal verification” and does not claim to have coined the bare term.

What, then, does the machine guarantee? It guarantees something important: under a specified formal environment, a proof term has been accepted for a formal proposition. What it cannot guarantee by that operation alone is that every relation through which this proposition becomes a mathematical claim has been settled. Those further relations may be examined, and they may be established with great rigour. But their warrant is not magically contained in the kernel's verdict.

The ideological question begins when the credential is made to conceal this distinction—not necessarily by stating something false, but by allowing a real local certainty to stand in for a final one. The fetish is not that the machine is unreliable. It is that the machine's reliability can be made to carry the authority of a whole that no single technical operation can certify by itself.

## 7. Conclusion

What is ideological about a correct proof? Nothing follows from its correctness alone. Lean’s kernel provides a genuine and valuable form of formal assurance. The ideological question begins when the credential associated with that assurance is made to stand for a wider mathematical authority that the checking operation does not, by itself, establish.

Drawing on Žižek’s critique of ideology, this article has proposed the concept of the ideological fetishism of formal verification. Ideological fantasy explains how a local check may stage the appearance that a wider uncertainty has been closed. Fetishism explains how authority generated through a network of technical, semantic, and institutional relations may appear to reside autonomously in the credential “Lean-verified.” Disavowal remains a secondary possibility where acknowledged limitations coexist with continued investment in a broader guarantee.

The four encounters do not establish that Lean is inherently fetishistic. They show instead why the question must be asked carefully. Riemann reveals layered institutional certification and foundational contestation. Navier–Stokes exposes the difference between a checked formal declaration and its correspondence to a natural-language proof. Erdős demonstrates the importance of human validation and artifact provenance. Liquid Tensor shows how semantic scrutiny can remain visible within a formalization project.

The article’s claim is therefore conditional. Formal verification is not an ideological error, and rational reliance on Lean is not a form of false consciousness. The issue is whether the credential remains a properly scoped component of a wider warrant architecture or becomes an apparently self-sufficient bearer of authority. The task of ideology critique is not to expose the machine as false. It is to explain how a real technical guarantee can be made to stand for more than it warrants.

The machine verifies. The question is what, beyond the proof term, we ask it to guarantee.

---

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

OpenAI. 2026. “On the Navier–Stokes Millennium Prize Problem.” 8 September. https://openai.com/index/navier-stokes-solution/.

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
