# The Ideological Fetishism of Formal Verification: A Žižekian Critique of the Lean-Verification Credential in Mathematical Knowledge Production

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

In “The Spectre of Ideology,” Žižek challenges the assumption that ideology can be identified simply by the falsity of explicit beliefs (Žižek 1994). The ideological function of a proposition depends not only on what it says but also on the position from which it is articulated and the social relation in which it operates. A true statement can participate in an ideological practice. This does not mean that every true statement is ideological, still less that truth is reducible to power. It means that factual accuracy alone does not settle the question of ideological function.

The distinction is essential here. “Lean checked this proof” may be entirely accurate. The ideological question is what this statement is made to authorize. Does it refer to the exact formal proposition, under a specified environment, with the relevant assumptions and semantic relation clearly identified? Or does the credential come to stand for the correctness, significance, or final acceptance of a wider mathematical result without those further relations being established?

A short statement is not automatically ideological. It may be a reasonable compression of technical detail. An institutional endorsement is not automatically fetishistic. It may accurately report what was checked and what experts reviewed. The distinction between a true statement, a compressed statement, an institutional act of legitimation, and an ideological function must be preserved. The last requires an additional argument: the credential must be shown to organize a wider relation of authority, not merely to omit detail.

Žižek’s account also directs attention beyond explicit discourse. In “The Spectre of Ideology,” he distinguishes ideology as doctrine, ideology in its material externality and apparatuses, and the more elusive spontaneous operation of ideology within social reality (Žižek 1994, 9–10). For the present inquiry, this means that we cannot limit ourselves to headlines or press releases. We must also consider the repositories, checking procedures, institutional announcements, and repeated practices through which the credential “Lean-verified” acquires meaning. Ideology, if it is present, is not only something said about the machine. It may also be something done with the credential.

### 3.2 Ideological fantasy: the scene of closure

In *The Sublime Object of Ideology*, fantasy is not simply a false picture that conceals an otherwise complete reality. It provides coordinates through which reality is experienced and helps sustain the appearance of coherence where a constitutive gap remains (Žižek 1989, 28–31). Fantasy does not merely tell the subject what to believe. It helps organize the scene in which a social practice appears intelligible and complete.

What is the relevant gap in formal verification? It is not a defect in Lean’s kernel. It is the non-identity between the formal object that is checked and the intended mathematical claim to which it is connected. This relation can be audited and, in many cases, established with considerable rigour. But it is not established by the same operation that checks the proof term. The wider warrant also depends on the adequacy of definitions and assumptions, the provenance of the formal artifact, mathematical interpretation, and the institutional assessment of the result.

The fantasy of verification becomes possible when the kernel’s local verdict is staged as the point at which this wider chain of uncertainty appears to have been closed. The formal certificate seems to settle not only whether \(t\) proves \(P^*\), but also whether \(P^*\) is the intended theorem, whether the theorem has the significance attributed to it, and whether the mathematical question is now beyond dispute.

The difference can be written schematically:

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

The fantasy is not necessarily an explicit belief that Lean can prove empirical reality or settle every question of mathematical interpretation. It is a possible symbolic organization of the verification event. The local check becomes the visible scene in which the broader demand for certainty appears to have been satisfied. The work of connecting \(P^*\) to \(P\) has not necessarily disappeared; it may simply appear already completed.

This is why fantasy cannot be reduced to rhetorical exaggeration. A headline that says “Lean proves the theorem” may be ordinary shorthand if the surrounding context makes the precise formal target clear. A technical report that identifies the formal proposition, the trusted base, the statement comparison, and the status of expert review may actively resist the fantasy of closure. The concept becomes useful only when it explains how a representation organizes the meaning of a practice, not when it merely labels a sentence as too confident.

### 3.3 Fetishism: the social relation in the machine-object

