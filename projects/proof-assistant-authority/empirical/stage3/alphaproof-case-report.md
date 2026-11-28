# AlphaProof Nexus — Public Recognition and Knowledge Reuse

**Snapshot:** 2026-11-28  
**Primary sources:** AP-01 through AP-10 in source-register.md.

## 1. What the nine formalized Erdős statements are

The pinned AlphaProof results archive contains nine proof files:

| Formalized item | File |
|---|---|
| Erdős #12(i) | APNOutputs/ErdosProblems/erdos_12.parts.i.lean |
| Erdős #12(ii) | APNOutputs/ErdosProblems/erdos_12.parts.ii.lean |
| Erdős #125, positive lower-density variant | APNOutputs/ErdosProblems/erdos_125.variants.positive_lower_density.lean |
| Erdős #138, difference variant | APNOutputs/ErdosProblems/erdos_138.variants.difference.lean |
| Erdős #152 | APNOutputs/ErdosProblems/erdos_152.lean |
| Tenenbaum variant associated with #26 | APNOutputs/ErdosProblems/erdos_26.variants.tenenbaum.lean |
| Erdős #741(i) | APNOutputs/ErdosProblems/erdos_741.parts.i.lean |
| Erdős #741(ii) | APNOutputs/ErdosProblems/erdos_741.parts.ii.lean |
| Erdős #846 | APNOutputs/ErdosProblems/erdos_846.lean |

The nine entries represent seven unique problem numbers. The table in the Science paper identifies parts and variants; the #26 item is a Tenenbaum variant rather than an original problem posed by Erdős. The public phrase “nine Erdős problems” therefore compresses a heterogeneous set of formal targets.

The nine pinned source files contain no explicit sorry/admit or axiom declaration. Their individual Git blob SHAs are recorded in the evidence ledger. The archive commit is 42f344cfa9d57154f36e6b9bef1f71760a438c54.

## 2. Recognition and validation

The Science paper (8 October 2026) reports nine solved formal Erdős statements among 353 formalized open problems and 44 OEIS conjectures among 492 attempts. It states that experts checked whether the nine Lean statements faithfully captured the original conjectures, and that human review was used for the OEIS formulations.

The public recognition chain includes:
- the peer-reviewed Science article;
- the AlphaProof results archive;
- Formal Conjectures status records;
- PR #3778, which assigns a solved status to a specific upper-density variant of Erdős #741(i), attributes proof discovery to the DeepMind prover agent, and records human approval;
- PR #4384, whose 53 commits and 135 comments document extensive human review, statement correction and integration for the OEIS outputs.

The Toledo audit reports ten proof items replayed through two kernels. It distinguishes kernel replay from the separate question of whether each formal statement fully captures the intended historical problem.

## 3. Attribution

The Science paper has 21 human authors. Its contribution statement assigns the agent a proof-search/discovery role, while humans selected and formalized targets, validated statements, reviewed outputs, wrote natural-language proofs, integrated results and wrote the paper. Some human-written proof drafts were assisted by agent-generated drafts. The first three authors are listed in random order with equal contribution.

The agent is publicly assigned a solver/prover position, but it is not listed as a human author. The public attribution is therefore layered: agent proof discovery, human mathematical and formalization work, expert validation, repository integration and scholarly exposition.

## 4. Downstream use of the nine Erdős results

Within the bounded scholarly and repository search, no later mathematical paper or formal development was located that uses one of the nine Erdős outputs as a premise in a new theorem. The formal statements have entered status registers and an inspectable proof archive, but a status transition or citation is not itself mathematical dependence.

This is a specific negative finding about the nine outputs, not a claim that AlphaProof has no downstream research use.

## 5. A separate downstream mathematical application: quantum optics

The AlphaProof paper also reports work on monochromatic quantum graphs. The agent found a Lean proof of the even-N, D=N theorem. The actual proof is present in Formal Conjectures at commit af88acbf9da0f26e3e934743a819e986e02f6875, in the theorem no_witness_general.

Krenn et al. (arXiv:2611.26300v1, 19 November 2026) turn this discovery into a human-digested mathematical result: for even N at least 4 and D at least N, no complex-weighted monochromatic quantum graph exists. They then derive a no-go result for photonic GHZ-state generation. This is a clear example of a formal AI-discovered result being translated into a mathematical argument with a physical interpretation. It is not one of the nine Erdős outputs.

A further, separate all-orders proof by Rishi Rajasekaran uses GPT-6 Astra for proof construction and Claude Fable 5.2 for porting. The external Lean proof covers even N at least 6 and D at least 3, has no proof hole in the final solution file, and is recorded in the Palomar registry. The Krenn paper describes this result as formally verified but not yet human-digested. Formal Conjectures PR #6627 remains open and points to the external proof; PR #8283 merged narrower N=6 support. This is a separate AI proof project, not an AlphaProof output.

## 6. Case judgment

AlphaProof has strong institutional recognition and a visible human-validation chain. The nine Erdős results are formally archived and locally recognized, but direct downstream mathematical dependence on those nine statements was not located. The system's other quantum-graph output has a much clearer research afterlife: it is extended, interpreted and used in a human-authored quantum-optics preprint.

The dominant trajectory is **benchmark recognition → formal status and attribution → research application → human mathematical translation**, with the nine Erdős outputs and the quantum-optics result kept analytically separate.
