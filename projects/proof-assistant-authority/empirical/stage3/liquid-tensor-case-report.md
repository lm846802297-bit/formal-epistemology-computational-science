# Liquid Tensor Experiment — Public Recognition and Knowledge Reuse

**Snapshot:** 2026-11-28  
**Primary sources:** LTE-01 through LTE-11 in source-register.md.

## 1. Recognition and project object

The Liquid Tensor Experiment was a collaborative formalization project around a central theorem in Clausen–Scholze's condensed mathematics. Its Lean 3 repository contains the formal definitions, theorem development, examples and supporting infrastructure. The project used a public Blueprint to keep the mathematical exposition, formal declarations and dependency structure navigable.

The project received recognition within the Lean/Mathlib community through Scholze's public accounts, Commelin's updates and the Mathlib completion announcement. The Stage 1 repository census records 57 PRs (49 merged, 6 closed unmerged, 2 open) and 15 PR-author accounts. These are repository participation measures, not a complete count of mathematical labour.

## 2. Direct reuse of definitions and proof code

The original lean-liquid repository is a Lean 3 project pinned to Lean 3.48 and a Mathlib3 revision. The main theorem and its supporting definitions remain in that repository.

The bounded GitHub code search for exact project names and imports located the original repository, references in LeanDojo documentation, and related Mathlib4 condensed modules. It did not locate a downstream project importing the LTE target theorem or its proof declarations directly.

The newer Mathlib4 Condensed.Basic implementation, authored by Adam Topaz, and downstream imports such as Atlas Lean use related condensed-mathematics structures. They are a separate Lean 4 implementation, not a verified port of the LTE theorem or proof code. This is conceptual and infrastructure continuity, not direct artifact reuse.

## 3. Downstream mathematical use of the underlying theory

Commelin and Topaz's 2024 Bulletin of the AMS article discusses the mathematical significance of the condensed/analytic-ring framework, including later generalizations and new algebraic proofs of classical results such as Serre's GAGA theorem. These are uses of the underlying mathematics. They cannot be attributed to the Lean formalization itself without a documented dependency on the formal artifact.

The evidence therefore supports continuing mathematical use of the theory, but not a causal claim that the formal proof generated those later mathematical results.

## 4. Methodological and Blueprint reuse

The strongest direct downstream reuse concerns method rather than theorem code.

The 2026 Carleson formalization paper (arXiv:2609.31334v1) explicitly states that the strategy of proving basic expected properties of definitions as semantic sanity checks goes back at least to the Liquid Tensor Experiment. It also discusses the use of Blueprint software to keep the informal mathematical structure and formal proof aligned. The associated Carleson repository provides a public Blueprint and formal development.

The 2026 LeanMarathon paper also cites LTE among large collaborative formalization projects and uses an evolving Blueprint as a shared system of record. This is adjacent evidence of broader blueprint-based practice; the paper does not establish a direct line of influence from LTE.

The distinction is important: the Blueprint tool was not invented by LTE, but the LTE project helped demonstrate and institutionalize its use in large-scale mathematical formalization. Later work explicitly reuses the definition-checking strategy and the Blueprint workflow.

## 5. Attribution and subject positions

LTE makes human mathematical work unusually visible: named contributors, public PR review, semantic examples, documentation discussion and Blueprint dependencies all remain part of the result's public presentation. The machine is positioned as a checker and formalization environment within a collaborative project, not as an autonomous solver receiving exclusive credit.

## 6. Case judgment

**Recognition:** strong within the formal mathematics community.  
**Direct theorem/proof-code reuse:** not located in the bounded search.  
**Underlying mathematical theory use:** documented in later condensed/analytic mathematics.  
**Methodological uptake:** explicit in the Carleson formalization, with broader Blueprint-based developments.  
**Dominant trajectory:** **collaborative formalization → public semantic auditability → methodological diffusion**, rather than direct reuse of the original proof code.
