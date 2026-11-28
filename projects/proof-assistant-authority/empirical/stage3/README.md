# Stage 3 — Public Recognition and Downstream Knowledge Reuse

**Project:** In Lean We Trust?  
**Status:** **Accepted at documentary scope on 2026-11-28**  
**Branch:** research/stage3-recognition-reuse  
**Parent:** Stage 2 dossier commit 5232f13feb215320c876f8f9cc79e6741beb44a8  
**Tracking issue:** [#8](https://github.com/lm846802297-bit/philosophy-papers/issues/8)  
**Draft PR:** [#9](https://github.com/lm846802297-bit/philosophy-papers/pull/9)

## Purpose

This stage examines how the four existing cases are recognized in public, mathematical and institutional settings, and whether their results, formal artifacts, methods or infrastructure are subsequently cited, reused, extended, replayed or contested.

Stage 1 (GitHub collaboration archive) and Stage 2 (AlphaProof/LTE synthesis) are frozen inputs. They were not recollected wholesale. Corrections require a specific error or new evidence and must be recorded as linked amendments.

## Fixed case set

1. Riemann Hypothesis (2026 Lean archive)
2. Navier–Stokes (OpenAI, 2026)
3. AlphaProof Nexus / Erdős problems
4. Liquid Tensor Experiment

Waring's problem is outside this four-case stage.

## Research questions

- How do mathematical, institutional, media and platform settings describe and recognize each result?
- How are solver, author, formalizer, validator, maintainer, auditor and expositor positions attributed?
- Which later works cite, import, extend, reproduce, criticize or otherwise reuse the relevant artifacts and results?
- Does semantic auditability remain operative in downstream use, or is it compressed into a portable credential or status?
- What evidence shows that actors preserve distinctions among kernel validity, statement correspondence, mathematical significance and provenance?

## Evidence classes

The evidence ledger distinguishes:
- REC — public or institutional recognition;
- CIT — citation or explicit mention, without assuming uptake;
- METH — methodological uptake;
- ART — direct reuse of code, declarations, proof terms, Blueprint, dataset or other formal artifact;
- DEP — mathematical or formal dependency on a result or declaration;
- REP — independent replay, replication or verification;
- CRI — critique, correction, challenge or withdrawal;
- REACH — media/platform circulation;
- SEARCH — a bounded negative search result.

Reuse strength:
- R0 — mention or recognition only;
- R1 — citation/contextual use;
- R2 — methodological uptake;
- R3 — direct artifact reuse;
- R4 — result-level mathematical dependence;
- R5 — independent replay/replication.

A citation is not automatically reuse. A repository import is not automatically substantive mathematical dependence. Views, stars, downloads and media repetition are not evidence of epistemic adoption.

## Deliverables

- source-register.md — source inventory, immutable versions, blob SHAs and literature antecedents.
- evidence-ledger.csv — dated, coded evidence records with exact locators and inference limits.
- riemann-case-report.md
- navier-stokes-case-report.md
- alphaproof-case-report.md
- liquid-tensor-case-report.md
- case-comparison.md
- theory-candidate-register.md
- theory-synthesis.md
- stage3-acceptance.md
- manuscript-revision-plan.md

## Main empirical findings

1. **Recognition and reuse are independent.** High public recognition does not by itself imply theorem-level mathematical dependence.
2. **Riemann:** strong formal recognition and independent checking; the dominant afterlife is readable refactoring, reconstruction and collective mathematical scrutiny. No downstream theorem dependency was located.
3. **Navier–Stokes:** an early formal-artifact gap was corrected two days after the announcement; later paper-to-Lean proof-route discrepancies remain a distinct issue. The artifact has substantial technical reuse in benchmarking, porting, auditing and formal-library integration, but no downstream theorem dependence was located.
4. **AlphaProof:** the nine Erdős proof files are formally archived, but they represent seven unique problem numbers and include parts/variants. No direct downstream use of those nine results was located. A separate AlphaProof quantum-graph result was extended and translated into a human-authored quantum-optics preprint.
5. **Liquid Tensor:** direct reuse of the original Lean3 theorem/proof code was not located. Its semantic definition-checking strategy and Blueprint practice have explicit methodological uptake in later formalization work.

## Theoretical direction selected

Retain Marx–Lacan–Žižek as the core account of objectified labour, symbolic recognition and conditional warrant-scope transfer. Add Bourdieu/Merton for recognition and credit, Derrida for archival selection and repeatability, and Hardwig/STS as the rational-dependence and production baseline. Byung-Chul Han is not a core framework on current evidence.

A candidate middle-range model, **post-verification circulation**, distinguishes credentialization, translation, integration, assimilation and archival stabilization. Its novelty boundary is documented in theory-synthesis.md; no priority claim is made.

## Governance

Stage 3 is accepted at the stated documentary scope. This PR contains empirical research assets and theory selection only. It does not modify the manuscript or Stage 1/2 records. Manuscript revision is a separate next phase, beginning with the theoretical framework only.
