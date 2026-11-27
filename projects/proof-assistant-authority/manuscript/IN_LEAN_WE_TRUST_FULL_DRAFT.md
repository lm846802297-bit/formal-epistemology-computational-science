# The Ideological Fetishism of Formal Verification: A Žižekian Critique of Scientific Knowledge Production

**Manuscript:** *In Lean We Trust? The Ideology of Machine-Checked Proofs in Science*  
**Version:** First complete research draft  
**Evidence cut-off:** 27 November 2026

## Abstract

Formal verification is often presented as a way of overcoming uncertainty in mathematical and scientific knowledge. A proof assistant such as Lean can provide a genuine and reproducible guarantee: under a specified formal environment, its kernel checks whether a proof term establishes a given proposition. Yet the epistemic authority of this local procedure may travel beyond the proposition it checks. This article asks how the bounded technical warrant of formal verification can acquire an ideological function as a symbolic guarantee of broader scientific certainty. Drawing primarily on Slavoj Žižek's critique of ideology, it develops the concept of the **ideological fetishism of formal verification**. The analysis distinguishes three related operations: ideological fantasy, through which a local check may stage the closure of wider uncertainty; fetishism, through which collective epistemic labour appears as an autonomous property of the machine; and disavowal, through which symbolic investment may persist despite acknowledged limitations. The model is tested against four Lean cases: the Riemann hypothesis, Navier–Stokes, Erdős problems investigated with AlphaProof Nexus, and the Liquid Tensor Experiment. The cases do not show that Lean is inherently ideological. Rather, they reveal different conditions under which its technical reliability is either enlarged into a wider guarantee or kept within a transparent network of human, semantic, and institutional mediation. The article contributes a Žižekian account of the social-symbolic authority of formal verification while preserving the genuine epistemic value of machine checking.

**Keywords:** philosophy of science; social epistemology; ideology critique; Slavoj Žižek; formal verification; Lean; fetishism; mathematical proof

---

## 1. Introduction: What Is Ideological About a Correct Proof?

What, precisely, is ideological about a correct proof?

At first sight, the question seems to contain a contradiction. If a theorem has been formalized and its proof term accepted by Lean's kernel, then the machine has done exactly what it was designed to do. The result is not a matter of persuasion, rhetoric, or collective enthusiasm. A proof term either has the required type in the specified formal environment or it does not. Why, then, introduce the language of ideology? Would this not amount to treating a genuine mathematical achievement as a disguised exercise in power?

The objection is persuasive only if ideology is understood in the traditional sense of false consciousness: an erroneous representation that can be corrected by supplying the relevant facts. But this is precisely the understanding of ideology that Žižek's work puts into question. The ideological function of a claim cannot always be read directly from its truth or falsity. A proposition may be factually accurate and still participate in an ideological relation, depending on the position from which it is enunciated and the social practice it helps sustain (Žižek 1989; 1994; Flisfeder 2023). The question is therefore not simply whether the machine's verdict is true. It is what this verdict is made to mean.

Formal verification offers an unusually clear example of this problem because its technical achievement is both real and sharply delimited. Lean checks whether a proof term establishes a specified formal proposition under a specified environment. This is a powerful form of assurance. It can reduce the possibility of certain errors in a derivation, make proof artifacts reproducible, and permit independent checking. It does not, by itself, determine whether the formal proposition faithfully expresses the intended mathematical theorem, whether the theorem's assumptions are appropriate, whether the result is significant, or whether a wider scientific claim has been established.

The philosophical problem appears in the passage between these levels. A local and technically precise guarantee can become a public symbol of a much broader certainty. The machine may be invoked not merely as a checker of a formal proposition but as the visible point at which uncertainty itself seems to have been overcome. The paradox is that the machine need not fail for this ideological operation to occur. On the contrary, its genuine reliability may be what makes the wider symbolic investment possible.

This article investigates that paradox through the concept of the **ideological fetishism of formal verification**. The central hypothesis is:

> The epistemic authority of formal verification may be ideologically sustained when the genuine reliability of a bounded machine check is made to function as an autonomous guarantee of broader scientific certainty, while the human, conceptual, semantic, and institutional relations that make the verification meaningful recede from view.

The argument is not that Lean is unreliable, that mathematical truth is socially constructed, or that every appeal to machine verification is ideological. Nor is the argument that researchers or institutions necessarily intend to deceive. The object of analysis is more specific: the social-symbolic function acquired by the credential “Lean-verified” as it circulates through mathematical research, institutional recognition, and scientific communication.

The article makes three contributions. First, it reconstructs a Žižekian framework for analyzing formal verification through ideological fantasy, fetishism, and disavowal. Second, it proposes a diagnostic model that distinguishes a genuine technical warrant from its possible ideological enlargement. Third, it tests this model against four cases that differ in their visibility of human mediation and in the relation between formal artifacts and public claims: the Riemann hypothesis, Navier–Stokes, Erdős problems investigated with AlphaProof Nexus, and the Liquid Tensor Experiment.

The argument proceeds from a distinction that must remain intact throughout: a formally correct proof can coexist with an ideological representation of its authority. The critique does not concern the truth of the proof term as such. It concerns the transformation through which the authority of a local formal result may become the apparent guarantee of a much wider scientific order.

## 2. What Does Formal Verification Actually Guarantee?

### 2.1 The technical object of verification

