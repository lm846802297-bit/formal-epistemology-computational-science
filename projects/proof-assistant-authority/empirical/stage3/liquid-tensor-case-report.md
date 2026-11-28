# Liquid Tensor Experiment — Public Recognition and Knowledge Reuse

**Snapshot:** 2026-11-28  
**Primary sources:** LTE-01 through LTE-14 and SEARCH-LTE-01 in source-register.md.

## 1. Definitions and theorem proved

The original `leanprover-community/lean-liquid` repository is a Lean 3 project pinned to Lean 3.48.0 and a Mathlib3 revision. Its source definitions use sheaves on the Profinite category with the pro-étale topology:

```lean
def CondensedSet : Type (u+2) :=
  Sheaf proetale_topology (Type (u+1))

def Condensed (C : Type u) [category C] :=
  Sheaf proetale_topology C
```

The source comments note that these objects are, strictly speaking, pyknotic in the formal implementation, while being intended to serve the same purpose in Lean's type theory.

The main theorem development has two layers:

- `first_target` formalizes a combination of Analytic 9.4 and 9.5.
- `liquid_tensor_experiment` formalizes Clausen–Scholze Theorem 1.1: the relevant Ext groups from p-measures on a profinite set to a p-Banach space vanish in positive degrees.

The project README records completion of the first target in 2021 and completion of Theorem 1.1 on 14 July 2022. The original definitions and proof code remain in the Lean 3 repository.

## 2. Recognition and collaborative organization

The project received recognition within the Lean/Mathlib community through Scholze's public accounts, Commelin's updates and the Mathlib completion announcement. The Stage 1 repository census records 57 PRs (49 merged, 6 closed unmerged, 2 open) and 15 PR-author accounts. These are repository participation measures, not a complete count of mathematical labour.

The public Blueprint keeps the mathematical exposition, formal declarations and dependency structure navigable. The Leanblueprint project lists the Liquid Tensor Experiment among the projects using the tool; the Lean community's Zulip archive also records the project's use of `PatrickMassot/leanblueprint`.

## 3. Direct reuse of definitions and proof code

The bounded GitHub code search for exact project names, theorem names and imports located the original repository, related documentation and later Mathlib4 condensed modules. It did not locate a downstream project importing the LTE target theorem or its Lean 3 proof declarations directly.

The newer Mathlib4 `Condensed.Basic` implementation, authored by Adam Topaz, uses a different site:

```lean
Condensed (C) := Sheaf (coherentTopology CompHaus) C
```

This is a separate Lean 4 implementation on compact Hausdorff spaces with the coherent topology. Its source comments describe future work to relate the CompHaus, Profinite and extremally disconnected presentations. It is not a verified port of the LTE Lean 3 theorem or proof code.

The later Atlas Lean project imports `Mathlib.Condensed.TopComparison` and uses Mathlib4 condensed structures to construct condensed topological rings and module sheaves. This is downstream use of related condensed infrastructure, not a direct import of the LTE target theorem.

## 4. Downstream mathematical use of the underlying theory

Commelin and Topaz's 2024 Bulletin of the AMS article discusses the mathematical significance of the condensed/analytic-ring framework, including later generalizations and algebraic proofs of classical results such as Serre's GAGA theorem. These are uses of the underlying mathematics. They cannot be attributed to the Lean formalization itself without a documented dependency on the formal artifact.

The evidence therefore supports continuing mathematical use of the theory, but not a causal claim that the Lean proof generated those later mathematical results.

## 5. Methodological and Blueprint reuse

The strongest direct downstream reuse concerns method rather than theorem code.

The 2026 Carleson formalization paper (arXiv:2609.31334v1) explicitly states that the strategy of proving basic expected properties of definitions as semantic sanity checks goes back at least to the Liquid Tensor Experiment. It also discusses the use of Blueprint software to keep the informal mathematical structure and formal proof aligned.

The associated Carleson repository publishes a Blueprint and dependency graph, and its `blueprint/requirements.txt` directly depends on `PatrickMassot/leanblueprint`. The Leanblueprint README itself lists LTE among its example projects. This is documentary evidence of methodological and tool uptake, not of theorem-code reuse.

The 2026 LeanMarathon paper also cites LTE among large collaborative formalization projects and uses an evolving Blueprint as a shared system of record. This is adjacent evidence of broader blueprint-based practice; it does not establish a direct line of influence for every design choice.

The 2024 Commelin–Topaz article provides a scholarly analysis of the experiment's abstraction boundaries and spec-driven development.

## 6. Attribution and subject positions

LTE makes human mathematical work unusually visible: named contributors, public PR review, semantic examples, documentation discussion and Blueprint dependencies remain part of the result's public presentation. The formal system is positioned as a checker and shared formalization environment within a collaborative project, not as an autonomous solver receiving exclusive credit.

## 7. Case judgment

**Recognition:** strong within the formal mathematics community.  
**Direct theorem/proof-code reuse:** not located in the bounded search.  
**Underlying mathematical theory use:** documented in later condensed/analytic mathematics.  
**Related formal infrastructure:** present in Mathlib4 and used by Atlas Lean, through a distinct implementation.  
**Methodological uptake:** explicit in the Carleson formalization, including definition-sanity checks and Blueprint tooling.  
**Dominant trajectory:** **collaborative formalization → public semantic auditability → definition-checking and Blueprint diffusion**, rather than direct reuse of the original proof code.