The more decisive theoretical move comes from Marx’s account of commodity fetishism. In *Capital*, Volume I, Chapter 1, Section 4, Marx analyzes how relations among producers assume the appearance of relations among things. Žižek’s discussion of commodity fetishism emphasizes the form through which an effect generated by a network of relations appears as an immediate property of an object (Žižek 1989, 19–20).

The present article proposes a structural extension of this insight to the **Lean-verification credential**. The object of analysis is not Lean software as such. It is the credential “Lean-verified” as it circulates through mathematical research, institutional statements, repositories, and public accounts.

The credential depends on a network of relations. Someone selects the problem and formulates the intended theorem. Mathematicians choose definitions and assumptions. Formalizers encode the proposition and construct or guide the proof. Libraries and software infrastructure make the formalization possible. Kernel developers and maintainers sustain the trusted implementation. Experts compare the formal statement with the intended mathematics. Institutions and journals evaluate the result and communicate its status. These activities do not all perform the same epistemic function. Nor does collective labour create mathematical truth in the same way that labour produces commodities. It produces, maintains, checks, interprets, and authorizes the artifacts and relations through which a formal result is connected to an intended mathematical claim.

The fetishistic possibility appears when the authority generated through this network seems to reside autonomously in the credential itself. The credential then appears to contain its own guarantee. What is in fact a relation among a formal proposition, a proof object, a checking procedure, a trusted base, mathematical interpretation, and institutional recognition appears as a property of the machine: Lean has verified it.

This is more specific than saying that a press release has omitted the names of contributors. Omission alone does not establish fetishism. A short announcement may reasonably foreground the checker while the surrounding technical record makes the rest of the warrant architecture explicit. The relevant question is whether the credential is represented or practically treated as self-sufficient, and whether the relations necessary to interpret its scope are displaced in that process.

The proposed concept can now be stated:

> **The ideological fetishism of formal verification is the objectal displacement through which the socially and semantically mediated authority of a machine-checked result appears to reside autonomously in the credential “Lean-verified,” allowing the warrant of a bounded formal check to stand for a wider mathematical claim.**

This is a proposed Žižekian extension, not a term coined by Žižek. The analogy with commodity fetishism is structural rather than identical. Lean is not being described as a commodity in Marx’s technical economic sense, and mathematical validity is not being reduced to the social production of a formal artifact. The point is the form of appearance: an authority generated through relations comes to look like an intrinsic property of the object.

### 3.4 Disavowal and the persistence of the guarantee

Žižek’s discussion of cynical ideology draws on Peter Sloterdijk’s critique of cynical reason (Sloterdijk 1987; Žižek 1989, ch. 1). The familiar formula that subjects know what they are doing and nevertheless continue to do it should not be presented as Žižek’s original coinage. Later scholarship distinguishes cynical disavowal from fetishistic disavowal (Kuldova 2019; Black 2025).

For this article, disavowal is a secondary and conditional mechanism. A credential may perform an objectal and legitimating function without the available evidence showing that a particular actor explicitly acknowledged its limitations. Disavowal is a stronger claim. It requires an explicit acknowledgement of the precise limitation, continued use of the same credential as a broader guarantee, a traceable connection within the same actor or institutional communication chain, and evidence that context, ordinary shorthand, or correction does not resolve the discrepancy.

Cynical disavowal requires still stronger evidence of a strategic or manipulative distance between acknowledged knowledge and practice. Public wording alone cannot establish unconscious motives. It is therefore important not to turn every mismatch between a caveat and a public claim into a diagnosis of cynicism. The four cases considered below do not establish cynical disavowal.

The Lacanian idea that there is no complete Big Other and no “Other of the Other” provides a background to this argument (Lacan 2019, ch. XVI; Žižek 1989, Part II). No final symbolic authority can guarantee the consistency of the entire order from outside it. This does not imply that mathematical proof is impossible or that standards are arbitrary. Lean is not the Big Other. The point is that a local technical credential may be made to function as if it supplied a final guarantee of every level of mathematical knowledge.

## 4. The Machine as a Fetish Object

