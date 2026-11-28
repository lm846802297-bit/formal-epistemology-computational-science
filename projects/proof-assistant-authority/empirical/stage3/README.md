# Stage 3 — Public Recognition and Downstream Knowledge Reuse

**Project:** *In Lean We Trust?*  
**Status:** Open; research initiated 2026-11-28  
**Branch:** `research/stage3-recognition-reuse`  
**Parent:** Stage 2 accepted dossier commit `5232f13feb215320c876f8f9cc79e6741beb44a8`  
**Tracking issue:** [#8](https://github.com/lm846802297-bit/philosophy-papers/issues/8)

## 1. Purpose

This stage examines how the four existing cases are recognized in public, mathematical and institutional settings, and whether their results, formal artifacts, methods or infrastructure are subsequently cited, reused, extended, replayed or contested.

Stage 1 (GitHub collaboration archive) and Stage 2 (AlphaProof/LTE synthesis) are frozen inputs. They are not to be recollected wholesale. Corrections require a specific error or new evidence and must be recorded as linked amendments.

## 2. Fixed case set

1. **Riemann Hypothesis (2026 Lean archive).**
2. **Navier–Stokes (OpenAI, 2026).**
3. **AlphaProof Nexus / Erdős problems.**
4. **Liquid Tensor Experiment.**

Waring's problem remains outside this four-case study. It is not a fifth case.

## 3. Questions

- How do mathematical, institutional, media and platform settings describe and recognize each result?
- How are solver, author, formalizer, validator, maintainer, auditor and expositor positions attributed?
- Which later works cite, import, extend, reproduce, criticize or otherwise reuse the relevant artifacts and results?
- Does semantic auditability remain operative in downstream use, or is it compressed into a portable credential or status?
- What evidence shows that actors preserve distinctions among kernel validity, statement correspondence, mathematical significance and provenance?

## 4. Evidence classes

Use separate codes for:
- **REC** — public or institutional recognition (certification, publication, status assignment, award, formal announcement).
- **CIT** — citation or explicit mention, without assuming uptake.
- **METH** — methodological uptake (adoption of workflow, formalization strategy, review procedure or proof-search method).
- **ART** — direct reuse of code, declarations, proof terms, Blueprint, dataset or other formal artifact.
- **DEP** — mathematical or formal dependency on a result or declaration.
- **REP** — independent replay, replication or verification.
- **CRI** — critique, correction, challenge or withdrawal.
- **REACH** — media/platform circulation or attention, not equivalent to epistemic adoption.

### Reuse strength

- **R0 — mention only:** no evidence of substantive use.
- **R1 — citation/contextual use:** cited or discussed, but no demonstrated dependence or adoption.
- **R2 — methodological uptake:** explicit use of a method or workflow.
- **R3 — artifact reuse:** exact code, formal declaration, data or proof component imported, forked or adapted.
- **R4 — result dependence:** later argument or theorem demonstrably depends on the result.
- **R5 — independent replay/replication:** independent reproduction of the relevant technical result; record separately from R2–R4 because replication may or may not imply downstream adoption.

A source may receive multiple codes. Record what was reused and at what level. An imported library dependency is not automatically substantive use of the case's target theorem.

## 5. Recognition is not a single variable

Distinguish:
- technical acceptance (e.g. kernel replay);
- semantic adjudication (whether the formal statement matches the intended target);
- mathematical recognition (expert discussion, citation, extension, incorporation);
- institutional recognition (journal, register, professional body, project announcement);
- public/media recognition (headlines, social discussion, public interpretation);
- attribution (who is represented as solver, author, validator, formalizer or contributor).

Do not rank cases on a single trustworthiness or popularity scale.

## 6. Search and provenance protocol

For every record retain:
- stable evidence ID and case;
- canonical URL and source title;
- author/institution;
- publication/event date and access date;
- immutable version, DOI, commit, PR, issue, release or exact locator;
- evidence class and reuse strength;
- short excerpt or factual event description;
- supported claim and counter-evidence;
- confidence and inference limit;
- raw-file SHA-256 only if the raw artifact was actually downloaded and archived.

Git blob SHA and SHA-256 are different identifiers; store them in separate fields. Never invent hashes. Preserve dated snapshots when web pages or registers can change.

### Search boundary

The initial search covers public scholarly records, official project/institutional statements, versioned repositories, independent technical assessments, citation/dependency records and purposively selected public discussion available by the cut-off date. It is not a representative survey of public opinion. Search queries, databases, date windows and result-screening decisions must be logged. A negative search result means “not located within this search boundary”, not “does not exist”.

## 7. Theoretical openness

No theorist is privileged in advance. Marx, Lacan, Žižek, Derrida, Byung-Chul Han, Bourdieu, Merton, STS, social epistemology, science communication and other relevant approaches are candidates. Theoretical concepts are entered in a separate candidate register with:
1. the observed phenomenon they may explain;
2. the explanatory mechanism;
3. the evidence required;
4. rival explanations;
5. relevant prior literature;
6. whether the concept is borrowed, adapted or genuinely proposed as new.

No theoretical chapter or manuscript text is modified during Stage 3. Empirical findings must not be coded to fit a preferred theory.

## 8. Initial literature leads (not exhaustive)

- Mathlib Community (2020), *The Lean Mathematical Library*, DOI: [10.1145/3372885.3373824](https://doi.org/10.1145/3372885.3373824): community organization and library development.
- Li et al. (2026), *The Network Structure of Mathlib*, arXiv:2604.24797: dependency networks at declaration/module level. This provides a method lead, not evidence that the four case artifacts were reused.
- Kurgan et al. (2026), *TheoremGraph: Bridging Formal and Informal Mathematics*, arXiv:2606.25363: cross-formality statement dependency and retrieval. This is a preprint and must be checked against current version and method.
- Druskat (2019), *Software and Dependencies in Research Citation Graphs*, DOI: [10.1109/mcse.2019.2952840](https://doi.org/10.1109/mcse.2019.2952840): software/dependency credit and citation graphs.
- FORCE11 Software Citation Principles (Smith et al. 2016), DOI: [10.7717/peerj-cs.86](https://doi.org/10.7717/peerj-cs.86): software identity, attribution, persistence and specificity.
- Desrochers et al. (2018), *Authorship, citations, acknowledgments and visibility in social media*, DOI: [10.1177/0539018417752089](https://doi.org/10.1177/0539018417752089): scientific reward and symbolic capital.
- Tahamtan & Bornmann (2022), *The Social Systems Citation Theory*, DOI: [10.3145/epi.2022.jul.11](https://doi.org/10.3145/epi.2022.jul.11): citation as both recognition and persuasion.
- Chevitarese (2023), *Infocracia e Psicopolítica em Byung-Chul Han*, DOI: [10.32334/oqnfp.2023n53a972](https://doi.org/10.32334/oqnfp.2023n53a972): a possible source for digital visibility and subjectivation; relevance to mathematical proof recognition remains to be demonstrated.
- Glavaš (2021), *Deconstruction and the Archival Revolution*, DOI: [10.14746/pss.2020.19.2](https://doi.org/10.14746/pss.2020.19.2): reception of Derrida's *Archive Fever* in new-media studies; use only if archival selection, preservation and access emerge as explanatory mechanisms.

The literature review must also examine direct antecedents and the already identified novelty risks in the Stage 2 source register before any originality claim is made.

## 9. Deliverables

- This protocol and a dated collection log.
- Expanded, source-pinned four-case source register.
- Machine-readable evidence ledger.
- Four case-level recognition/reuse reports.
- Unified comparison report.
- Stage 3 acceptance record.

## 10. Acceptance criteria

Stage 3 closes when:
1. Each case has a stated search boundary and dated source inventory.
2. Recognition, citation, reuse, replication and critique are coded separately.
3. Every direct reuse claim has a traceable artifact/dependency or explicit downstream-use statement.
4. Every interpretive claim includes supporting evidence, counter-evidence and an inference limit.
5. Raw artifacts and provenance are archived to the stated standard.
6. Stage 1/2 records remain unchanged except for linked, evidence-based corrections.
7. No manuscript or theory-chapter edits occur; PR #6 and PR #7 remain unchanged.

**Initial cut-off:** 2026-11-28. Subsequent observations must be dated and added as a new snapshot rather than silently rewriting the historical record.
