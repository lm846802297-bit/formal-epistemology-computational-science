# Empirical Research Dossier: In Lean We Trust?

Status: initial structured corpus; collection and coding in progress.
Branch: research/empirical-evidence-dossier.

## Purpose

This dossier builds an auditable empirical foundation for the philosophical analysis. It records observable practices, public representations, recognition events, attribution, reuse, and counter-evidence before theoretical interpretation. It does not assume that the cases confirm the Žižekian framework.

## Research questions

1. How are formal mathematical results produced through distributed human, computational, and institutional labour?
2. How are formal statements related to informal targets, and who performs semantic validation?
3. Through which public procedures do proof artifacts become recognized mathematical achievements?
4. How are solver, author, validator, formalizer, maintainer and reader positions assigned?
5. What is actually cited, reused, challenged or incorporated into later work?
6. Where do public practices preserve rather than displace distinctions between kernel validity, representational fidelity, significance and provenance?

## Four cases

| Case | Empirical focus |
|---|---|
| Riemann Hypothesis (2026 Lean archive) | Institutional certification, independent replay, statement review |
| Navier–Stokes (OpenAI, 2026) | Formal statement, natural-language proof, public solution claim and independent critique |
| AlphaProof Nexus / Erdős problems | Automated search, target correction, status registers and solver attribution |
| Liquid Tensor Experiment | Collaborative formalization, blueprint, semantic examples and negotiated attribution |

These are contrastive cases, not a statistically representative sample. Time-specific 2026 records must be versioned rather than silently overwritten.

## Files

- source-register.md: source inventory, evidence role, access status and collection priorities.
- coding-framework.md: common codebook and decision rules.
- theory-evidence-map.md: theoretical claims, supporting evidence, counter-evidence and inference limits.
- collection-log.md: dated research activity and unresolved retrieval tasks.

## Evidence hierarchy

1. Primary technical artifact: paper, source code, Lean declaration, build/replay record, versioned repository.
2. Primary institutional record: formal announcement, merged PR, official register, certification.
3. Participant account: public blog, talk, interview, retrospective.
4. Independent assessment: external audit, critique, replication, peer-reviewed analysis.
5. Reception and secondary discourse: news, community wiki, forum, citations and reuse.
6. Research interpretation: coding and philosophical inference.

No source category automatically proves claims in another. Kernel acceptance establishes derivational validity relative to a formal proposition and environment; it does not alone establish informal target correspondence, significance or authorship.

## Provenance rules

For each retained artifact record canonical URL, author/institution, event and access dates, immutable commit/DOI/version, exact locator, evidence type, claims supported, caveats and SHA-256 of the archived raw file. Git blob SHA is not SHA-256. Never invent a hash or infer one from a source identifier.

Code observable evidence before interpretation. Distinguish explicit statements, observed actions and researcher inferences. Use “not observed” rather than “absent” when the corpus has not been searched sufficiently. Record contradictions instead of silently reconciling them. Public statements do not provide transparent access to private belief.

## Method

Core method: documentary digital ethnography and comparative case study. Supporting methods: process tracing for status/correction events, repository trace analysis for labour and review, discourse analysis for public attribution, and citation/dependency analysis for reuse.

This is not interview-based ethnography: no interviews have been conducted. Interviews, if later pursued, require separate consent and ethics procedures.

## Current status

The first-pass GitHub collaboration survey is archived. The LTE PR census is complete for the 57 PRs returned by the repository search; RH uses the generated contributor snapshot plus a purposive PR/issue sample; Navier–Stokes has a two-commit repository history and no public PR/issues; AlphaProof's results archive is fully inventoried at six commits/four issues, with selected Formal Conjectures PRs sampled. Systematic reception and downstream reuse collection remain open.