A proof assistant such as Lean operates within dependent type theory. A mathematical proposition is represented as a formal type, and a proof is represented by a term inhabiting that type. Lean's kernel checks whether the term has the required type under the definitions, axioms, imported libraries, and formal environment in use.

The relevant technical claim is therefore precise:

\[
\text{Lean accepts } t : P
\]

means that, relative to the formal environment and trusted kernel, the term \(t\) is accepted as a proof of the proposition \(P\).

This is not a trivial achievement. A formal proof artifact can be replayed, inspected, and checked independently. Automation may help construct the proof, and a large elaboration process may transform human- or machine-generated commands into a proof term, but the kernel checks the resulting term against the formal proposition. The reliability of this process is a genuine epistemic resource.

Yet the expression “Lean verified the theorem” can conceal several distinct claims. The kernel checks a formal derivation. It does not independently determine whether the formal statement is the theorem that mathematicians intended to prove. Nor does it establish the significance of the result or its place in a scientific discipline. The distinction is not a criticism of Lean. It is a specification of what Lean does.

### 2.2 Five levels of epistemic warrant

For the purposes of this article, five levels must be distinguished.

| Level | Question | What establishes it? |
|---|---|---|
| Derivational validity | Does the proof term establish the formal proposition? | Kernel checking under a specified formal environment |
| Statement identity | Is the formal proposition the intended theorem? | Comparison with the source statement and mathematical formulation |
| Semantic correspondence | Does the formalization faithfully represent the intended mathematical claim? | Mathematical interpretation, definition checks, and expert scrutiny |
| Mathematical understanding | Can the proof be interpreted, explained, reconstructed, and assessed? | Mathematical exposition and competent human engagement |
| Epistemic significance and recognition | Is the result novel, important, and accepted as relevant by the discipline? | Expert assessment, publication, institutional procedures, and community deliberation |

These levels are connected, but none should be silently substituted for another. A kernel-accepted proof term establishes derivational validity. It does not automatically establish the remaining levels.

This distinction is already developed in important prior work. Kallel and El Louadi (2026) distinguish derivational validity, representational fidelity, and epistemic significance, and argue that the availability of abundant machine checking does not eliminate the need for human adjudication. Their analysis is a close predecessor, and the present article does not claim the distinction itself as original. Duede and Davey (2025), meanwhile, argue that transparent proof-checking can provide genuine mathematical knowledge even when a proof is generated by an opaque AI system. Their argument is equally important: machine checking is not merely a symbolic performance. It can provide real epistemic warrant (Kallel and El Louadi 2026; Duede and Davey 2025).

The question of this article begins after these points have been accepted. If machine verification is genuinely valuable, how does its authority acquire meanings beyond the formal proposition it checks?

### 2.3 Rational dependence and the social conditions of knowledge

The answer cannot be that non-specialists should simply inspect every proof themselves. Modern knowledge depends on a division of epistemic labour. Hardwig's account of epistemic dependence explains why it may be rational for an individual to rely on an expert whose evidence and competence they cannot personally reproduce (Hardwig 1985). Earlier work on mathematical proof likewise emphasizes that confidence in proofs develops through social processes of criticism, communication, and acceptance rather than through formal derivation alone (De Millo, Lipton, and Perlis 1979). This dependence is not necessarily a defect. It is one of the conditions under which complex scientific knowledge is possible.

The same point applies within mathematics. A formal proof depends on theorem formulation, definitions, libraries, software, and expert interpretation. No single participant necessarily possesses or independently checks every element of this network. The existence of such dependence does not make the result irrational or ideological. It makes the question of authority unavoidable.

Hardwig therefore provides a normative baseline: reliance on experts and technical systems can be justified. Žižek's contribution is different. He helps explain how a particular form of warrant can become symbolically invested with a promise of certainty that exceeds its epistemic scope. The present analysis does not replace social epistemology with ideology critique; it asks what the latter reveals that a normative account of justified dependence does not by itself explain.

## 3. A Žižekian Critique of the Ideology of Formal Verification

### 3.1 Ideology beyond false consciousness

In “The Spectre of Ideology,” Žižek rejects the assumption that ideology can be identified simply with false propositions or distorted representations. The explicit content of a claim may be factually correct, while its ideological function depends on the social position from which it is articulated and the relations it helps reproduce (Žižek 1994, especially 8–10). This is not the claim that every true statement is ideological. It is the claim that factual truth alone cannot settle the question.

This distinction is decisive for the present study. The statement “Lean checked this proof” may be entirely accurate. The ideological question is what this statement is made to authorize. Does it refer to the exact formal proposition, or does it become a credential for a broader claim about the correctness, significance, or final acceptance of a scientific result?

The critique must therefore move beyond a simple opposition between truth and falsehood. The object is the relation between a true technical statement and the wider symbolic function it may perform.

Žižek's account also directs attention to the material and practical dimensions of ideology. In “The Spectre of Ideology,” he distinguishes explicit doctrines, the materiality of ideological apparatuses, and the more elusive spontaneous ideology operating within social reality itself (Žižek 1994, 9–10). Applied here, the analysis cannot be limited to headlines. It must examine technical repositories, checking procedures, expert review, institutional announcements, and repeated practices of relying on formal verification.

### 3.2 Ideological fantasy: the scene of closure

In *The Sublime Object of Ideology*, fantasy is not merely a false picture that conceals an otherwise complete reality. It provides coordinates through which reality is experienced and social practice becomes intelligible. Fantasy can sustain the appearance of consistency where the social order remains incomplete or antagonistic (Žižek 1989, 28–31).

