# Testing the Žižekian model against the four Lean cases

**Project:** *In Lean We Trust? The Ideology of Machine-Checked Proofs in Science*  
**Date:** 27 November 2026  
**Status:** operational case-testing document. The theoretical model is defined in THEORETICAL_MODEL.md. Case findings are provisional and source-bounded; this is not a mathematical referee report or a representative survey of public opinion.

## 1. Common test protocol

Each case is assessed against the same evidence chain:

1. **Technical object:** exact formal proposition, proof artifact, definitions, assumptions, environment, and kernel/checker status.
2. **Semantic bridge:** relation between the formal proposition and the intended theorem or scientific claim.
3. **Collective mediation:** theorem selection, mathematical formulation, formalization, library/toolchain work, expert scrutiny, and institutional assessment.
4. **Discursive plane:** exact statements by the researchers, institutions, journals, and media; preserve date, speaker, genre, and surrounding qualification.
5. **Material-institutional plane:** how the Lean artifact is reviewed, certified, cited, published, or used in institutional decisions.
6. **Spontaneous-practical plane:** whether a broader reliance on the Lean credential is reproduced as a routine practice. Do not infer this from one announcement.
7. **Counter-evidence and rival explanations:** accurate shorthand, transparent qualification, visible human contribution, independent review, institutional reputation, and ordinary genre conventions.

The five epistemic levels—derivational validity, semantic correspondence, mathematical understanding, significance, and institutional/public recognition—must remain separate.

## 2. How the Žižekian mechanisms are coded

| Mechanism | Case-level question | Positive evidence | Counter-evidence |
|---|---|---|---|
| Ideological fantasy | Is a bounded check staged as closure of wider uncertainty? | Recurrent language or practice treating “verified” as a final settlement beyond the formal target | Explicit scope statements and a clear distinction between formal checking and broader acceptance |
| Fetishistic displacement | Does the machine appear to possess authority independently of the relations that make the check meaningful? | Collective mathematical, semantic, technical, or institutional mediation recedes while autonomous machine authority is foregrounded | Contributors, dependencies, semantic review, and institutional responsibilities remain visible |
| Disavowal | Does investment in a broader guarantee persist after the relevant limit is acknowledged? | Same actor/institution acknowledges the precise limit and continues a connected practice that exceeds it | Correction, scope-preserving qualification, no continued overreach, or no actor-level connection |

Disavowal is an additional test, not a required condition for every case of fetishism. “Cynical disavowal” requires stronger evidence of a manipulative distance between acknowledged knowledge and practice. Public wording alone does not reveal unconscious motives.

## 3. Riemann hypothesis — Claude-assisted Lean development

### Technical and institutional record
- Levent Alpöge's 20 November 2026 note presents the result as a proof he believes he discovered while working with Claude and releases a Lean development.
- The original archive and compact rewrite have extensive reported compilation, kernel replay, independent checker runs, and statement comparison with Mathlib.
- The Lean FRO/Mathlib and Waterloo materials describe the formal statement, checking process, and contributors.
- The 26 November source audit records the existence of a 1,582-page AI-mediated exposition (497-page main text, 963-page appendix, 122-page index), written by several AI models from Lean source and cross-checked. It is therefore inaccurate to describe the case as having no readable exposition.
- Expert understanding, independent mathematical assessment, conventional publication, and Clay recognition remain analytically distinct from kernel acceptance and statement comparison.

### Fantasy test
**Evidence in favour:** the combination of a historically unresolved problem, an enormous formal archive, multiple independent checker results, and headlines such as “AI solves the Riemann hypothesis” can stage a visible scene of mathematical closure.

**Counter-evidence:** the author's own wording is qualified; expert and institutional accounts distinguish formal certification, statement identity, human mathematical understanding, and community acceptance. The later exposition also changes the earlier picture of the case as lacking a readable account.

**Assessment:** plausible but qualified. The case tests how strong local certification and AI-mediated exposition can symbolize broader certainty without automatically settling every level of mathematical understanding and recognition.

### Fetishism test
**Evidence in favour:** compressed “Claude + Lean” narratives can background the mathematician's direction, formalizers, Mathlib, kernel/checker developers, and independent human assessment.

**Counter-evidence:** the detailed Waterloo and Lean community records make much of the technical and human network visible; the exposition and independent verification work add further mediation rather than simply erasing it.

