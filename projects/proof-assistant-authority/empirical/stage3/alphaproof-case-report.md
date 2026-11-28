# AlphaProof Nexus — Public Recognition and Knowledge Reuse

**Snapshot:** 2026-11-28  
**Primary sources:** AP-01 through AP-12 and SEARCH-AP-01 in source-register.md.

## 1. Nine statements in the Science paper are not nine original Erdős problems

The Science paper's Table 1 reports nine formalized statements across seven Erdős problem numbers. The table contains two parts of #12, two parts of #741, and three variants. The #26 item is a Tenenbaum variant, not an original problem posed by Erdős.

| Science-table item | Target | Status reported |
|---|---|---|
| #12(i) | Divisibility-restricted infinite set with a positive density condition | Existence |
| #12(ii) | A second density/divisibility question associated with #12 | Negative answer |
| #125* | Positive lower-density variant for a sumset of base-3/base-4 digit sets | Negative answer |
| #138* | Difference variant concerning W(k+1)-W(k) | Proved |
| #152 | Growth of isolated elements in A+A for sufficiently large Sidon sets | Proved |
| #741(i) | Corrected upper-density version of the partition question | Proved |
| #741(ii) | Second additive-basis statement associated with #741 | Proved |
| #846 | Finite decomposition statement for planar point sets | Negative answer |
| #26† | Tenenbaum variant of the Behrend problem | Negative answer |

The asterisk marks variants; the dagger marks the #26 generalization. The paper's abstract uses the compact phrase “nine Erdős problems,” while the table makes the mixture of problem parts and variants visible.

## 2. The pinned archive and the Science table differ at #741(i)

The pinned AlphaProof results archive at commit `42f344cfa9d57154f36e6b9bef1f71760a438c54` contains nine files under `APNOutputs/ErdosProblems/`. Eight correspond to the Science-table targets. The #741(i) file is a different density reading:

- `erdos_741.parts.i.lean` formalizes the natural-density reading and gives a counterexample.
- The Science paper's Table 1 counts the corrected upper-density version.
- Formal Conjectures PR #3778 records the upper-density variant as solved and attributes discovery to the DeepMind prover agent.

The paper itself explains that, for #125 and #741(i), the interpretation of “density” was corrected after the agent found proofs under the natural-density reading. The agent then resolved the corrected lower- and upper-density questions. For #741, the archive's natural-density counterexample and the PR's upper-density result are distinct mathematical statements.

Accordingly, the pinned archive has nine proof files, but its #741(i) file is not the #741(i) target counted in the Science table. Counting both density readings gives ten proof items across the archive and the Formal Conjectures record, consistent with the external audit's ten-item replay count.

The nine file-level Git blob SHAs are recorded in the evidence ledger as AP-FILE-01 through AP-FILE-09. A file scan found no explicit `sorry`, `admit` or `axiom` token in those nine files. This source scan is kept distinct from the external kernel replay and from semantic comparison with the original historical problems.

## 3. Recognition and validation

The Science paper (8 October 2026) reports nine solved formal statements among 353 formalized open Erdős problems and 44 OEIS conjectures among 492 attempts. It states that, after each solve, experts on the team checked that the Lean statement faithfully captured the original conjecture. The paper also describes human review of the OEIS formulations.

The public recognition chain includes:

- the peer-reviewed Science article;
- the pinned AlphaProof results archive;
- the Formal Conjectures status records;
- PR #3778, which records the corrected upper-density variant of #741(i);
- PR #4384, whose 53 commits and 135 comments document extensive human review, statement correction and integration for the OEIS outputs;
- the external Toledo audit, which reports ten proof items replayed through Lean and nanoda while treating statement correspondence as a separate question.

A status transition is evidence of local institutional recognition, not by itself evidence of universal mathematical consensus.

## 4. Human and machine contribution

The Science paper has 21 human authors. Its contribution statement assigns the prover agent the proof-search/discovery role, while humans selected and formalized targets, validated statements, wrote natural-language proofs, contributed Lean formalizations, coordinated runs, integrated the repository and wrote the paper. Agent-generated drafts assisted some natural-language proof writing. The first three authors are listed in random order with equal contribution.

The paper identifies several distinct human roles: George Tsoukalas initiated and led the use of the system on mathematical research tasks; George Bérczi was the first research mathematician to use AlphaProof Nexus; named authors identified problems and validated generated solutions; a larger group contributed Lean formalizations and natural-language proofs; and the repository was coordinated by a human author.

The public attribution is therefore layered: automated proof search, human problem selection, statement design, expert validation, formalization, exposition and repository integration.

## 5. Downstream use of the nine Erdős results

Within the bounded scholarly and repository search, no later mathematical paper or formal development was located that uses one of the nine Science-table Erdős results as a premise in a new theorem. The statements entered a public proof archive and formal status registers, but a status transition, citation or repository presence is not itself theorem-level mathematical dependence.

This is a bounded negative finding about the nine Erdős outputs, not a claim that AlphaProof has no downstream research use.

## 6. A separate downstream application: monochromatic quantum graphs

The AlphaProof paper also reports a separate quantum-graph result. The formal target is the non-existence of complex-weighted monochromatic quantum graphs for even N at least 4 in the case D=N. The proof is recorded in Formal Conjectures at commit `af88acbf9da0f26e3e934743a819e986e02f6875`. The Krenn paper extends the result to D greater than N by restricting the colour set.

Krenn et al. (arXiv:2611.26300v1, 19 November 2026) turn this AI-discovered proof into a tensor-algebraic argument and give a physical interpretation for photonic GHZ-state generation. Their Table 1 explicitly labels the April AlphaProof Nexus result “formally verified, human-digested (this manuscript).” This is a clear example of translation from formal discovery to a human-readable mathematical argument and a physical application. It is not one of the nine Erdős outputs.

The same table records three subsequent AI-assisted results in the quantum-graph research line:

- Kenta Kitamura's July result on the bound D_max ≤ N−2 for even N at least 6;
- Kenta Kitamura's July result for integer weights, D_max=2;
- Rishi Rajasekaran's September result proving D_max=2 for even N at least 6.

The Krenn paper describes the Kenta and Rishi results as formally verified but not human-digested. It attributes the Rishi proof to Codex/Claude. Formal Conjectures PR #6627, by contrast, attributes proof construction to GPT-6 Astra and the Lean 4.35 port to Claude Fable 5.2. Both attribution records are preserved without attempting to reconcile their tool labels.

The Rishi repository's final `Solution.lean` contains no proof hole and proves the all-orders statement for even N at least 6 and D at least 3. PR #6627 remains open and points to the external proof; PR #8283 merged narrower N=6 support; the external proof is registered in Palomar. This is a separate AI-assisted proof project, not an AlphaProof output.

## 7. Case judgment

AlphaProof has strong institutional recognition and a visible human-validation chain. The nine Science-table Erdős results are formally archived and locally recognized, but direct downstream theorem dependence on those nine statements was not located. The #741 density correction shows that proof search can also feed back into the articulation of the target statement.

The separate quantum-graph result has a clearer research afterlife: it is translated into a human-digested mathematical argument and physical interpretation, and it becomes part of a continuing line of AI-assisted research.

The dominant trajectory is **benchmark recognition → formal status and attribution → statement correction and expert validation → separate research application → human mathematical translation**, with the nine Erdős outputs and the quantum-graph research line kept analytically separate.