The hypothesis of this article is that formal verification can stage a scene of closure. A complex process of mathematical reasoning, formalization, software development, and expert assessment appears to culminate in a short and reproducible verdict: verified. The formal checker becomes the visible point at which uncertainty seems to have been resolved.

The fantasy is not that Lean literally proves empirical reality. It is not even necessary that anyone explicitly believes that it does. The issue is whether the certainty achieved at the formal level comes to symbolize closure at other levels: the identity of the formal statement with the intended theorem, the adequacy of its assumptions, the understanding of the proof, or the acceptance of the result by the mathematical community.

The structure can be represented as follows:

\[
\text{Formal proposition}
\longrightarrow
\text{Kernel acceptance}
\]

is a technical relation. By contrast,

\[
\text{Kernel acceptance}
\longrightarrow
\text{Scientific certainty as such}
\]

is not a conclusion supplied by Lean. It is a possible symbolic extension.

Why is this extension attractive? The formal check makes one part of an otherwise difficult-to-survey process visible, reproducible, and communicable. The complexity of the proof may remain inaccessible, but the result of the checking procedure can be stated in a compact form. The visible credential can therefore offer an image of closure in a context where the wider production of knowledge remains distributed and difficult to inspect.

The ideological fantasy of verification names this possible function. It does not imply that every public reference to a checked proof participates in the fantasy. A statement that accurately identifies the formal proposition, assumptions, and status of review may preserve the technical scope rather than enlarge it.

### 3.3 Fetishism: from collective epistemic labour to machine autonomy

The second mechanism is more specific. In *Capital*, Volume I, Chapter 1, Section 4, Marx analyzes commodity fetishism as a form of social appearance in which relations among producers assume the form of relations among things. The point is not merely that the human labour behind a commodity is forgotten. The social relation itself appears in an objectified form.

Žižek's discussion of commodity fetishism in *The Sublime Object of Ideology* emphasizes how an effect generated by a network of relations can appear as an immediate property of one element within that network (Žižek 1989, 19–20). This provides the theoretical basis for the article's proposed concept: **the ideological fetishism of formal verification**.

The authority of a Lean-checked result depends on a network of relations. Researchers select a problem and formulate an intended theorem. Mathematicians develop definitions and arguments. Formalizers encode statements and proof strategies. Library maintainers provide formalized mathematics. Software developers maintain the kernel and infrastructure. Experts assess whether the formal proposition corresponds to the intended mathematics. Institutions and journals assess significance and responsibility. Communicators explain the result to wider audiences.

These contributions are not interchangeable, and they do not all perform the same epistemic function. The kernel's checking is real; human labour does not create the mathematical validity of a proof term. But the authority of the formal result as a claim about a particular mathematical problem depends on the relations that connect the formal artifact to that problem and situate it within a mathematical community.

The fetishistic hypothesis arises when the authority produced and mediated through this network appears as an autonomous property of the machine. The public statement “Lean verified it” can be accurate at the level of derivational validity while simultaneously condensing a much wider set of relations into the apparent agency of a single technical object.

The proposed concept can be stated as follows:

> **The ideological fetishism of formal verification occurs when the socially mediated authority of a machine-checked result appears as an autonomous property of the machine, while the human, semantic, and institutional relations that make the check relevant recede from view.**

The commodity analogy is structural, not an identity. Lean is not a commodity in Marx's technical economic sense, and mathematical truth is not produced by collective labour in the same way that commodities are produced. The analogy concerns the form of appearance through which a network-dependent epistemic authority can be attributed to an apparently autonomous object.

This is more than a criticism of technological admiration. Nor is it enough to observe that a headline omits the names of formalizers. A diagnosis of fetishism requires evidence that the machine is represented or used as an independent source of authority while the relations necessary to interpret its result are displaced.

### 3.4 Disavowal: knowing the limit and sustaining the guarantee

The third mechanism concerns the possible persistence of symbolic investment after a limitation has been acknowledged. Žižek's discussion of cynical ideology draws on Sloterdijk's critique of cynical reason. The familiar formula that subjects know what they are doing and nevertheless continue to do it should not be presented as a phrase originally coined by Žižek (Žižek 1989, 24–27).

For the present study, it is important to distinguish two forms of disavowal. Black (2025) distinguishes cynical disavowal from fetishistic disavowal. Cynical disavowal involves a manipulative distance between acknowledged knowledge and practice. Fetishistic disavowal can acknowledge the relevant state of affairs while preserving the attachment sustained by the fetish object. Kuldova (2019) similarly emphasizes that fetishism should not be reduced to simple misrecognition.

Applied to Lean, the relevant question is not merely whether researchers know that formal verification has limits. Many researchers state those limits clearly. The question is whether the technical object continues to function as a broader guarantee despite that knowledge.

A strict diagnosis requires more than finding a caveat next to an ambitious headline. It requires evidence that the same actor or institutional communication chain acknowledges a precise limitation and nevertheless continues to communicate or act as if the verification guarantees a wider claim. If the surrounding text preserves the proper scope, or if the claim is later corrected, the discrepancy may not constitute disavowal at all.

Disavowal is therefore a conditional mechanism. It is not necessary for every instance of fetishism, and no individual's unconscious motive can be inferred from public wording alone.

### 3.5 The missing guarantee: the Big Other as structural background