**Assessment:** mixed. Fetishistic displacement is possible in selected compressed accounts, but it is not established as the dominant representation of the case.

### Disavowal test
No strict cynical or fetishistic disavowal is established by the current record. Explicit qualifications and the availability of detailed technical accounts complicate such a diagnosis.

**Role in the model:** ambivalent case for the coexistence of strong formal certainty, expert authorization, AI-mediated exposition, and continuing questions about the scope of scientific recognition.

## 4. Navier–Stokes — OpenAI discovery and Lean formalization

### Technical and semantic record
- OpenAI's 8 September 2026 announcement presents an analytical proof claim for a finite-time singularity result for three-dimensional incompressible Navier–Stokes with smooth forcing and describes a Lean formalization.
- The Lean kernel can check the proof terms for the exact formal declarations in the repository.
- Bastounis, Circelli, and Hansen (arXiv:2610.08144) report discrepancies between the natural-language paper and the Lean formalization, including the derivative count in the inverse estimate of Lemma 8.6 (m+4 in the written proof versus m+5 in the Lean declaration) and a difference in the pressure-flux estimate/proof route.
- These discrepancies concern correspondence between the formal artifact and the separate natural-language proof. They do not establish a Lean kernel failure or prove the underlying Navier–Stokes result false.
- The independent critique and subsequent public responses make the correspondence question visible and contested.

### Fantasy test
**Evidence in favour:** an announcement of a solution to a Millennium Prize problem alongside Lean verification can be interpreted as a machine-certified settlement of the full scientific claim.

**Counter-evidence:** the later critique and public responses distinguish the formal declarations from the written proof. The record contains an explicit dispute about the scope of the guarantee, not a settled demonstration that the mathematical community accepts Lean as the final arbiter.

**Assessment:** strongest candidate for an enlarged fantasy of verification. The exact inferential gap is between kernel acceptance of formal declarations and the claim that the separate written proof has been faithfully represented.

### Fetishism test
**Evidence in favour:** the genuine authority of the kernel over the formal declarations may be allowed to stand in for the semantic relation between those declarations and the paper. The machine credential can thereby appear to guarantee a broader object than it checks.

**Counter-evidence:** the repository, independent critique, and public response make the mismatch contestable. The semantic mediation is not wholly hidden.

**Assessment:** strongest candidate for fetishistic displacement at the level of public representation, but the final diagnosis depends on a matched analysis of the original announcement, its qualifications, and the subsequent correction/response chain.

### Disavowal test
The acknowledged mismatch creates a possible test of persistence. The present record does not establish cynical intent. A stronger fetishistic-disavowal claim requires evidence that the same actor or institutional communication chain acknowledges the precise limit and nevertheless continues to rely on the Lean credential as a broader guarantee.

**Role in the model:** principal case for testing the difference between local formal warrant and a broader scientific claim.

## 5. Erdős problems — AlphaProof Nexus

### Technical and institutional record
- Tsoukalas et al. report 9 solutions among 353 open Erdős problems represented in the formal conjecture repository and 44 proofs among 492 OEIS conjectures attempted. These denominators describe the benchmark represented and attempted, not all open Erdős problems.
- The Science paper describes Lean-based proof search and reports human validation of the correspondence between the nine formal Erdős statements and the intended conjectures.
- The project audit identifies artifact/prose provenance issues that must not be exaggerated:
  - **#26:** the top-level Lean target is a lower-density Tenenbaum variant rather than the prose upper-density theorem, but the same file contains a uniform pointwise lemma strong enough to establish the prose upper-density result.
  - **#741(i):** the linked AlphaProof file proves an exact-density counterexample; the upper-density theorem exists separately in Formal Conjectures.
  - **#741(ii):** the cited arXiv v2 link points to a file for Problem 12, while the appropriate #741(ii) proof is located elsewhere.
- These are target-identity, citation, and provenance issues. They do not establish that all reported results are invalid or that Lean's kernel failed.

### Fantasy test
**Evidence in favour:** headlines such as “AI solves Erdős problems” can imply autonomous discovery or general mathematical capability beyond the formalized benchmark.

**Counter-evidence:** the primary paper gives denominators, describes the formal conjecture corpus, and reports human statement validation. These disclosures preserve important scope conditions.

**Assessment:** limited and context-dependent. The case tests whether media compression removes the boundaries retained by the technical paper.

