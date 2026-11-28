# Comparative Sociological Coding Framework

Version 0.1. Applies to RH, NS, APN and LTE.

## 1. Principles

- Code observable evidence before interpretation.
- Unit of analysis: dated and locatable artifact, utterance, review, status transition, correction or reuse event.
- Every code needs a source ID and locator.
- Use positive, negative, mixed or not observed. Not observed is not absent.
- A participant's public statement is evidence of their public account, not transparent access to private belief.
- Repository activity is not automatically mathematical recognition.
- Independent kernel replay is distinct from independent semantic adjudication.
- Do not collapse derivational validity, target correspondence, significance, credit and trust.

## 2. Evidence record schema

| Field | Definition |
|---|---|
| record_id | Stable identifier, e.g. AP-PR-3778-01 |
| case | RH, NS, APN or LTE |
| source_id | ID in source-register |
| source_version | DOI/version, commit SHA, PR number or archive release |
| event_date | Date of event |
| access_date | Date retrieved |
| locator | Section, line, comment ID, path or timestamp |
| actor_role | Author, mathematician, formalizer, agent, maintainer, institution, auditor or reader |
| evidence_type | Technical artifact, institutional record, participant account, independent assessment, reception or reuse |
| excerpt | Exact short excerpt or faithful event description |
| primary_code | Code below |
| polarity | Supports, contradicts, mixed or not observed |
| confidence | High, medium or low, with reason |
| research_memo | Interpretation separated from observation |
| raw_sha256 | Hash of retained raw artifact, if archived |
| follow_up | Specific retrieval task |

## 3. Codebook

### L — Labour and production

| Code | Name | Operational definition |
|---|---|---|
| L1 | Problem framing | Who selected, posed or refined the informal problem? |
| L2 | Formal specification | Who created or changed the Lean statement and definitions? |
| L3 | Proof production | Who or what generated proof strategy or proof term? |
| L4 | Semantic validation | Who assessed whether formal target expresses intended mathematics? |
| L5 | Infrastructure labour | Library, toolchain, CI, build, checker and repository work |
| L6 | Exposition | Who translated formal artifacts into human-readable explanation? |
| L7 | Review and correction | Who found, adjudicated and repaired errors? |

### S — Semantic and technical warrant

| Code | Name | Operational definition |
|---|---|---|
| S1 | Kernel validity | Proof term accepted in a stated formal environment |
| S2 | Environment provenance | Axioms, imports, toolchain and dependencies specified |
| S3 | Statement correspondence | Explicit comparison of informal target and formal proposition |
| S4 | Definition adequacy | Checks that formal definitions behave as intended |
| S5 | Proof-route correspondence | Comparison of formal derivation with published informal proof route |
| S6 | Mathematical significance | Assessment of whether result answers intended/important question |
| S7 | Independent replay | Independent party or implementation checks artifact |
| S8 | Semantic counterevidence | Mismatch, ambiguity, correction or pathological definition |

### R — Recognition and institutionalization

| Code | Name | Operational definition |
|---|---|---|
| R1 | Public announcement | Institution/team announces achievement |
| R2 | Formal status transition | Register changes problem status |
| R3 | Institutional certification | Named body explicitly certifies or endorses result |
| R4 | Publication recognition | Peer-reviewed publication or editorial decision |
| R5 | Community uptake | Dated evaluation by relevant mathematicians |
| R6 | Downstream reuse | Later work imports, cites, builds upon or applies artifact |
| R7 | Recognition contestation | Public challenge to status, claim or meaning |

### A — Attribution and subject positions

| Code | Name | Operational definition |
|---|---|---|
| A1 | Solver attribution | Agent/person publicly identified as solver |
| A2 | Author attribution | Authorship of exposition or result |
| A3 | Formalizer attribution | Credit for formal statement, proof code or translation |
| A4 | Validator attribution | Credit/responsibility for semantic and mathematical review |
| A5 | Infrastructure attribution | Credit for libraries, tools and maintenance |
| A6 | Collective credit | Recognition distributed across team/community |
| A7 | Attribution asymmetry | Some roles foregrounded while others backgrounded |
| A8 | Machine subject position | Machine represented as solver, collaborator, tool, verifier or object |

### P — Practical investment and behaviour

| Code | Name | Operational definition |
|---|---|---|
| P1 | Credential reliance | Actor uses certificate/status as reason to accept or use result |
| P2 | Continued use with acknowledged limits | Same actor acknowledges limit and continues relevant reliance |
| P3 | Procedural incorporation | Credential becomes part of workflow, checklist or policy |
| P4 | Behavioural change | Observable downstream action changes because of credential |
| P5 | Public contestability | Others can inspect, challenge, correct and receive response |
| P6 | Disavowal evidence | Acknowledged gap is practically treated as settled or displaced by credential; requires both acknowledgement and evidence of substitution |
| P7 | Counter-practice | Workflow keeps scope, semantic checks and provenance visible |

### I — Infrastructure and material organization

| Code | Name | Operational definition |
|---|---|---|
| I1 | Material artifact | Proof object, repository, register, benchmark or interface stabilizes result |
| I2 | Standardization | Shared definitions, libraries, labels and review conventions structure practice |
| I3 | Gatekeeping | Maintainers, experts, institutions or review systems control admission |
| I4 | Labour visibility | Infrastructure makes contributions traceable or hides them |
| I5 | Maintenance dependence | Result depends on sustained maintenance/version compatibility |
| I6 | Scarcity/bottleneck | Qualified reviewers/maintainers constrain adjudication; requires direct evidence |

## 4. Polarity and confidence

- Supports: record directly supports operational definition.
- Contradicts: record directly provides contrary evidence.
- Mixed: record supports and limits claim.
- Not observed: defined search has not found evidence; not proof of absence.

High confidence: primary record, explicit action, exact locator, stable version.  
Medium: credible participant account or independent secondary source with adequate locator.  
Low: indirect inference, incomplete snapshot or ambiguous provenance.

## 5. Cross-case comparison matrix

Complete each cell with coded records before writing an interpretation.

| Dimension | RH | NS | APN | LTE |
|---|---|---|---|---|
| Problem framing | Pending | Pending | Pending | Pending |
| Formal specification | Pending | Pending | Pending | Pending |
| Proof production | Pending | Pending | Pending | Pending |
| Semantic validation | Pending | Pending | Pending | Pending |
| Independent replay | Pending | Pending | Pending | Pending |
| Institutional recognition | Pending | Pending | Pending | Pending |
| Downstream reuse | Pending | Pending | Pending | Pending |
| Attribution pattern | Pending | Pending | Pending | Pending |
| Credential reliance | Pending | Pending | Pending | Pending |
| Counter-practice | Pending | Pending | Pending | Pending |

## 6. Sampling

- Core census: all official statements, main papers, formal declarations and status-changing PRs.
- Purposive repository sample: PRs/issues concerning theorem statements, definitions, proof corrections, review, attribution and reproducibility.
- Reception sample: dated responses by mathematicians, participants, institutions and independent reviewers.
- Reuse sample: subsequent papers/repositories citing or importing artifacts.
- Negative-case sample: at least one limiting or contradictory source per case where available.

Report purposive sampling as purposive, not random or exhaustive.

## 7. Inter-coder reliability

If a second human coder becomes available, independently code a preselected subset (e.g. 10–20%), resolve disagreements transparently and report an appropriate agreement measure. Until then, describe the work as single-researcher qualitative coding, not inter-coder validated.
