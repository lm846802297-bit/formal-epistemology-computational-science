# Riemann Hypothesis — Public Recognition and Knowledge Reuse

**Snapshot:** 2026-11-28  
**Primary sources:** RH-01 through RH-10 in source-register.md.

## 1. Recognition

The Lean FRO/Mathlib joint statement of 21 November is a formal-community recognition event. It records that the Lean statements were vetted against the intended Riemann/Generalized Riemann Hypothesis claims and that the proof artifacts were checked by the Lean kernel and independent verification routes.

The result also received broad public-media attention (Nature, Washington Post, Al Jazeera and other outlets). The Science Media Centre comments show that expert reactions were not uniform: several mathematicians described the result as potentially historic while distinguishing machine checking from understanding the mathematical structure.

The most important development after the initial announcement is the G.R.H. Polymath project, launched on 24 November by Anurag Sahay, Will Sawin and Lior Silberman. Its stated goals include coordinating mathematical work, reconstructing a human-readable proof, checking the literature and investigating generalizations. This is direct evidence of mathematical-community participation, not merely repetition of a headline.

## 2. Independent verification

The MIT verification archive and Waterloo page document independent checking of the original archive and readable refactor. The Waterloo page records several independent checking routes and publishes both a 45-page proof outline and a longer 265-page guide.

The verification evidence supports a strong claim about formal derivational validity for the pinned formal statements and environments. It does not make human mathematical assimilation identical to kernel acceptance.

## 3. Human reconstruction and artifact reuse

Three downstream activities are observable:

1. **Readable Lean refactor.** The community repository's main branch is based on Luke Sernau's readable refactor at commit 72fead102f. The repository retains separate original, alpoge and main histories, making the relation between the first release, community cleanup and readable edition inspectable.
2. **Waterloo reconstruction.** The 45-page outline and 265-page guide are attempts to recover a conventional mathematical narrative. The page explicitly records that key steps remain incomplete; they are research documents, not completed independent proofs.
3. **Adriazola reconstruction.** The public repository contains a 297-page reconstruction of the original archive, a 117-page working manuscript and a 59-page RH-specific version. It maps 60 manuscript passages to Lean declarations and reports 631 Lean theorem declarations reduced to eight principal propositions. The author labels the work incomplete, conditional and not independently verified.

The generated CONTRIBUTORS file lists 192 accounts and 6,079 merged-PR counts, including the earlier alpoge history. These figures describe repository maintenance and refactoring, not 192 theorem authors or 6,079 mathematical contributions.

## 4. Downstream mathematical use

The strongest downstream use currently located is reconstruction, independent replay, proof exposition and collective research. No later mathematical paper or formal project was located that uses the new RH result as a premise in a subsequent theorem.

This is a positive finding about the current trajectory: the result's early afterlife is primarily translation and assimilation rather than theorem-level dependency.

## 5. Attribution and subject positions

The public record assigns the original proof to Levent Alpöge with Claude assistance, while subsequent work assigns distinct roles to independent checkers, formalizers, maintainers and expositors. The reconstruction repository explicitly preserves the original attribution and describes its own contribution as reconstruction rather than a new proof.

The machine is publicly positioned as a proof-search and formalization aid; the mathematical community remains active in statement checking, reconstruction and interpretation.

## 6. Case judgment

**Recognition:** high within formal mathematics and public science communication.  
**Independent formal checking:** strong and multiply documented.  
**Human mathematical assimilation:** actively underway, not complete at the snapshot date.  
**Artifact reuse:** strong in refactoring and reconstruction.  
**Theorem-level downstream dependence:** not located in the bounded search.

The dominant post-verification trajectory is **certification → archival preservation → independent replay → human reconstruction**.
