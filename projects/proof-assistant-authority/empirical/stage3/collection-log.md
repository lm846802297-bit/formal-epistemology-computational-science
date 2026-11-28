# Stage 3 Collection Log

## 2026-11-28 — Stage initiated

### Governance and repository state
- Created tracking issue #8: Stage 3 public recognition and downstream knowledge reuse.
- Created branch `research/stage3-recognition-reuse` from accepted Stage 2 dossier commit `5232f13feb215320c876f8f9cc79e6741beb44a8`.
- PR #6 and PR #7 remain open Draft; no changes made to either.
- Manuscript/theoretical chapter files are out of scope for this stage.

### Existing evidence reused, not recollected
- Stage 1 event ledger, 78 participation edges, 23-PR review sample, contribution-network analysis and case reports.
- Stage 2 AlphaProof/LTE synthesis and theory-evidence map.
- Existing source register and coding framework.
- Existing public-reception module was located in the wider research project; its existing material is a starting point and must be inspected in the current branch before any append/merge decision. Do not create a duplicate public-reception corpus.

### Initial literature discovery
Searches were run across scholarly indexes for mathematical formalization dependencies, software citation, scientific recognition/citation, Derrida/archive theory, and Byung-Chul Han/digital visibility. Initial leads are recorded in the Stage 3 README and require source-level assessment before use.

Important method leads:
- Li et al. (2026), *The Network Structure of Mathlib*: declaration and module dependency graphs. It demonstrates that formal dependency networks can be analyzed at scale; it does not establish reuse of any one of our four case artifacts.
- Kurgan et al. (2026), *TheoremGraph*: cross-formal/informal theorem dependency graph. Preprint; methods and precision of inferred links need inspection.
- Druskat (2019), *Software and Dependencies in Research Citation Graphs*: argues that software/dependency relationships are poorly represented in ordinary citation graphs.
- FORCE11 software citation principles: persistent, specific software identity and attribution.
- Desrochers et al. (2018), Tahamtan & Bornmann (2022): citation, acknowledgement, symbolic capital and citation functions.
- Han and Derrida are retained as conditional theory candidates, not assumed to fit the evidence.

### Initial empirical status
- No downstream reuse event is marked as confirmed solely from citation counts, stars, views, downloads or generic Mathlib imports.
- No new case-level reuse conclusion has been accepted yet.
- Search and screening boundaries, including negative searches, will be recorded before any “no reuse found” statement.

### Next actions
1. Inspect existing public-reception records and map already collected materials to the new Stage 3 evidence classes.
2. Build per-case query plans and date windows.
3. Search exact downstream citations, repositories, imports, forks, adaptations and independent replay.
4. Populate the evidence ledger with exact immutable locators and counter-evidence.
5. Produce case reports only after each case's evidence has been screened.


## 2026-11-28 — Four-case collection and Stage 3 acceptance

### Existing public-reception materials integrated
- Mapped the pre-existing Riemann media sample, Science Media Centre comments, Reddit threads, Navier–Stokes public discussion, AlphaProof expert responses and general survey baselines into the Stage 3 evidence ledger.
- Excluded Waring's problem from the four-case corpus as specified.
- Kept population surveys as contextual sources only; none measures trust in Lean or machine-checked proofs.

### Riemann
- Added the Polymath launch, Waterloo independent-check/reconstruction page, readable refactor and Adriazola reconstruction.
- Verified the community repository's original/alpoge/main branch provenance and contributor-file caveat.
- Found strong independent formal checking and substantial human reconstruction; no downstream theorem dependency located.

### Navier–Stokes
- Compared the 8 September and 10 September OpenAI commits. The second adds 188 changed files, 19,388 additions and 79 deletions, including the candidate/theorem files that discharge energy and force-support obligations.
- Inspected the Bastounis–Circelli–Hansen critique, New Scientist/OpenAI response, KCL summary, cert-machine audit and SafeVerifyAgent audit.
- Added three downstream technical reuse records: Vilin97 reproducible benchmark with SHA-256 provenance manifest, KTS Global Lean 4 port, and Tengoku formal-library integration.
- No later theorem-level mathematical dependence located.

