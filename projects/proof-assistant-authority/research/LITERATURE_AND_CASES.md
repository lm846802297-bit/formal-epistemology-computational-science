# Literature and public-case pilot: literature map and first findings

**Research project:** From Checking Proofs to Settling Claims  
**Research phase:** Initial literature and public-text pilot  
**Status:** In progress; not a completed systematic review  
**Scope:** Public textual construction of epistemic authority. No inference about actual reader belief or author motive.

## 1. Main finding

The initial survey supports a viable research question, but not yet a conclusion that proof-assistant discourse systematically overstates what has been checked. Existing social epistemology already explains why non-experts rationally depend on experts and institutions. Science-communication studies show that simplification and popularization are themselves practices through which expertise and authority are organized. Recent work on artificial epistemic authorities directly discusses whether AI systems can count as epistemic authorities.

The distinctive proposed contribution must therefore be narrower: compare the exact scope of formal verification with the scope attributed to it in project-authored and independent public texts, and identify when the latter attributes a wider scientific or mathematical verdict than the formal artifact and its documented semantic bridge warrant.

## 2. Literature map

### 2.1 Epistemic dependence and expert testimony

- John Hardwig, “Epistemic Dependence,” *The Journal of Philosophy* 82(7) (1985), 335–349. JSTOR stable record: https://www.jstor.org/stable/2026523. Foundational account of rational dependence on experts when an individual cannot personally possess or assess all relevant evidence.
- Ben Almassi, “Experts, Evidence, and Epistemic Independence,” *Spontaneous Generations* 1(1) (2007). DOI: https://doi.org/10.4245/sponge.v1i1.2972. Discusses Hardwig's account and the tension between rational dependence and epistemic independence.
- Fernando Broncano-Berrocal and Jesús Vega-Encabo, “A Taxonomy of Types of Epistemic Dependence,” *Synthese* 197 (2020), 2745–2763. DOI: https://doi.org/10.1007/s11229-019-02233-6. Offers a goal-relative taxonomy of epistemic dependence.
- Jeroen de Ridder, “How to Trust a Scientist,” *Studies in History and Philosophy of Science Part A* (2022). DOI: https://doi.org/10.1016/j.shpsa.2022.02.003. Useful for the content and justification of trust among scientists.
- George Kwasi Barimah, “Second-Order Assessment of Scientific Expert Claims and Sharing Epistemic Burdens in Science Communication,” *Episteme* (2022). DOI: https://doi.org/10.1017/epi.2022.11. Explains why non-experts cannot easily assess experts and why epistemic burdens should be shared in communication.

**Use in this paper:** Hardwig explains why delegation to a proof assistant, formalization expert, or research team can be rational. It does not by itself explain scope expansion. Dependence can be legitimate even when the dependent reader cannot inspect the proof. The key question becomes whether the chain of testimony preserves the distinction between what the kernel checked and what the scientific claim requires.

### 2.2 Science communication, popularization, and authority

- Stephen Hilgartner, “The Dominant View of Popularization: Conceptual Problems, Political Uses,” *Social Studies of Science* 20(3) (1990), 519–539. DOI: https://doi.org/10.1177/030631290020003006. Critiques the two-stage model of scientific knowledge followed by simplified public dissemination; shows how popularization discourse can sustain hierarchies of expertise.
- Harry Collins and Robert Evans, “The Third Wave of Science Studies: Studies of Expertise and Experience,” *Social Studies of Science* 32(2) (2002), 235–296. DOI: https://doi.org/10.1177/0306312702032002003. Distinguishes forms of expertise and the problem of extending technical decision authority.
- George Kwasi Barimah (2022), above. Relevant to second-order assessment and the allocation of epistemic burdens.
- Carrie Figdor, “Science Journalism and Epistemic Virtues in Science Communication: A Defense of Sincerity, Transparency, and Honesty,” *Episteme* (2023). DOI: https://doi.org/10.1017/epi.2023.38. Addresses epistemic virtues in science journalism and the relationship between institutional and individual communication.

**Use in this paper:** Do not treat every simplification as distortion. Code whether the scope is preserved, reasonably compressed, ambiguous, or substantively expanded. Analyze the public text as a communicative act, not as transparent access to the speaker's mental state.

### 2.3 Artificial and algorithmic epistemic authority

- “Artificial Epistemic Authorities,” *Social Epistemology* (2025). DOI: https://doi.org/10.1080/02691728.2025.2449602. Directly discusses whether AI systems can be recognized as artificial epistemic authorities, including identification and deference problems.

**Novelty implication:** It is no longer defensible to claim that this project is the first to ask whether non-human computational systems can acquire epistemic authority. The more specific contribution is the relation between a proof assistant's bounded verification relation and the broader scope of claims attributed to that verification in scientific communication. Proof assistants differ from general-purpose AI recommenders: their formal checking is tied to explicit propositions, definitions, axioms, and proof terms. The communication problem concerns how those bounded results are represented and connected to a target claim.

### 2.4 Lacan and Žižek: theoretical hypothesis, not established mechanism

