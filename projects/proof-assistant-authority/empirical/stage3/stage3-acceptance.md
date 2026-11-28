# Stage 3 Acceptance Record

**Date:** 2026-11-28  
**Branch:** `research/stage3-recognition-reuse`  
**Tracking issue:** [#8](https://github.com/lm846802297-bit/philosophy-papers/issues/8)  
**Draft PR:** [#9](https://github.com/lm846802297-bit/philosophy-papers/pull/9)

## 1. Scope fixed before acceptance

Stage 3 covers exactly four cases:

1. Riemann Hypothesis (2026 Lean archive).
2. Navier–Stokes (OpenAI, 2026).
3. AlphaProof Nexus / Erdős problems.
4. Liquid Tensor Experiment.

Waring's problem and other projects are not added as fifth cases. External projects appear only as evidence of downstream use, methodological uptake or comparison.

Stage 1 and Stage 2 are frozen inputs. Their accepted ledgers and conclusions are reused rather than recollected wholesale.

## 2. Predefined acceptance criteria

| Criterion | Required evidence | Result |
|---|---|---|
| Existing public-reception material | Prior `PUBLIC_TRUST_AND_RECEPTION.md` inspected and existing evidence migrated without replacing the original | PASS |
| Source traceability | New claims point to source-register IDs; repository artifacts are pinned to commits or file blob SHAs where available | PASS |
| Riemann investigation | Community recognition, independent verification, reconstruction, public counter-evidence and downstream-use search recorded | PASS |
| Navier–Stokes investigation | Independent critique, repository correction history, source-level mismatch persistence, technical reuse and downstream-use search recorded | PASS |
| AlphaProof investigation | Nine Science-table statements distinguished from archive files; #741 density correction, attribution, independent audit and later research use recorded | PASS |
| LTE investigation | Definitions, theorem statements, Lean 3 implementation, Blueprint, later mathematical infrastructure and method uptake distinguished | PASS |
| Unified comparison | Four cases compared on recognition, validation, attribution, translation, artifact reuse, method uptake and theorem-level dependence | PASS |
| Theory selection | Core framework selected from the four-case evidence; auxiliary theories and novelty constraints stated | PASS |
| Manuscript isolation | No manuscript file changed; no Stage 1/2 record, PR #6 or PR #7 modified | PASS |
| Scope discipline | No fifth case, no population-level trust claim, and no inference from citation/mention to mathematical dependence | PASS |

## 3. Accepted empirical conclusions

### Riemann Hypothesis

The case has strong formal-community and public recognition, independent machine checking, active Polymath participation and several human-readable reconstructions. Its early afterlife is dominated by verification, archival preservation and mathematical reconstruction. No downstream theorem dependence was located in the bounded search. The non-peer-reviewed Emmerson preprint is recorded as public counter-evidence, not as an adjudicated disproof.

### Navier–Stokes

The second OpenAI commit closed an initial formal-artifact completeness gap by adding candidate and theorem files. The two source files cited for the later paper-to-Lean discrepancies remained byte-identical between the initial and 10 September commits. The case therefore contains both a documented repository correction and persistent intermediate proof-route mismatches. Direct technical reuse is substantial: benchmark, port, audit and formal-library integration. No downstream theorem dependence was located.

### AlphaProof Nexus

The Science paper's nine formalized statements cover seven unique Erdős problem numbers and include three variants; #26 is a Tenenbaum variant rather than an original Erdős problem. The nine files in the pinned results archive are not identical to the nine rows in the Science table: the archive's #741(i) file formalizes the natural-density reading, while the paper's table counts the corrected upper-density version recorded in Formal Conjectures PR #3778. The extra natural-density result and the corrected upper-density result are kept separate.

The nine Erdős results have formal status and a human-validation chain, but no later theorem depending on one of those nine was located. A separate AlphaProof Nexus quantum-graph result has a clearer mathematical afterlife: Krenn et al. translate it into a tensor-algebraic proof and physical interpretation. Later Kenta Kitamura and Rishi Rajasekaran results are recorded separately, with their own tool and attribution statements.

### Liquid Tensor Experiment

The original Lean 3 definitions and theorem remain in the `lean-liquid` repository. No direct downstream import of the LTE target theorem or proof declarations was located. Related condensed mathematics is formalized separately in Mathlib4 and used by later projects. The strongest demonstrated downstream effect is methodological: LTE's definition-sanity-check strategy and Blueprint practice are explicitly recognized and reused in later formalization work, including Carleson's theorem.

## 4. Accepted theoretical selection

Retain Marx–Lacan–Žižek as the core framework:

- Marx explains how distributed mathematical labour can appear as a property of a portable proof artifact.
- Lacan's Big Other and subject-supposed-to-know explain symbolic authorization and the position assigned to a solver or certificate.
- Žižek's practical belief and ideological fantasy explain the conditional transfer from a genuine, bounded formal warrant to a broader sense of closure.

Use Bourdieu/Merton for recognition and credit, Derrida for archival selection and repeatability, and Hardwig/STS as the rational-dependence and material-production baseline.

Treat **post-verification circulation** as a middle-range descriptive model with distinct modes—credentialization, translation, integration, assimilation and archival stabilization—not as a universal linear sequence.

The stronger diagnosis of fetishistic disavowal remains conditional: it requires an acknowledged gap, an observable practice subordinating that gap to the credential, and a consequence for recognition or action. Stage 3 does not establish community-wide private disavowal or deliberate cynicism.

## 5. Acceptance decision

**Stage 3 is accepted at documentary scope.**

The acceptance covers the four-case evidence dossier, source register, evidence ledger, comparison, theoretical selection and revision plan. It does not mean that the manuscript has already been revised, that every preprint claim has been adjudicated, or that a journal has accepted the paper.

The PR remains a Draft and is not merged by this acceptance record.

## 6. Next phase

The next phase is a separate manuscript revision beginning with the theoretical framework only. Case-section, abstract and conclusion revisions remain deferred until that first round is reviewed. The current manuscript remains unchanged.
