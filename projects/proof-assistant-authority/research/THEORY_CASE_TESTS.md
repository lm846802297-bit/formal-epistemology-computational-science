# Testing the Žižekian model against the four Lean cases

**Project:** *In Lean We Trust?*  
**Cut-off:** 27 November 2026  
**Status:** revised case-testing document. The model is defined in THEORETICAL_MODEL.md. Findings are source-bounded and provisional; no case is presumed ideological.

## 1. Common unit of analysis

The unit is a dated public or institutional claim invoking Lean verification as part of the warrant for a mathematical result, paired with the exact formal artifact, intended claim, specification relation, source context, and subsequent responses.

For each case, record:
1. exact formal proposition and proof artifact;
2. environment, axioms, dependencies, and checking status;
3. intended mathematical claim and specification relation;
4. human, technical, and institutional mediation;
5. exact public/institutional wording and its genre;
6. counter-evidence, correction, and rival explanations;
7. any documented institutional or practical effect.

The article does not claim to rebuild every repository or independently adjudicate the mathematics. Source-level inspection, reported independent checking, and mathematical adjudication are kept separate.

## 2. Diagnostic requirements

Technical warrant is the baseline, not an indicator of ideology. A strong diagnosis requires all three:

- **S — Scope extension:** the credential is made to warrant more than the formal proposition and documented specification relation establish.
- **O — Objectal displacement:** the credential appears to contain autonomous authority while the relations that make it meaningful are displaced.
- **E — Social efficacy:** the representation plays a documented role in legitimation, recognition, credibility allocation, institutional action, or repeated practice.

The formation mechanism has five analytical moments: real technical reliability; distributed epistemic labour; credential condensation; objectal displacement and symbolic authority; and fetishistic disavowal as a mechanism of reproduction. The first four explain how the credential acquires authority; the fifth explains how that authority can persist after its limits are known. The case tests distinguish these moments and assess S, O, and E separately.

## 3. Riemann hypothesis — formal certification, institutional authorization, contested meaning

### Technical and institutional record
- Levent Alpöge released a note and Lean archive on 20 November 2026.
- The 21 November Lean FRO/Mathlib joint statement expressed full confidence and said that both the statement and proof were certified. It reported expert vetting of the Mathlib statement, successful compilation, independent statement comparison, and acceptance by Lean’s kernel and independent checkers.
- Andrew Sutherland’s report records 175,187 compiling modules, five headline theorems using only propext, Classical.choice, and Quot.sound, kernel replay, independent checkers, and statement comparison.
- A shorter rewrite published on 25 November is a distinct artifact with its own verification report.
- The rh-lean-roadmap project published a 497-page main exposition, 963 pages of longer proofs, and a 122-page index on 26 November. The documentation states that several AI models generated the exposition from the Lean source and cross-checked it.
- Parker Emmerson posted a non-peer-reviewed preprint on 24 November arguing that the certified derivation does not prove RH in several senses. It grants the derivation and reported checks but disputes the interpretation of what follows from them. This article does not adjudicate that argument.

### Fantasy test
The combination of a very large formal archive, independent checks, an institutional statement of “full confidence,” and a substantial exposition can stage a scene of closure around a historically difficult problem.

**Counter-evidence:** the joint statement identifies expert vetting and independent comparison; the exposition discloses its AI-mediated provenance; further mathematical explanation is explicitly anticipated; a public foundational challenge contests the meaning of the certification.

**Assessment:** the case reveals layered and contested authorization. The available evidence does not establish that the credential is treated as an autonomous guarantee beyond the stated warrant.

### Fetishism test
Compressed accounts may attribute the achievement to “AI + Lean,” but the primary institutional record names expert vetting, multiple checkers, Mathlib, and community work.

**Assessment:** objectal displacement is not established. This case is more useful for studying how machine checking and institutional authorization combine, and how that authorization remains open to dispute.

### Fetishistic disavowal test
The public record documents technical qualifications and the independent-checking basis, but does not show the same institutional communication chain acknowledging the precise scope and continuing to mobilize the credential as a broader guarantee. The Emmerson preprint is a public foundational challenge, not evidence of fetishistic disavowal by the certifying institutions.

**Role:** layered institutional authorization and contested meaning of a formal certificate.

## 4. Navier–Stokes — kernel validity and the natural-language proof

### Technical and semantic record
- OpenAI’s 8 September 2026 announcement states that its system produced an analytical proof and a Lean formalization of finite-time singularity formation for a three-dimensional incompressible fluid with smooth external forcing and finite energy. It claims to establish statements C and D of the official Millennium Prize formulation.
- Bastounis, Circelli, and Hansen (arXiv:2610.08144) distinguish compiling a Lean proof of a formal statement from semantically faithful translation of a natural-language mathematical text.
- They identify an inverse-estimate discrepancy: the written proof uses m+4 input derivatives, while the corresponding Lean declaration requires m+5. They also identify a difference in the pressure-flux estimate and proof route.
- These are mismatches between the written proof and the formal artifact. They do not establish a kernel failure or prove the underlying PDE theorem false. The critique explicitly does not adjudicate the correctness of the natural-language proof.

### Fantasy test
The announcement presents a major mathematical result together with a Lean formalization. This can invite a reading in which the formal credential closes the entire question.