### Fetishism test
**Evidence in favour:** a simplified account that credits only AlphaProof Nexus can background formal conjecture curation, Lean, statement validation, and expert review.

**Counter-evidence:** the Science paper makes the human-AI workflow and validation visible. The source-level audit also makes provenance questions explicit and demonstrates that the credential remains open to scrutiny.

**Assessment:** weak-to-mixed. The case is more useful as a test of transparent mediation than as a clear example of autonomous machine authority.

### Disavowal test
No cynical or fetishistic disavowal is established. The existence of artifact-link errors does not by itself show that an actor knowingly maintained an enlarged guarantee.

**Role in the model:** mixed case and counter-test for whether explicit human validation and artifact provenance constrain symbolic overreach.

## 6. Liquid Tensor Experiment — historical Lean case

### Technical and institutional record
- The Lean community announced completion of the formal verification of the main theorem of liquid vector spaces in July 2022.
- The project record identifies a broad mathematical and formalization network, including contributors and Mathlib dependencies.
- Scholze's contemporaneous account emphasizes human mathematical interaction and scrutiny as central to his confidence.
- Adam Topaz's 2022 discussion explicitly addresses the correctness of formal definitions and documents readable sanity-check examples.

### Fantasy test
**Evidence in favour:** headlines saying Lean “confirmed” or “verified” the result can stage technical closure.

**Counter-evidence:** the primary project record names contributors, and Scholze's account makes human mathematical scrutiny visible.

**Assessment:** weak. The case does not support a strong claim that the machine credential replaces the broader mathematical process.

### Fetishism test
**Evidence in favour:** a headline that attributes confirmation to Lean can background the collective project.

**Counter-evidence:** the official record and subsequent explanation make collective labour, definition checks, and expert judgement visible.

**Assessment:** weak. This is the strongest counter-case to the claim that formal verification is inherently fetishistic.

### Disavowal test
No evidence of disavowal is established. The primary accounts preserve the human and semantic conditions of the formal result.

**Role in the model:** counter-case showing that formal verification can be integrated into a visible collective epistemic practice rather than represented as an autonomous machine guarantee.

## 7. Cross-case synthesis

| Case | Fantasy of closure | Fetishistic displacement | Disavowal | Main function |
|---|---|---|---|---|
| Riemann | Plausible, qualified | Possible in compressed accounts; countered by detailed records | Not established | Ambivalent case: high formal certainty and layered recognition |
| Navier–Stokes | Strongest candidate | Strongest candidate | Not established; persistence remains to be tested | Formal validity versus semantic correspondence |
| Erdős / AlphaProof | Limited and context-dependent | Weak-to-mixed | Not established | Transparent mediation and artifact-provenance test |
| Liquid Tensor | Weak | Weak | Not established | Counter-case: visible collective labour and semantic scrutiny |

## 8. What the four cases establish—and do not establish

The cases support a differentiated thesis:
- Lean can function as a symbolic credential of mathematical reliability.
- The strongest candidate for a broader guarantee is the Navier–Stokes announcement/formalization dispute.
- Riemann demonstrates the coexistence of very strong formal certification with other dimensions of understanding and recognition.
- Erdős demonstrates the importance of statement identity, provenance, and visible human validation.
- Liquid Tensor demonstrates that formal verification can be embedded in transparent collective practice.

The cases do **not** establish:
- that all uses of Lean are ideological;
- that the general public uniformly treats Lean as a final guarantor;
- that any named researcher has a cynical motive;
- that a single headline proves fetishism;
- that a mismatch between a paper and a Lean declaration is a kernel failure or a refutation of the mathematical result.

## 9. Case-level acceptance criteria

A strong case-level diagnosis of the ideological fetishism of formal verification requires:
1. the exact Lean proposition and check are identified;
2. the broader claim attributed to the check is identified;
3. the missing semantic or inferential link is specified;
4. the collective and institutional relations are traced;
5. the representation of the machine as autonomous authority is demonstrated;
6. ordinary shorthand, context, corrections, and counter-evidence are considered.

A disavowal claim additionally requires explicit acknowledgement of the precise limit and continued investment in a broader guarantee within a traceable actor/institutional practice.

If these criteria are not met, the case is coded as warranted reliance, transparent mediation, ambiguity, or insufficient evidence—not as ideological fetishism.
