# Pre-submission source-audit integration record

**Integration date:** 2026-11-27  
**Repository:** `lm846802297-bit/formal-epistemology-computational-science`  
**Target PR:** [#1](https://github.com/lm846802297-bit/formal-epistemology-computational-science/pull/1)  
**Target branch:** `research/initial-literature-review`  
**Branch head before integration:** `9ccaece3bfbe0fb76db1a27a14cb614d18a1251c`

## Audit source and snapshot

The author-provided source audit is preserved on branch `audit/submission-source-check-2026-11-27` at commit `b5c4ce03b1157e2af018ff857cf7b166ec1b3ee7`.

- Audited manuscript commit: `61d565a204b3ff0f76e0c9522651263617abb2a0`
- Audited integrated-manuscript blob reported in the HTML: `f080288c9196e9aefe7ee3d6b6d53074f430d11b`
- HTML report Git blob SHA: `4edf3d756b940f017fd844e4231bbd6599252329`
- CSV evidence table Git blob SHA: `363e9e332c1a132536d1da9fcbd714bc5aad545f`
- Coverage: 23 cited works and 50 claim/evidence records.
- The audit summary identifies six correction recommendations and twelve claims supported with qualifications.
- The current PR branch was eight commits ahead of the audited manuscript snapshot. Edits were mapped to current paragraphs; stale report line numbers were not applied mechanically.

## Fixed formalization source pins

- OSforGFF: `fef84a82937dfd2bb7f672108a72da329d3ef0fd`
- OSreconstruction: `cf0904e34a7c146a9f312f601e3707dca4a87697`
- OSreconstruction-comparator: `93cdb40e728ba27b7b1b55efc30d57f7b43de9aa`

## Integrated corrections

Rabe's judgment-preservation terminology and model-reduct direction; DAMF/SC-TPTP distinction; E0′ limited to the Section IV forward theorem; Douglas QFT four-dimensional scope versus OSforGFF's all-(D\geq2) corollary; Glimm–Jaffe p. 91 n. 1; Douglas et al. Remark 3.2 attribution for the L1(μ) ergodicity extension; Comparator 460-line mathematical-block scope, bidirectional record adapters, three theorem equivalences, configured targets and historical CI evidence; bounded negative finding for the three pinned public revisions; and corrected attributions for Gelfert, Hughes, Suárez, Contessa, and Frigg–Nguyen.

## Verification and limits

- The audit HTML and CSV were read from the audit branch at the pinned commit.
- The audited manuscript snapshot and current PR branch were compared before editing.
- The editable Markdown section files were regenerated as exact slices of the updated integrated manuscript.
- The anonymous LaTeX source was regenerated from the revised Markdown manuscript.
- Targeted checks cover revised claims, section synchronization, 23 references, balanced math delimiters, and anonymous metadata.
- No Lean kernel was rerun; no new proof replay or numerical computation was performed. Comparator claims rely on source comparison and archived workflow logs.
- The official `sn-jnl.cls` template remains unavailable; no successful Springer-template compilation or PDF inspection is claimed.

## Author item still open

The continuation of Glimm and Jaffe (1987), second edition, §6.1(i), containing the full OS4 quantifiers, norm, and time-average formula was not available in the public preview. The author must inspect these pages directly. All 23 source entries remain subject to author approval.
