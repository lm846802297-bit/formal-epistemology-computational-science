# Navier–Stokes — Public Recognition and Knowledge Reuse

**Snapshot:** 2026-11-28  
**Primary sources:** NS-01 through NS-11 in source-register.md.

## 1. Recognition and correction timeline

OpenAI announced the result on 8 September 2026. The first public repository commit is 8937a8f4 (8 September). A second commit, f9e8bc5b (10 September), added 188 changed files, with 19,388 additions and 79 deletions.

The independent cert-machine audit compares these two versions. At the initial commit, the candidate proof did not yet discharge the energy-bound and positive-time force-support obligations. The 10 September commit added ActualCandidate.lean and Theorem.lean, supplying the missing witnesses and the full theorem statement. This is a concrete post-announcement correction to the formal artifact.

The repository has only these two public commits in the inspected history and no public issues. No later repository correction was found by the snapshot date.

## 2. Independent critique and counter-evidence

Bastounis, Circelli and Hansen (arXiv:2610.08144, 6 October) identify mismatches between the written proof and the Lean formalization at the 10 September commit. Their examples include:
- the inverse estimate in written Lemma 8.6 using m+4 input derivatives while the corresponding Lean estimate uses m+5;
- a difference in the pressure-flux bound and its proof route.

The authors explicitly distinguish this paper-to-Lean correspondence problem from a claim that the theorem is false or that the Lean kernel accepted an invalid proof. OpenAI acknowledged the mismatch to New Scientist and said it would correct errors in the written proof as they were found.

The cert-machine audit reaches a different but compatible conclusion at a different level: it records that the initial commit omitted the energy/support witnesses, that the head commit supplies them, and that the main formal theorem statement matches the relevant Clay alternatives. It does not issue a verdict on the mathematical correctness of the proof.

The SafeVerifyAgent audit reports no load-bearing weakening or kernel defect in the coverage it examined. Its own coverage record shows that the audit is partial: a substantial portion of the estimate-heavy proof remains unread or only mechanically screened. It is therefore evidence of an additional audit, not a complete independent mathematical review.

These records must be kept distinct:
- statement correspondence at the theorem level;
- correspondence of intermediate arguments between paper and Lean;
- kernel acceptance of the Lean proof;
- independent mathematical understanding.

## 3. Direct technical reuse

Three public downstream uses are documented.

### 3.1 Reproducible build benchmark

Vilin97/ns-formalization-benchmark compares the OpenAI source with a LeanPool port. It pins the source and Mathlib versions, supplies a per-module SHA-256 provenance manifest, and builds the same two target theorems in the same Lean environment.

| Version | Build time | Aggregate peak memory |
|---|---:|---:|
| OpenAI source | 18m 04s | 13.273 GiB |
| LeanPool port | 11m 11s | 6.451 GiB |

The benchmark reports a 1.62x speed-up and 51.4% lower aggregate memory for the LeanPool version. This is direct source/proof reuse and independent build comparison. It does not independently establish semantic equivalence between the formal statement and the informal Clay problem.

### 3.2 Lean 4 port

KTS Global publishes a Lean 4.34.1 port and an R2/R3 community verification package. Its README explicitly says that the mathematical proof is inherited from OpenAI, that the port is not an independent mathematical proof, and that it does not claim Clay recognition or independent specialist review. This is a responsible scope statement and a direct technical port.

### 3.3 Formal-library integration

The Tengoku repository includes the LeanPool/Navier–Stokes material in a larger Lean library and records upstream attribution in its NOTICE and source metadata. This is a further artifact-integration path, not a new proof of the theorem.

## 4. Citation and mathematical use

The main scholarly follow-up located is the independent critique. The benchmark, port, audit and library aggregation demonstrate technical reuse, but no subsequent mathematical paper was located that uses the Navier–Stokes theorem as a premise in a new theorem.

The current pattern is therefore **high public recognition, substantial technical reuse and audit, but no located theorem-level downstream dependence**.

## 5. Attribution

The public announcement assigns discovery to OpenAI's internal multi-agent system and the formalization to a GPT-based workflow. The public repository's commit history is much thinner than the actual claimed production process, so repository authorship cannot be treated as a complete map of internal labour.

Downstream projects preserve source attribution to OpenAI and LeanPool. The result is not simply copied anonymously; it is ported, benchmarked, audited and integrated under explicit provenance records.

## 6. Case judgment

The case shows that formal artifacts can be reused extensively as technical infrastructure even while their relationship to a separate written proof remains contested. The initial formal archive was corrected two days after the announcement; later paper-to-Lean discrepancies remain a separate issue. The dominant post-verification trajectory is **public claim → formal correction → external critique/audit → porting, benchmarking and library integration**.