**Counter-evidence:** OpenAI says it is sharing both a write-up and a formalization; it does not explicitly say that Lean alone verifies every step of the natural-language paper. The independent critique makes the specification issue public.

**Assessment:** strongest candidate for scope extension, but the exact public inference must not be overstated.

### Fetishism test
The mismatch shows that a valid proof of a formal declaration cannot by itself certify faithful translation of the separate written argument. However, the available public wording does not yet demonstrate that the credential was treated as an autonomous source of authority independently of the analytical proof and other review.

**Assessment:** objectal displacement remains a candidate, not an established finding.

### Social efficacy and fetishistic disavowal
The announcement has public significance. The current source record identifies the public credential and the subsequent specification critique, but does not establish that the same actor or institutional chain acknowledged the precise mismatch and continued to mobilize Lean verification as a broader guarantee. The fifth moment is therefore a question for the communication history, not an inference from the mismatch alone.

**Role:** principal case for testing the gap between formal validity and specification fidelity.

## 5. Erdős problems — AlphaProof Nexus, human validation, and artifact provenance

### Technical and institutional record
- Tsoukalas et al. report nine solutions among 353 formalized Erdős problems and 44 proofs among 492 OEIS conjectures attempted.
- The *Science* paper states that experts validated the correspondence between the nine solved Lean statements and the original conjectures. It also reports that the system detected and prompted correction of density misformalizations.
- A source-level audit found several link/provenance issues:
  - **#26:** the top-level linked Lean target differs from the upper-density theorem in the prose, but an auxiliary pointwise lemma in the same file is strong enough to establish the prose result.
  - **#741(i):** the linked file proves an exact-density counterexample; the upper-density theorem exists separately in Formal Conjectures.
  - **#741(ii):** the cited link points to a file for Problem 12 rather than Problem 741.
  - **#125:** the linked file proves the relevant lower-density variant but differs from the file first posted in the original forum discussion.
- These findings concern linked artifact identity and provenance, not kernel failure or invalidity of all reported results.

### Fantasy test
“AI solves Erdős problems” can compress the human-AI workflow and the scope of the benchmark.

**Counter-evidence:** the primary paper reports denominators, formalized targets, Lean checking, and expert statement validation. It also acknowledges corrections to misformalizations.

**Assessment:** limited and context-dependent.

### Fetishism test
The source audit demonstrates that a published credential still requires traceability from prose claim to exact formal artifact. However, the publication itself makes human validation visible, and the audit does not establish that the credential was treated as autonomous authority.

**Assessment:** mixed case; objectal displacement and social efficacy are not established.

### Fetishistic disavowal test
The paper reports human statement validation, while the artifact audit identifies link and provenance issues. The available record does not establish that the same authors or institution acknowledged those specific issues and nevertheless continued to use the Lean credential as a broader guarantee.

**Role:** statement identity, provenance, and human validation.

## 6. Liquid Tensor Experiment — semantic scrutiny as counter-case

The 15 July 2022 completion announcement states the main theorem and lists mathematical, formalization, technical, library, and institutional contributors. Adam Topaz’s 14 October 2022 discussion explicitly asks how mathematicians can be confident that the definitions introduced in Lean are correct. It describes the possibility of pathological definitions and the creation of a readable examples folder as sanity checks for mathematicians with limited Lean experience. Scholze’s contemporaneous account also emphasizes mathematical interaction and scrutiny.

**Fantasy test:** a headline may present the completion as technical closure, but the primary project record preserves the human and semantic work.

**Fetishism test:** this is strong counter-evidence. The validity of definitions is made an explicit object of public scrutiny rather than being attributed to the machine alone.

**Social efficacy and reproduction:** the public record documents collective review and semantic sanity checks. This visible mediation interrupts the move from credential condensation to autonomous objectal authority; the project presents the formal result through the practices that sustain its meaning.

**Role:** counter-case showing how a formal verification credential can remain embedded in visible collective and semantic practice.

## 7. Comparative result

| Case | Scope extension | Objectal displacement | Social efficacy | Overall role |
|---|---|---|---|---|
| Riemann | Contested/unclear | Not established | Institutional certification documented, but not as autonomous machine guarantee | Layered authorization |
| Navier–Stokes | Strongest candidate | Candidate only | Public announcement documented; credential-specific effect uncertain | Formal validity vs specification fidelity |
| Erdős / AlphaProof | Limited and context-dependent | Not established | Publication and validation documented; no autonomous credential effect established | Provenance and human validation |
| Liquid Tensor | Weak | Counter-evidence strong | Collective semantic review documented | Counter-case |

No case currently satisfies S ∧ O ∧ E. The empirical contribution is a differentiated diagnostic comparison, not a claim that Lean is generally fetishized.

## 8. Inference limits

1. A discrepancy between a formal artifact and a natural-language proof is not a kernel failure.
2. The Navier–Stokes discrepancies do not prove the PDE theorem false.
3. The AlphaProof provenance issues do not invalidate all reported results.
4. The Emmerson preprint is non-peer-reviewed and its mathematical/logical argument is not adjudicated here.
5. Public texts establish representations and documented practices, not population-level belief or unconscious motive.
6. A case is not diagnosed as fetishism unless scope extension, objectal displacement, and social efficacy are separately supported.