The Lacanian notion of the Big Other provides a further background to the argument, but it is not a fourth co-equal mechanism. The Big Other is not a person, institution, or software system. It names the symbolic locus of norms, recognition, and authorization. The Lacanian claim that there is no Other of the Other means that no final signifier can guarantee the consistency of the symbolic order from outside (Lacan 2019, Seminar VI, ch. XVI).

Lean is not the Big Other. It may, however, be positioned as a technical credential within a symbolic order that seeks a guarantee of scientific knowledge. The machine's output can be treated as if it supplies a final point of authorization, even though its actual guarantee remains conditional on a formal proposition, definitions, assumptions, and a trusted environment.

The point is not that scientific authority is unreal. Mathematical communities, journals, institutions, and technical systems do exercise real forms of authority. The point is that no single element can guarantee every level of scientific knowledge. The Big Other and its lack help explain why a local technical guarantee may be invested with the symbolic function of a final one.

### 3.6 Three empirical planes

The theoretical model is examined across three planes drawn from Žižek's “The Spectre of Ideology”:

1. **Discursive plane:** explicit statements in papers, repositories, announcements, institutional pages, and media reports.
2. **Material-institutional plane:** the actual procedures of formal checking, statement validation, expert review, publication, and institutional recognition.
3. **Spontaneous-practical plane:** repeated practices in which a Lean credential is treated as a routine warrant for a broader claim.

The third plane requires evidence of repeated practice. It cannot be inferred from a single headline. The three planes are empirical dimensions, not additional ideological mechanisms. Fantasy, fetishism, and disavowal may operate across all three.

## 4. The Analytical Model and Case-Study Method

### 4.1 Conditions and operations

The model distinguishes conditions of possibility from ideological operations. Four conditions make the phenomenon possible:

- scientific knowledge is produced through a division of epistemic labour;
- Lean provides a genuine and visible form of local technical assurance;
- semantic and institutional mediation connects the formal artifact to the intended mathematical claim;
- no single technical or institutional credential can guarantee every level of scientific knowledge.

These conditions do not automatically produce ideology. The ideological operations must be demonstrated.

| Operation | Theoretical question | Analytical function |
|---|---|---|
| Fantasy | What scene makes the practice appear coherent and complete? | The local check may stage the closure of wider uncertainty |
| Fetishism | How do social relations appear as properties of an object? | Collective mediation may appear as autonomous machine authority |
| Disavowal | How can investment persist when limits are known? | A broader symbolic guarantee may persist despite acknowledged boundaries |

Fantasy and fetishism are mutually reinforcing analytical dimensions, not consecutive stages in a deterministic process. Disavowal is conditional.

### 4.2 Diagnostic threshold

A strong diagnosis of the ideological fetishism of formal verification requires four conditions:

- **T — Technical warrant:** the exact formal proposition and the actual Lean check are identified.
- **E — Epistemic enlargement:** a representation or practice attributes to the formal credential a broader warrant than the checked proposition and documented semantic bridge establish.
- **F — Fetishistic displacement:** the authority generated through collective epistemic and institutional relations appears as an autonomous property of the machine.
- **R — Reproduction:** the enlargement and displacement recur or have a documented institutional or practical role; they are not merely an isolated phrase.

The diagnostic form is:

\[
\boxed{T \land E \land F \land R}
\]

This is an operational criterion developed for the present study, not a formula taken from Žižek. Disavowal is tested separately and is not required for the core diagnosis.

The model also specifies counter-evidence. It is weakened where public and institutional descriptions consistently identify the exact formal proposition, make semantic correspondence explicit, acknowledge human contributions, and treat Lean as one component in a wider process of assessment. Ordinary shorthand, genre conventions, surrounding qualifications, and subsequent corrections must also be considered.

### 4.3 Comparative case design

The article uses a source-based comparative analysis of four Lean cases. Each case is examined through the same questions:

1. What exact mathematical proposition is represented as proved?
2. What does the Lean artifact actually establish?
3. What is the relation between the formal proposition and the intended mathematical claim?
4. Which human, technical, semantic, and institutional relations make the result meaningful?
5. How do the researchers, institutions, and media represent the result?
6. What evidence supports the ideological mechanisms, and what evidence resists them?

The cases were selected because they vary in formal verification, human validation, institutional recognition, and public representation. They are not intended to represent all proof-assistant use. The study does not infer population-level beliefs from public texts, nor does it diagnose unconscious motives. It examines documented claims and practices.

## 5. Four Lean Cases

### 5.1 Riemann hypothesis: formal certification and the limits of closure

On 20 November 2026, Levent Alpöge published a note stating that he believed he had discovered a proof of the Riemann hypothesis while working with Claude (Alpöge 2026). The result was released as a Lean 4 development. The original archive was exceptionally large, and subsequent work produced a more compact formalization. The Lean FRO and Mathlib community issued a joint statement on 21 November describing the formal statement and verification process. Waterloo's subsequent verification record reported compilation, kernel replay, statement comparison, and independent checking of the compact development (Lean FRO and Mathlib Initiative 2026; University of Waterloo 2026). By 26 November, a 1,582-page exposition generated by several AI models from the Lean source and cross-checked had also been made available (rh-lean-roadmap 2026).

These developments provide substantial technical evidence. The formal proof terms were checked, the statement was compared with the Mathlib formulation, and independent checking procedures were reported. It would be mistaken to dismiss this achievement as merely rhetorical. The formal certification is a genuine part of the case.