Primary works to consult:
- Jacques Lacan, *The Seminar, Book XI: The Four Fundamental Concepts of Psychoanalysis* (1964), especially the sessions on transference and “the subject who is supposed to know.” A chapter titled “Of the Subject Who is Supposed to Know, of the First Dyad, and of the Good” appears in the published English edition.
- Jacques Lacan, “Proposition of 9 October 1967 on the Psychoanalyst of the School.”
- Jacques Lacan, *The Seminar, Book XVII: The Other Side of Psychoanalysis* (1969–70), for the discourse of the university and the relation between knowledge and authority.
- Slavoj Žižek, *The Sublime Object of Ideology* (1989).
- Slavoj Žižek, “The Interpassive Subject,” https://www.lacan.com/zizek-pompidou.htm.

**Conceptual caution:** The subject supposed to know is not simply a person or device that knows more, nor a synonym for trust in technology. It concerns a position attributed within the structure of transference. Interpassivity is a related but distinct concept and should not be substituted for it. A Lacanian reading can be advanced only as an interpretive hypothesis about the attribution of a knowing position; public text analysis alone cannot establish a psychological mechanism or diagnose individual authors/readers.

## 3. Initial formalization cases

### 3.1 Lean: quantum cryptography and BB84 (2026)

Maor Ben-Shahar, Jonathan Morag, Dirk Englund, and Kfir Sulimany, “Quantum Cryptography and Autoformalization in Lean,” arXiv:2610.17286 (2026). https://arxiv.org/abs/2610.17286

Primary source inspected: full text. Key materials:
- Abstract and introduction claim an end-to-end machine-verified composable finite-key security proof for entanglement-based qubit BB84 against coherent attacks.
- Theorem 1 states a finite-key composable security bound in diamond norm.
- Theorem 2 bounds abort probability for an honest memoryless channel.
- The protocol is encoded in a Lean language whose constructors enforce local operations and classical communication (LOCC).
- The paper explicitly distinguishes Lean kernel checking from human review of whether definitions and theorem statements match the intended physical protocol and security claim.
- It states that the model is finite-dimensional and describes further extensions required for prepare-and-measure protocols and optical QKD with decoy states.

**Provisional code:** scope-aware author presentation / valuable negative case. The authors explicitly separate kernel verification from semantic audit. The paper's broad phrase “end-to-end” is then narrowed by a detailed protocol definition, assumptions, and theorem statements. Do not code this as overclaim without a specific public statement that omits or contradicts these qualifications.

**Third-party coverage:** not yet collected. The author paper is a primary artifact, not independent coverage.

### 3.2 Isabelle/HOL: Schutz axioms for Minkowski spacetime (2022)

Richard Schmoetten, Jake E. Palmer, and Jacques D. Fleuriot, “Towards Formalising Schutz’ Axioms for Minkowski Spacetime in Isabelle/HOL,” *Journal of Automated Reasoning* 66 (2022), 953–988. DOI: https://doi.org/10.1007/s10817-022-09643-1

Primary article inspected in full. It mechanizes Schutz's axiomatic system and theorems about temporal order. The authors report that some results needed additional steps, alternative approaches, or corrections to Schutz's prose. Crucially, they state that they have not formalized a model of the theory, while expressing confidence in the formulation of their axioms of order and incidence.

**Provisional code:** scope-aware author presentation / negative case. The distinction between axiomatization, theorem verification, and model construction is explicit. The formalization is not presented as an empirical test of special relativity.

### 3.3 Coq: Robertson-type uncertainty relation (2015)

Takaaki Masuhara, Toru Kuriyama, Masakazu Yoshida, and Jun Cheng, “Formal Verification of Robertson-Type Uncertainty Relation,” *Journal of Quantum Information Science* 5 (2015), 58–70. DOI: https://doi.org/10.4236/jqis.2015.52008

Primary paper inspected. Its abstract says the relation is verified in Coq and frames the work as being “toward verifying unconditional security” of QKD. That wording may be a statement of motivation rather than a claim that the full protocol's security is established. The theorem statement, source code, conclusion, and any external retelling must be inspected before coding.

**Provisional code:** ambiguous / requires context. Do not infer substantive scope expansion from the abstract alone.

### 3.4 HOL Light + Isabelle: Flyspeck / Kepler conjecture (2017)

Thomas Hales et al., “A Formal Proof of the Kepler Conjecture,” *Forum of Mathematics, Pi* (2017). DOI: https://doi.org/10.1017/fmp.2017.1

The published paper is the official account of the completed Flyspeck project and describes a formal proof of the Kepler conjecture using HOL Light and Isabelle. The project formalized both traditional text-based proof components and computational parts of the proof.

**Provisional code:** scope-preserving mathematical benchmark. It concerns a mathematical theorem, not an empirical claim about physical sphere packings in nature. Independent communication sources should be compared against the exact theorem.

### 3.5 Lean: Liquid Tensor Experiment (2020–2022)

Peter Scholze, “Liquid Tensor Experiment,” *Experimental Mathematics* 31(2) (2022), 349–354. DOI: https://doi.org/10.1080/10586458.2021.1926016.