We can now state more precisely what is at stake in the expression “the ideological fetishism of formal verification.” The fetishized object is not simply a machine that people admire. It is the credential “Lean-verified,” understood as a portable bearer of mathematical authority.

Why does this credential have such power? Because it condenses several distinct relations into one visible result. The proof may be too long for most readers to inspect. The formalization may depend on extensive libraries. The semantic relation between the formal statement and the intended theorem may require expert judgement. The institutional significance of the result may remain unsettled. Yet the credential can be stated in a single phrase. It makes a complex process communicable.

This condensation is not inherently deceptive. Every public account of scientific knowledge must select and compress information. Nor is the credential empty. It refers to a real checking event. The fetishistic operation begins when this real and limited function is made to appear as the source of a wider authority in its own right.

The distinction can be put this way. The machine’s kernel establishes that a proof term has the required type for a formal proposition under a specified environment. The credential may then circulate as if it guaranteed that the proposition faithfully expresses the intended theorem, that the result has the significance claimed for it, and that the relevant mathematical dispute has been settled. The problem is not that these further claims are necessarily false. They may be true. The problem is that their warrant is not contained in the kernel check alone.

The credential thus becomes an object in which a distributed epistemic relation is condensed. Its apparent autonomy is precisely what requires explanation. We should not say that human beings disappear from the process: they remain indispensable. The fetishistic appearance is subtler. The human, technical, semantic, and institutional relations continue to operate, but their contribution to the authority of the result can recede behind the visible machine verdict.

This is also where the distinction between rational reliance and fetishism becomes decisive. A mathematician may rely on Lean because its kernel is reliable. A journal may require a formal artifact because it provides a valuable check. A reader may trust an expert’s assessment that the formal proposition matches the intended theorem. None of these practices is fetishistic merely because they involve trust. The stronger diagnosis applies only when the credential is made to function as a self-sufficient source of authority, when its scope is extended beyond the formal proposition and documented specification relation, and when this representation has a role in legitimation or institutional practice.

For clarity, three questions must therefore remain distinct. First, does the credential claim more than the formal check establishes? Second, does the authority appear to reside in the credential itself rather than in the relations that make it meaningful? Third, does this representation do something in practice—authorize a result, allocate credibility, close a dispute, or shape institutional recognition? A scope mismatch alone does not prove fetishism. The omission of contributors alone does not prove objectal displacement. And a symbolic representation without any identifiable practical or institutional role is not yet evidence of a reproduced ideological practice.

This is the point at which the analysis becomes genuinely Žižekian rather than a general complaint about technological overconfidence. The issue is not simply that a machine is granted too much trust. It is that the credential may serve as the object through which a demand for a final guarantee is staged and temporarily satisfied. The symbolic authority of the object is not an illusion detached from reality; it is supported by the real success of the technical procedure. The machine is persuasive because it genuinely verifies something. The question is whether that real success is made to bear the weight of a guarantee it cannot supply by itself.

The argument does not require that every case display the same mechanism. Fantasy and fetishism are related but not mechanically sequential. Disavowal is not a necessary stage. A case may exhibit a scene of closure without clear objectal displacement; it may foreground the machine without showing a wider scope extension; it may contain a public credential without any demonstrated institutional effect. The concept is useful only if it can distinguish these possibilities.

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

The four encounters do not form a progression from reliable technology to inevitable fetishism. They show that the same technical procedure can occupy different positions within mathematical knowledge production. In the Riemann case, formal checking is joined to institutional certification and then challenged at the foundational level. In Navier–Stokes, the relation between a formal declaration and a natural-language proof becomes the central point of dispute. In the Erdős case, human statement validation coexists with problems of artifact provenance. In Liquid Tensor, semantic scrutiny and collective labour are made visible as part of the formalization process.