The ideological question concerns what this certification is made to signify. Public descriptions such as “AI solves the Riemann hypothesis” can stage the scene of a historically unresolved problem receiving a decisive machine verdict. The scale of the formal archive and the multiplicity of checker results make the technical credential unusually visible. This can support a fantasy of closure: a difficult mathematical problem appears to have been settled by a reproducible procedure.

Yet the case also contains important counter-evidence. The Lean community and Waterloo materials explain the formal statement, the checking process, and the contributions involved. Expert commentary distinguishes formal certification from mathematical understanding and broader community acceptance. The extensive AI-mediated exposition provides a route into the argument, but its existence does not by itself establish that the mathematical community has independently understood and accepted every part of the proof.

The fetishism hypothesis is therefore mixed. Compressed narratives that foreground “Claude + Lean” can background the mathematician's direction, formalization work, Mathlib, kernel and checker developers, and expert assessment. But the technical and institutional record makes much of this network visible. The available evidence supports the possibility of fetishistic displacement in selected public representations, not a general conclusion that the case is dominated by machine autonomy.

No strict form of disavowal is established. The public record includes qualifications and technical explanations, and there is insufficient evidence that the same actor knowingly maintained an enlarged guarantee in practice after acknowledging its limits.

The Riemann case is therefore ambivalent. It shows that very strong formal certification can coexist with unresolved questions about understanding, exposition, and institutional acceptance. It does not show that the machine's result is false, nor that its authority is automatically fetishistic.

### 5.2 Navier–Stokes: formal validity and disputed semantic correspondence

On 8 September 2026, OpenAI announced a proof claim concerning finite-time singularity formation for three-dimensional incompressible Navier–Stokes equations with smooth forcing and published a Lean formalization (OpenAI 2026). The announcement presented the result as a solution to a Millennium Prize Problem. The formal repository provides declarations and proof artifacts that can be checked by Lean's kernel.