Primary public sources:
- Formal blueprint: https://leanprover-community.github.io/liquid/sect0001.html
- Completion announcement: https://leanprover-community.github.io/blog/posts/lte-final/
- Scholze's retrospective guest post: https://xenaproject.wordpress.com/2021/06/05/half-a-year-of-the-liquid-tensor-experiment-amazing-developments/
- Follow-up explanation of the theorem's structure: https://xenaproject.wordpress.com/2022/09/12/beyond-the-liquid-tensor-experiment/

The challenge concerned a precise theorem about Ext groups of condensed real vector spaces, not the wholesale verification of condensed mathematics. The Lean blueprint gives the theorem statement and links to the formal code. The Lean community's completion post says the main theorem of liquid vector spaces was formally verified on 14 July 2022. Scholze's 2021 post explicitly described the then-achieved milestone as verification of the part of the argument he was unsure about, while the later completion post marks completion of the full challenge.

**Independent retelling located:** Kevin Hartnett, “Proof Assistant Makes Jump to Big-League Math,” *Quanta Magazine*, 28 July 2021: https://www.quantamagazine.org/lean-computer-program-confirms-peter-scholze-proof-20210728/. This is a promising source for close comparison with the primary project record. The headline says “confirms Peter Scholze proof”; the article must be read in full and compared with the exact scope of the June 2021 milestone, not the later July 2022 completion.

**Provisional code:** potentially ambiguous compression at the headline level, but no final classification yet. The headline's “confirms” may be journalistic shorthand for a specified portion of the proof; article body and date-specific project state must decide the code.

### 3.6 Lean: Ax-Prover (2025/2026)

“Ax-Prover: A Deep Reasoning Agentic Framework for Theorem Proving in Mathematics and Quantum Physics,” published in *Machine Learning: Science and Technology* 7 (2026), DOI: https://doi.org/10.1088/2632-2153/ae9452; preprint: https://arxiv.org/abs/2510.12787.

This is a current case in which an LLM-based agentic workflow uses Lean to formalize and check results in mathematics and quantum cryptography. It reports a human-in-the-loop use case in which formalization exposed a gap in an informal cryptography argument, and a separate case formalizing an entropy bound in the Lo–Chau framework.

**Provisional code:** candidate for studying the attribution of epistemic authority across LLM, domain expert, and Lean kernel. It is not itself a clean “machine alone” case. The article's own distinctions between generation, proof checking, and domain-expert guidance must be preserved. Independent public retellings remain to be collected.

## 4. First public-text comparison

The Liquid Tensor Experiment currently offers the strongest three-layer pilot:
1. Formal artifact: the Lean blueprint with an exact theorem statement and code links.
2. Project-authored communication: Scholze's Xena posts and the Lean community completion announcement.
3. Independent retelling: Quanta Magazine's 28 July 2021 article.

A critical temporal distinction is necessary. The Quanta article was published in July 2021, when the project had verified the part of the proof Scholze had singled out as uncertain; the full experiment was completed in July 2022. Comparing the 2021 headline to the 2022 completion announcement without respecting this timeline would create a false scope mismatch.

This case can reveal whether the headline's “confirms” accurately compresses the 2021 milestone in the context of the article body, or whether it invites readers to infer that the entire theorem/proof was already formally verified. No conclusion is assigned until the full article and exact dated project statements are coded side by side.

## 5. Coding scheme and stopping rule

Use four primary codes:
- **Accurate:** explicit claim supported by the formal artifact and does not imply a broader target.
- **Reasonable compression:** details omitted but intended scope preserved by context or qualification.
- **Ambiguous:** materially different readings remain possible or relevant evidence is missing.
- **Substantive scope expansion:** claim exceeds what the formal artifact and linked semantic bridge establish; specify the missing inferential link.

For every record, code the target level separately:
1. local formal deduction;
2. record translation/interoperability;
3. correspondence to source mathematics/physics;
4. model/protocol instantiation;
5. empirical/physical target;
6. public verdict that the scientific question is settled.

Stop or narrow the thesis if the pilot contains only accurate shorthand or cannot reliably distinguish expansion from ambiguity. Do not infer belief, motive, or Lacanian transference from public text alone.

## 6. Stage status

**Completed in this pass:**
- Identified the key social-epistemology and science-communication literatures.
- Located the primary sources for five formalization projects across Lean, Coq, Isabelle, and HOL Light.
- Read the full primary paper for the Isabelle/Minkowski case, Coq/Robertson case, and the 2026 BB84 Lean paper.
- Located a promising independent Quanta retelling of the Liquid Tensor Experiment.
- Established a provisional codebook and recorded cases in the evidence register.

**Still required for acceptance of the literature/case stage:**
- Read the full Quanta article and pair each relevant statement with the date-specific Liquid Tensor project status.
- Locate and code at least one independent retelling for a second project.
- Inspect the exact formal theorem and conclusion/code for the Coq/Robertson paper before assigning a final category.
- Read the original Lacan passages directly in the published Seminar XI and 1967 Proposition; distinguish the concept from Žižek's later uses.
- Verify bibliographic details and add page/section locators for all cited theoretical sources.

No claim is made that the public-text study has already demonstrated systematic scope expansion.