The comparison matters because it prevents a simple conclusion. Formal verification is not inherently ideological. A machine check can be used in a way that accurately reflects its scope. A credential can remain embedded in a visible network of mathematical and institutional relations. Conversely, a genuine technical warrant can become a symbolic bearer of authority beyond the formal proposition it checks. The task is to identify the conditions under which this occurs, not to presume that it occurs whenever a proof assistant is used.

The analysis therefore distinguishes three questions. Does the public or institutional representation attribute to the credential a warrant broader than the formal proposition and its documented specification relation establish? Does the credential appear to contain this wider authority autonomously, while the relations that make it meaningful recede from view? And does this representation have a documented role in legitimation, recognition, credibility allocation, institutional action, or repeated practice? These questions concern, respectively, scope extension, objectal displacement, and social efficacy. They must be answered separately. A mismatch between a paper and a Lean file does not by itself establish fetishism. Nor does the omission of contributors from a short announcement. A diagnosis requires evidence that the credential is made to stand for more than it warrants, that its authority appears to reside in the object itself, and that this appearance does something in practice.

On the evidence considered here, no case establishes the full conjunction. Navier–Stokes is the strongest candidate for scope extension, but objectal displacement and credential-specific social efficacy remain uncertain. The Riemann case demonstrates institutional authorization, but the public record also makes expert vetting and independent checking visible. Erdős reveals the importance of human validation and artifact provenance, but does not show that the machine credential was treated as autonomous authority. Liquid Tensor provides counter-evidence by making semantic scrutiny an explicit part of the public account.

Does this mean that the concept of ideological fetishism has failed? No. It means that the concept must be used as a diagnostic instrument rather than a label applied in advance. Its value lies partly in the distinctions it forces us to make. It prevents us from confusing technical validity with semantic fidelity, semantic fidelity with mathematical understanding, or institutional recognition with the autonomous authority of a machine. It also prevents us from treating every form of justified epistemic dependence as ideological.

The originality of the present argument must be located against recent work. Vallverdú’s Locus Thesis provides a detailed account of the components of mathematical warrant and the conditions under which properties of a whole proof can be inferred from its parts (Vallverdú 2026). Kallel and El Louadi (2026) examine the relation between abundant proof checking and scarce human adjudication. López-Corona’s account of “studio mathematics” analyzes human-machine assemblages, provenance, mathematical understanding, agency, and responsibility in AI-assisted proof production (López-Corona 2026). Erfani (2026) directly examines ideological functions of AI systems, while Hourigan (2009) has already applied Žižek to technological fetishization and knowledge production. Omodeo (2019) develops a broader political epistemology of ideology in science studies.

The present article does not claim to be the first social epistemology of proof assistants, the first account of distributed mathematical labour, the first ideology critique of AI, or the first Žižekian critique of technology. Its contribution is narrower. It asks how the specific credential “Lean-verified” can become an objectal bearer of mathematical authority: how the genuine but bounded warrant of a formal checker may be made to stand for a wider claim, how the relations that make the credential meaningful may recede from view, and how this representation may acquire a legitimating role.

The point is not that the machine replaces the mathematician. The point is almost the reverse. The more mathematical knowledge depends on distributed labour, specialized expertise, and complex technical infrastructures, the more attractive a compact and portable credential of certainty may become. The credential can serve as a visible point of closure within a process that remains distributed. It is this relation between the real technical achievement and its possible symbolic enlargement that a Žižekian analysis makes available for examination.

A further distinction is necessary. The phrase “epistemic fetishism” has been used in analytic epistemology in a different sense by Ahlstrom-Vij (2021). The present article therefore uses the full expression “the ideological fetishism of formal verification” and does not claim to have coined the bare term. The proposed contribution is the specific Žižekian analysis of the Lean-verification credential and its possible objectal and legitimating function.

The ideological function of mathematical certainty is thus not that certainty is false. Formal verification can provide a real and powerful form of certainty. The question is whether a certainty achieved at one level is made to bear the authority of the whole. The fetish is not simply the machine. It is the appearance that the guarantee resides in the machine, when the authority of the credential depends on a wider network of relations.

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