The crucial dispute concerns not whether the kernel accepts the formal declarations, but whether those declarations faithfully correspond to the separate natural-language proof. Bastounis, Circelli, and Hansen (2026) reported discrepancies between the written proof and the Lean formalization (Bastounis, Circelli, and Hansen 2026; King's College London 2026). Among them, the inverse estimate in Lemma 8.6 uses \(m+4\) input derivatives in the written proof, whereas the corresponding Lean declaration uses \(m+5\). They also identify a difference in the pressure-flux estimate and proof route. These discrepancies concern the relation between two proof artifacts. They do not establish a kernel failure, nor do they prove that the underlying Navier–Stokes theorem is false.

This case provides the strongest test of the distinction between formal validity and semantic correspondence. A proof term can be correctly checked for a formal declaration while the relation between that declaration and a separate natural-language argument remains disputed. The machine's local guarantee does not settle the translation relation.

The fantasy of verification is particularly visible here. An announcement of a solution to a Millennium Prize Problem accompanied by Lean verification can be read as a machine-certified settlement of the entire claim. But the kernel checks the formal declarations, not the correspondence between every declaration and every estimate in the written paper. The public credential may therefore carry a wider meaning than the technical artifact warrants.

The fetishism hypothesis is also strongest in this case. The kernel's real authority over formal declarations can stand in for the semantic work required to establish that the declarations faithfully represent the written proof. The machine appears to guarantee the whole result, while the relation between the formal and natural-language objects depends on mathematical interpretation and comparison.

Yet the counter-evidence matters. The repository is public, the independent critique is public, and the discrepancy has become an explicit subject of discussion. The mismatch is not wholly concealed. This makes it difficult to claim that the case demonstrates a settled or systematic disavowal. The existence of a dispute is evidence of contestation, not evidence of cynical intent.

Navier–Stokes is thus the strongest candidate for epistemic enlargement and fetishistic displacement, but the full diagnostic threshold is not yet met. In particular, the reproduction condition requires evidence that the enlarged credential continues to perform an institutional or practical role after the correspondence problem has been acknowledged. The case is analytically powerful precisely because it shows how a valid local check can become entangled with a disputed semantic bridge.

### 5.3 Erdős problems and AlphaProof Nexus: the visibility of mediation

Tsoukalas et al. (2026) report that AlphaProof Nexus solved nine problems among 353 open Erdős problems represented in a formal conjecture repository and produced 44 proofs among 492 OEIS conjectures attempted. These denominators describe the formalized benchmark and attempted problems, not all open Erdős problems. The system alternates language-model-generated proof attempts with Lean checking. The published study reports human validation of the correspondence between the nine formal Erdős statements and the intended conjectures, and manual review of OEIS formalizations.

This workflow is important because it makes the division of epistemic labour relatively visible. The AI system searches for proof strategies, Lean checks formal proof terms, and human experts assess the relation between formal statements and intended conjectures. The result is not presented solely as a machine's autonomous verdict.

A source-level audit nevertheless identified provenance and statement-correspondence issues that require precision. For problem #26, the top-level Lean target is a lower-density Tenenbaum variant rather than the upper-density theorem described in the prose. However, the same file contains a stronger uniform pointwise lemma sufficient to establish the prose result. For #741(i), the linked AlphaProof file proves an exact-density counterexample, while an upper-density theorem exists separately in the Formal Conjectures repository. For #741(ii), the cited arXiv link points to a file for another problem, while the relevant formalization is available elsewhere. These findings concern the identity and provenance of particular artifacts. They do not establish a kernel failure or invalidate all reported results.

The fantasy test is therefore limited and context-dependent. Headlines such as “AI solves Erdős problems” can suggest autonomous discovery beyond the benchmark. The primary paper, however, reports denominators, formalized statements, Lean verification, and human validation. It preserves qualifications that compressed media descriptions may omit.

The fetishism hypothesis is also weaker than in Navier–Stokes. If the result is attributed only to AlphaProof Nexus, the role of conjecture curation, formal statement design, Lean, and human validation may recede. But the published workflow makes much of this mediation visible. The case therefore functions as a mixed example and a counter-test: formal verification can be integrated into a transparent human-AI research process without necessarily producing an autonomous-machine narrative.

No disavowal is established. Artifact-link problems alone do not show that an actor knowingly maintained a broader guarantee after acknowledging the relevant limitation.

### 5.4 Liquid Tensor Experiment: a counter-case of visible collective labour

The Liquid Tensor Experiment provides a historical counter-case. The Lean community announced completion of the formal verification of the main theorem of liquid vector spaces in July 2022 (Lean Community 2022). The result concerns the vanishing of higher Ext groups for specified condensed real vector spaces:

\[
\operatorname{Ext}^{i}\bigl(\mathcal{M}_{p'}(S),V\bigr)=0,
\qquad i\geq 1.
\]

The completion announcement identifies contributors and credits mathematical support, formalization work, Mathlib dependencies, and institutional assistance. Scholze's contemporaneous account emphasizes the role of human mathematical interaction and scrutiny in establishing confidence (Scholze 2021). Adam Topaz's later discussion addresses the possibility of pathological or incorrect definitions and explains the use of readable sanity-check examples for mathematicians with limited Lean experience (Topaz 2022).

This case is important because the collective process is not merely an invisible background condition. It is part of the public account of the result. Lean provides a genuine formal guarantee, but the mathematical community also makes visible the work required to ensure that the formal definitions correspond to the intended mathematics.

A media headline that says Lean “confirmed” a proof may still create a compressed image of technical closure. Yet the primary project record resists the idea that the machine is an autonomous source of mathematical authority. The formal result is embedded in a transparent network of mathematicians, formalizers, libraries, and definition checks.

The fantasy of closure is therefore weakly supported, and the fetishism hypothesis is weaker still. The case does not show that formal verification is inherently fetishistic. It shows that the authority of a proof assistant can be integrated into a visible collective practice in which human interpretation remains central.

Liquid Tensor is consequently not an inconvenient exception to the theory. It is necessary to the theory's validity. If every use of Lean were automatically classified as ideological fetishism, the concept would explain nothing. A counter-case establishes the conditions under which formal verification can remain a bounded and transparent epistemic practice.

## 6. Comparative Analysis: When Does the Credential Become Ideological?

The four cases do not form a simple progression from technical verification to ideological authority. They show different relations among the formal object, semantic mediation, collective labour, and public representation.

| Case | Fantasy of closure | Fetishistic displacement | Disavowal | Analytical role |
|---|---|---|---|---|
| Riemann | Plausible but qualified | Possible in compressed accounts; countered by detailed records | Not established | Ambivalent case: high formal certainty and layered recognition |
| Navier–Stokes | Strongest candidate | Strongest candidate | Not established | Formal validity versus disputed semantic correspondence |
| Erdős / AlphaProof Nexus | Limited and context-dependent | Weak to mixed | Not established | Transparent mediation and provenance test |
| Liquid Tensor | Weak | Weak | Not established | Counter-case: visible collective labour and semantic scrutiny |

The comparison supports three conclusions.

First, formal verification is not intrinsically ideological. The same technical procedure can be embedded in different social and institutional practices. Where the exact proposition, human contributions, semantic checks, and review status remain visible, the machine can function as one component of a wider process rather than as an autonomous guarantor.

Second, the strongest ideological candidate is not necessarily the case with the most impressive technical achievement. The Riemann case contains extensive checking and independent certification, but it also contains detailed technical records and expert qualifications. Navier–Stokes is more revealing because the formal artifact and the natural-language proof have a disputed correspondence. The issue is not that Lean failed to check its declarations. It is that the authority of this successful check may be made to stand for a relation that the check itself does not establish.

Third, the absence of evidence for cynical disavowal is significant. None of the four cases currently supports a strict claim that actors knowingly maintained an enlarged guarantee in a manipulative way. The analysis should not convert every discrepancy into a diagnosis of bad faith. The central concept of ideological fetishism does not require such a psychological accusation. It concerns the form in which collective epistemic relations may appear as autonomous machine authority.

The comparative result can be stated as follows:

\[
\text{Technical reliability}
\not\Rightarrow
\text{ideological fetishism}.
\]

Rather, the ideological diagnosis requires the conjunction of a genuine technical warrant, an identifiable enlargement of its scope, the displacement of collective mediation into machine autonomy, and the reproduction of that representation in practice or institutional communication.

## 7. Discussion: The Real Machine and the Symbolic Guarantee

### 7.1 Why the machine's reliability matters

The ideological critique of formal verification would be trivial if Lean were simply unreliable. One could then explain the authority of the system as a mistaken belief in a defective instrument. But this is not the phenomenon under investigation. Lean's technical reliability is real, and its epistemic value should be recognized.

The more difficult question is why a real technical guarantee may become the support of a wider symbolic promise. The kernel checks a formal proposition. The scientific claim, however, is embedded in semantic interpretation, mathematical understanding, expert evaluation, and institutional recognition. The technical procedure does not abolish these relations. It makes one part of them unusually visible.

This is where the Žižekian framework adds something to a normative account of epistemic dependence. Hardwig explains why reliance on experts and distributed knowledge can be rational. Duede and Davey explain why transparent proof checking can provide genuine mathematical knowledge. Kallel and El Louadi show why the abundance of machine checking does not remove the scarcity of human adjudication. The present article asks a different question: why does the visible credential of a local check sometimes acquire the symbolic function of a guarantee for a wider epistemic order?

### 7.2 The fetish is not the machine itself

The phrase “epistemic fetishism” may suggest that the problem lies in excessive admiration of technology. That interpretation is insufficient. The fetishistic operation is not simply an attitude toward a machine. It concerns a form of appearance in which the authority generated through a network of relations is attributed to the object as if it were self-grounding. A terminological qualification is necessary: Ahlstrom-Vij (2021) uses “epistemic fetishism” in a different analytic-epistemological sense. The present article therefore uses the full expression “the ideological fetishism of formal verification” and does not claim to have coined the bare term.

This distinction also marks the limit of the Marxian analogy. The present article does not claim that formal verification is a commodity form or that the social relations of mathematical labour are identical to capitalist relations of production. It borrows the structural insight that a relation-dependent effect can appear as an intrinsic property of an object. The machine's technical function is real; the fetishistic displacement concerns the apparent autonomy of the wider authority attributed to it.

### 7.3 The political-epistemological significance

The paper belongs primarily to philosophy of science, with a critical orientation in social and political epistemology. Political epistemology has examined the ideological dimensions of scientific knowledge and science studies (Omodeo 2019). Hourigan (2009) has already applied Žižek to technological fetishization and knowledge production; the present contribution is narrower, focusing on the formal proof assistant, the exact boundary of its technical warrant, and the symbolic authority that may accrue to the credential “Lean-verified”. Its object is not AI consciousness, general public trust in artificial intelligence, or the social consequences of automation in general. It is the specific role of formal verification in the production and legitimation of mathematical and scientific knowledge.

The ideological question is therefore also a question about scientific authority. Scientific communities must establish reliable procedures, distribute epistemic labour, and communicate results to audiences that cannot reproduce every stage of inquiry. These requirements are legitimate. Yet the credentials used to make knowledge publicly legible can become symbols of a certainty that exceeds their scope.

A Žižekian critique does not ask science to abandon technical verification. It asks that the social relations and semantic conditions through which a verification result becomes meaningful remain visible. The issue is not whether science needs guarantees; it is whether a local guarantee is made to stand in for a final one.

### 7.4 Limits of the present evidence

The four cases support an analysis of technical artifacts, institutional representations, and documented practices. They do not establish how the general public actually interprets Lean verification. A headline can invite a particular reading without proving that readers adopt it. Nor can public texts establish unconscious motives. Claims about audience belief would require separate audience research, which is outside the scope of this article.

The present study therefore makes a deliberately bounded claim. It identifies the conditions under which formal verification can acquire an ideological function and shows how those conditions appear, or fail to appear, in four cases. It does not claim that all formal verification is fetishistic or that every public appeal to Lean constitutes disavowal.

## 8. Conclusion

What is ideological about a correct proof? Nothing follows from its correctness alone. A proof term accepted by Lean's kernel provides a genuine and valuable form of formal assurance. The ideological question begins when this local warrant acquires a symbolic function beyond the proposition it checks.

Drawing on Žižek's critique of ideology, this article has developed the concept of the ideological fetishism of formal verification. Ideological fantasy explains how a bounded check may stage the closure of wider scientific uncertainty. Fetishism explains how the collective epistemic relations that make a formal result meaningful may appear as an autonomous property of the machine. Disavowal identifies a possible persistence of symbolic investment despite acknowledged limitations, although the four cases do not establish cynical disavowal.

The comparative analysis also shows why the theory must remain conditional. Riemann is ambivalent: extensive technical certification coexists with layered questions of exposition and recognition. Navier–Stokes is the strongest candidate for scope enlargement and fetishistic displacement because the authority of kernel-checked declarations can be made to stand for a disputed semantic correspondence. Erdős demonstrates how explicit human validation and provenance issues complicate simple narratives of autonomous machine discovery. Liquid Tensor provides a counter-case in which collective mathematical labour and semantic scrutiny remain visible.

The central conclusion is therefore not that machines have replaced human judgment, nor that formal verification is an illusion. It is more precise: **a machine can correctly verify a formal proposition and still become the bearer of an ideological promise that exceeds that proposition.** The authority of the machine is real at one level; its wider symbolic function is a separate question.

The task of ideology critique is not to expose the machine as false. It is to explain how a real technical guarantee can be made to appear as the guarantee of an entire scientific order. In this sense, the most revealing feature of formal verification is not that it removes the need for human judgment, but that its genuine success can make the continuing need for such judgment less visible.

---

## References

Ahlstrom-Vij, Kristoffer. 2021. “Esoteric Reliabilism.” *Episteme* 18 (4): 603–623. https://doi.org/10.1017/epi.2019.39.

Alpöge, Levent. 2026. Research note on a Claude-assisted Lean proof of the Riemann hypothesis, 20 November. https://alpo.ge/.

Bastounis, Dimitrios, Marco Circelli, and Jonas Hansen. 2026. Independent analysis of the correspondence between OpenAI's Navier–Stokes paper and Lean formalization. arXiv:2610.08144. https://arxiv.org/abs/2610.08144.

Black, Jack. 2025. “Examining the Mechanism of Disavowal and Its Two Forms: Cynical Disavowal and Fetishistic Disavowal.” *Theory & Psychology* 35 (1): 117–135. https://doi.org/10.1177/09593543241308199.

De Millo, Richard A., Richard J. Lipton, and Alan J. Perlis. 1979. “Social Processes and Proofs of Theorems and Programs.” *Communications of the ACM* 22 (5): 271–280. https://doi.org/10.1145/359104.359106.

Duede, Eamon, and Kevin Davey. 2025. “A Priori Knowledge in an Era of Computational Opacity: The Role of Artificial Intelligence in Mathematical Discovery.” *Philosophy of Science* 92 (5): 1394–1404. https://doi.org/10.1017/psa.2025.10160.

Flisfeder, Matthew. 2023. “There Is No Metalanguage; or, Truth Has the Structure of a Fiction: The Žižekian System, between Post-Ideology and Post-Truth.” *Enrahonar* 70: 171–185. https://doi.org/10.5565/rev/enrahonar.1420.

Hardwig, John. 1985. “Epistemic Dependence.” *The Journal of Philosophy* 82 (7): 335–349. https://doi.org/10.2307/2026523.

Hourigan, Daniel. 2009. *The Phantasmatic Subject of Technology: Slavoj Žižek, Techne, and the Abyss*. PhD thesis, Griffith University. https://doi.org/10.25904/1912/3124.

Kallel, Maher, and Mohamed El Louadi. 2026. “Verification Abundance, Adjudication Scarcity: What Happens to Mathematical Knowledge When Proof Checking Becomes Free.” arXiv:2608.28997. https://arxiv.org/abs/2608.28997.

Kuldova, Tereza Østbø. 2019. “Fetishism and the Problem of Disavowal.” *Qualitative Market Research: An International Journal*. https://doi.org/10.1108/QMR-12-2016-0125.

Lacan, Jacques. 2019. *Desire and Its Interpretation: The Seminar of Jacques Lacan, Book VI*. Edited by Jacques-Alain Miller. Translated by Bruce Fink. Cambridge: Polity. Chapter XVI, “There Is No Other of the Other.”

Marx, Karl. 1976 [1867]. *Capital: A Critique of Political Economy*, vol. 1. Translated by Ben Fowkes. London: Penguin. Chapter 1, section 4, “The Fetishism of Commodities and the Secret Thereof.”

Omodeo, Pietro Daniel. 2019. *Political Epistemology: The Problem of Ideology in Science Studies*. Cham: Springer. https://doi.org/10.1007/978-3-030-23120-0.

Scholze, Peter. 2021. “Half a Year of the Liquid Tensor Experiment: Amazing Developments.” 5 June. https://xenaproject.wordpress.com/2021/06/05/half-a-year-of-the-liquid-tensor-experiment-amazing-developments/.

Topaz, Adam. 2022. “Liquid Tensor Experiment: Sanity Checks.” 14 October. https://leanprover-community.github.io/blog/posts/lte-examples/.

Tsoukalas, et al. 2026. “Advancing Mathematics Research with AI-Driven Formal Proof Search.” *Science* 394 (6820), 8 October. https://doi.org/10.1126/science.aej2213.

Žižek, Slavoj. 1989. *The Sublime Object of Ideology*. London: Verso.

Žižek, Slavoj. 1994. “The Spectre of Ideology.” In *Mapping Ideology*, edited by Slavoj Žižek, 1–33. London: Verso.

### Primary case records

Lean FRO and Mathlib Initiative. 2026. “Riemann Hypothesis Formalization: Community Statement.” 21 November. https://leanprover-community.github.io/blog/posts/riemann-hypothesis/.

University of Waterloo. 2026. Verification and exposition materials for the Alpöge–Claude Riemann hypothesis formalization. https://www.math.uwaterloo.ca/~mrubinst/alpoge_claude_grh/.

OpenAI. 2026. “A Proof of the Navier–Stokes Equations.” 8 September. https://openai.com/index/navier-stokes-solution/.

King's College London. 2026. “OpenAI's Navier–Stokes Proof Called into Question.” 27 October. https://www.kcl.ac.uk/news/openais-navier-stokes-proof-called-into-question.



Science Media Centre Spain. 2026. Expert reactions to AlphaProof Nexus and the Erdős problem results. 8 October.

Lean Community. 2022. “Liquid Tensor Experiment: Final Completion Announcement.” 15 July. https://leanprover-community.github.io/blog/posts/lte-final/.

Omodeo, Pietro Daniel. 2019. *Political Epistemology: The Problem of Ideology in Science Studies*. Cham: Springer. https://doi.org/10.1007/978-3-030-23120-0.

Hourigan, Daniel. 2009. *The Phantasmatic Subject of Technology: Slavoj Žižek, Techne, and the Abyss*. PhD thesis, Griffith University. https://doi.org/10.25904/1912/3124.

rh-lean-roadmap. 2026. *The Riemann Hypothesis and GRH for Dirichlet L-Functions: A Readable Account of the Lean Proof in Alpöge's Archive*. Version 44. Zenodo, 26 November. https://doi.org/10.5281/zenodo.24562451.
