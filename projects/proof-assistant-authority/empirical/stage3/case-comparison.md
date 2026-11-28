# Stage 3 — Four-Case Recognition and Reuse Comparison

**Snapshot:** 2026-11-28  
**Status:** completed source-pinned comparison; no manuscript text changed.

## 1. Unified comparison matrix

| Dimension | Riemann Hypothesis | Navier–Stokes | AlphaProof Nexus | Liquid Tensor Experiment |
|---|---|---|---|---|
| Public / institutional recognition | High formal-community and mainstream media recognition | High institutional and media recognition through OpenAI announcement | High scholarly recognition through Science and Formal Conjectures status records | Strong recognition within Lean/Mathlib and formal-mathematics communities |
| Independent checking | MIT and Waterloo verification routes; Lean FRO/Mathlib statement vetting | Kernel checks, cert-machine and SafeVerifyAgent audits; later paper-to-Lean critique | Expert statement validation plus external ten-item/two-kernel audit | Collaborative PR review, explicit semantic examples and public Blueprint |
| Human translation | Polymath, Waterloo and Adriazola reconstructions; still incomplete | Independent paper-to-Lean analysis and public critique; no consensus human reconstruction located | Krenn quantum-graph result human-digested into tensor-algebraic proof and physical interpretation; Rishi full proof not yet human-digested | Natural-language proof and Blueprint are integral to the project |
| Direct artifact reuse (R3) | Strong in readable refactor and reconstruction | Strong in benchmark, Lean 4 port and library integration | Nine Erdős outputs archived; no later direct reuse of those nine located; separate quantum-graph proof enters a new paper | No direct import of the original Lean 3 target theorem/proof located |
| Methodological uptake (R2) | Collective reconstruction and formal reading practices | Reproducible benchmark, audit and porting practices | AI-assisted formal proof search deployed in a separate quantum-optics research result | Strong: definition-sanity-check strategy and Blueprint tooling explicitly reused in Carleson formalization |
| Result-level mathematical dependence (R4) | Not located | Not located | Not located for the nine Erdős outputs; the separate quantum-graph result is used in a human-authored physical interpretation and extended in later AI-assisted work | Not located for the LTE Lean theorem; underlying condensed mathematics continues in later research |
| Independent replay / replication (R5) | Strong, multiple checking routes | Strong at the build/kernel level for the benchmarked versions; semantic scope remains disputed | External replay of ten proof items through Lean and nanoda | Formal build and public collaborative review are documented |
| Attribution pattern | Alpöge/Claude origin plus separate checkers, maintainers and reconstructors | OpenAI system and GPT workflow; downstream projects preserve source attribution | AI proof-search role plus human target selection, validation, formalization, exposition and repository work | Named human collaborators and visible PR/Blueprint contributions |
| Main counter-evidence / qualification | Emmerson non-peer-reviewed foundational critique; incomplete human reconstructions | m+5 versus m+4 inverse estimate and pressure-flux mismatch persist in files unchanged since initial commit | Nine archive files do not exactly match the nine Science-table statements at #741(i); #125/#138/#26 are variants | Mathlib4 condensed implementation is related but not a direct port; no direct LTE proof-code import found |

## 2. Reuse levels

The ledger uses the following distinctions:

- **R0:** recognition or mention only; no demonstrated downstream reuse.
- **R1:** citation or contextual use without evidence of uptake.
- **R2:** methodological or infrastructure uptake.
- **R3:** direct artifact reuse, such as a code import, proof-file port, benchmark or reconstruction from the formal source.
- **R4:** result-level mathematical dependence, where a later theorem or research argument uses the result as a premise.
- **R5:** independent replay or replication at a specified formal/build level.

The levels are not a ranking of mathematical importance. A case can have R3 technical reuse and no R4 theorem dependence. R5 replay does not automatically establish semantic fidelity or human understanding.

## 3. Four distinct post-verification trajectories

### Riemann: certification and reconstruction

The result receives strong institutional recognition and independent checking. Its public afterlife is dominated by archival preservation, readable refactoring, replay, public contestation and human reconstruction. Polymath participation is genuine mathematical-community uptake, but no later theorem dependency was located.

### Navier–Stokes: contested correspondence and technical integration

The initial formal artifact was completed after the announcement. Later source-level comparison shows that two files central to the paper-to-Lean critique remained byte-identical across the initial and 10 September commits. At the same time, the formal artifact is directly reused in a benchmark, port and larger library. Technical reuse therefore coexists with a persistent correspondence dispute.

### AlphaProof: status, correction and selective assimilation

The Science paper's nine statements cover seven unique problem numbers and include variants. The #741 density correction shows that proof search can feed back into the articulation of the target statement. No downstream theorem use of the nine Erdős outputs was located. A separate AlphaProof Nexus quantum-graph result, however, is translated into a human-digested mathematical proof and physical interpretation, and becomes part of a continuing AI-assisted research line.

### Liquid Tensor: semantic auditability and methodological diffusion

The original Lean 3 theorem is not directly imported by the later projects inspected. Related condensed mathematics is reimplemented in Mathlib4, and later projects use that infrastructure. The strongest direct uptake is methodological: definition-sanity checks and Blueprint software are explicitly carried into later formalization practice.

## 4. Cross-case findings

1. **Recognition and reuse are independent.** High media or institutional recognition does not entail theorem-level mathematical dependence.
2. **Artifact reuse and result assimilation are different.** Navier–Stokes is technically reused despite a correspondence dispute; the nine AlphaProof Erdős outputs are archived without located downstream theorem dependence.
3. **Methodological uptake can outlive proof code.** LTE's Blueprint and definition-checking practice have clearer downstream evidence than direct reuse of its Lean 3 proof.
4. **Formalization can change the target.** The AlphaProof density corrections show that proof search can expose ambiguity and trigger a revised statement, rather than merely certify a fixed translation.
5. **Human translation is a separate empirical event.** It is incomplete and contested in Riemann, absent as a settled consensus in Navier–Stokes, explicit for the Krenn quantum-graph result, and built into LTE's collaborative Blueprint practice.
6. **Attribution is distributed.** Across all four cases, proof discovery, formalization, validation, maintenance, exposition and institutional recognition are not performed by one actor.

## 5. Implication for the philosophical argument

The four cases support a conditional account of symbolic authorization, not a universal claim that formal verification automatically becomes ideological authority. A genuine kernel-level warrant can circulate as a credential, but its subsequent path depends on statement fidelity, human translation, institutional recognition, technical integration and later mathematical uptake.

The comparison therefore supports retaining Marx–Lacan–Žižek as the core explanatory framework while using Bourdieu/Merton, Derrida, Hardwig and STS for distinct auxiliary tasks. **Post-verification circulation** is best treated as a middle-range descriptive model, not as a replacement philosophical theory.

## 6. Bounded negative findings

“Not located” means that the stated searches did not identify a qualifying downstream theorem dependency within the public sources inspected by 2026-11-28. It is not a claim that no such use exists anywhere. No population-level trust or private belief is inferred from media or Reddit samples.