### AlphaProof
- Pinned the nine Erdős proof files at archive commit 42f344cfa9d57154f36e6b9bef1f71760a438c54 and recorded their Git blob SHAs.
- Confirmed that the nine files contain no explicit sorry/admit or axiom declarations; this is a source inspection, not a substitute for the recorded build/replay evidence.
- Re-read the Science paper's author contribution statement and the exact problem table. The nine entries represent seven unique problem numbers and include parts/variants; #26 is a Tenenbaum variant.
- Added the Krenn quantum-graph follow-up, the Formal Conjectures proof commit, and the separate Rishi Rajasekaran all-orders proof/Palomar record. Kept the latter separate from AlphaProof attribution.
- No direct downstream use of the nine Erdős outputs located.

### Liquid Tensor
- Inspected the Lean3 repository, toolchain pin, Blueprint and later literature.
- Found explicit methodological uptake in the Carleson formalization: definition-sanity-check strategy traced to LTE and Blueprint used in the project.
- Found related Mathlib4 condensed infrastructure used by Atlas Lean, but not a direct port of the LTE theorem/proof code.
- No direct downstream import of the LTE target theorem/proof located.

### Theory selection and reviewer-evaluation integration
- Consulted the uploaded paper-evaluation file and mapped its three root questions (fetish-form, practical investment, real effects) to the four-case evidence.
- Selected Marx–Lacan–Žižek as the core mechanism; added Bourdieu/Merton for recognition, Derrida for archive/versioning, and Hardwig/STS as the baseline.
- De-prioritized Han as a core framework on current evidence.
- Added post-verification circulation as a candidate middle-range model, with explicit novelty constraints from Kallel & El Louadi, López-Corona, Druskat, FORCE11, De Millo et al., MacKenzie, Rosental, Mathlib network work and TheoremGraph.

### Acceptance
- Created stage3-acceptance.md and manuscript-revision-plan.md.
- Stage 3 accepted at the documentary scope stated in the acceptance record.
- No Stage 1/2 files, PR #6, PR #7 or manuscript files were modified in this Stage 3 branch.


## 2026-11-28 — Source reconciliation and acceptance amendment

The earlier collection entry recorded that the acceptance and revision-plan documents had been created; those files were not present in the branch tree at the time of this audit. They have now been added as actual version-controlled artifacts, together with the theory synthesis. The README links directly to all deliverables.

Additional source-level checks and corrections:

- Reconciled the Science Table 1 nine statements with the nine pinned AlphaProof archive files. The #741(i) natural-density archive file and the corrected upper-density result in PR #3778 are distinct; both are now separately recorded.
- Added the Krenn quantum-graph follow-up and the Kenta/Rishi continuation records. The tool-attribution difference between the Krenn paper and Formal Conjectures PR #6627 is preserved.
- Compared the two OpenAI Navier–Stokes commits at the exact blob level. The cited inverse-estimate and pressure-flux files are unchanged across the initial and 10 September commits.
- Compared the original LTE Lean 3 condensed definitions with the first Mathlib4 Condensed implementation. They use different sites and are not a direct port.
- Verified the Carleson Blueprint package dependency and the explicit reference to LTE's definition-sanity-check strategy.
- Added the Emmerson preprint as public counter-evidence in the Riemann case; it is recorded as a non-peer-reviewed challenge, not as an adjudicated disproof.
- Repaired the source-ID crosswalk for the existing Reddit and bounded-search records, and added file-level Git blob pins for the nine AlphaProof files and the key Navier–Stokes/LTE source files.

The case comparison is now populated. The theoretical selection is complete and the manuscript-revision plan is separate. No manuscript file was edited.
