# Stage 3 — Empirical Theory Synthesis

**Snapshot:** 2026-11-28  
**Status:** theoretical framework selected; manuscript text unchanged.

## 1. What the four cases establish

The four cases do not form one uniform story in which machine verification automatically produces scientific authority or mathematical use. They exhibit distinct post-verification trajectories.

| Case | Strongest observed trajectory | What was not established |
|---|---|---|
| Riemann Hypothesis | Formal-community recognition, independent checking, public discussion, archival preservation and human reconstruction | No downstream theorem dependence located; reconstruction remains incomplete |
| Navier–Stokes | Public claim, formal-artifact completion, independent critique, source-level comparison, technical porting and benchmark reuse | No downstream theorem dependence located; paper-to-Lean intermediate mismatches remain |
| AlphaProof Nexus | Benchmark recognition, expert statement validation, formal status and attribution; separate quantum-graph result translated into human mathematics and physics | No later theorem dependence on the nine Erdős outputs located |
| Liquid Tensor Experiment | Collaborative formalization, public semantic checks and Blueprint; later methodological uptake and related condensed infrastructure | No direct import of the original Lean 3 target theorem or proof declarations located |

The empirical result is therefore not a single acceptance pipeline. Recognition, artifact reuse, method reuse, human translation and theorem-level assimilation are separate dimensions.

## 2. The central philosophical problem

The central question remains:

**How does a genuine but bounded technical warrant become a symbolic guarantee of broader scientific certainty as the proof artifact circulates through institutions, publications, repositories and later research?**

The relevant distinction is among:

1. **Derivational validity:** whether the formal proof is accepted by the kernel and its declared foundations.
2. **Representational fidelity:** whether the formal statement and definitions capture the intended mathematical claim.
3. **Mathematical understanding:** whether researchers can reconstruct, explain and assess the argument.
4. **Institutional recognition:** whether a journal, formalization community, repository or research group confers status on the result.
5. **Downstream use:** whether later work cites, imports, extends or depends on the result.

These dimensions can reinforce one another, but none entails all the others.

## 3. Retained core framework

### 3.1 Marx: commodity fetishism and objectified labour

The proof artifact is produced through distributed labour: problem selection, mathematical planning, formal statement design, proof search, tactic and library work, expert validation, maintenance, exposition and attribution.

A portable formal artifact can make this distributed production appear as an intrinsic property of the object itself. The Marxian task is to trace the social relations and labour that are condensed into the artifact, not to deny the genuine technical property of kernel-checked derivation.

The evidence is strongest where a solver label or certificate becomes detached from the human and institutional work required to produce and interpret it. LTE supplies an important counter-pattern because its public Blueprint and contributor history make much of that work visible.

### 3.2 Lacan: Big Other and subject-supposed-to-know

The Big Other is not identical to a particular institution or software package. It is the symbolic order through which statements, proofs, credentials and recognized procedures acquire authority.

Lean FRO/Mathlib, Science, Formal Conjectures, journals, repositories and expert communities can function as supports for this symbolic order. A formal solver may be positioned as a subject-supposed-to-know when its output is treated as carrying an authority that exceeds the specific theorem statement it checked.

The analysis must distinguish the actual technical warrant from the symbolic position assigned to the solver.

### 3.3 Žižek: practical belief, fantasy and disavowal

The strongest Žižekian question is not simply why people believe an incorrect proposition. It is how a practice can continue to treat a formal certificate as a guarantee even when the limits of the certificate are known.

The AlphaProof density corrections and the Navier–Stokes paper-to-Lean dispute show that formalization is not a neutral, one-way translation. The statement itself can be revised, challenged or clarified through proof search and expert scrutiny. LTE's definition checks show a visible counter-practice in which semantic scrutiny is built into the formalization process.

The stronger diagnosis of fetishistic disavowal is reserved for cases meeting all three conditions:

1. a constitutive gap is acknowledged;
2. observable practice subordinates that gap to the credential;
3. the subordination has a consequence for recognition, attribution or subsequent action.

A headline, a successful build or the use of Lean alone does not satisfy this threshold.

## 4. Auxiliary frameworks

| Framework | Distinct task | Why it remains auxiliary |
|---|---|---|
| Bourdieu | Field position, symbolic capital, recognition and status conversion | Explains the distribution of recognition better than the fetishistic mechanism itself |
| Merton | Priority, authorship, credit and reward structures | Clarifies scientific attribution and reward without replacing the account of symbolic guarantee |
| Derrida | Archive, trace, iterability, versioning and repeatability | Explains how artifacts are preserved and made retrievable, not why they acquire broader authority |
| Hardwig | Rational epistemic dependence on experts and testimony | Prevents every reliance on formal tools or experts from being misdiagnosed as ideology |
| STS / sociology of proof | Material workflow, maintenance, review and infrastructure | Grounds the empirical account of distributed knowledge production |

Byung-Chul Han is not selected as a core framework. The current cases show visibility and performance metrics, but do not establish the broader psychopolitical mechanisms required for a central Hanian explanation.

## 5. Middle-range model: post-verification circulation

The empirical comparison supports a descriptive model of five distinct circulation modes:

1. **Credentialization:** a proof, solver or formal statement receives status and is represented as a recognized result.
2. **Translation:** the formal artifact is reconstructed as a human-readable mathematical argument or physical interpretation.
3. **Integration:** code, declarations, dependencies or proof artifacts enter another repository, benchmark, library or toolchain.
4. **Assimilation:** the result becomes a premise, method or object in subsequent mathematical research.
5. **Archival stabilization:** version pins, source histories, contributor records, citations and documentation make the artifact repeatable and retrievable.

These are modes, not mandatory sequential stages. Riemann has strong credentialization and translation but no located theorem-level assimilation. Navier–Stokes has strong technical integration while its paper-to-Lean correspondence remains contested. AlphaProof's nine Erdős outputs have formal status without located theorem-level reuse, while its separate quantum-graph result is translated into a human-digested mathematical and physical argument. LTE has strong methodological diffusion without direct reuse of its original proof code.

The model therefore describes the divergence between public recognition, technical reuse and mathematical assimilation.

## 6. Novelty boundary

The proposed contribution is not any of the following:

- the distinction between derivational validity, representational fidelity and epistemic significance (Kallel & El Louadi, 2026);
- distributed human-machine mathematical authorship, provenance governance or understanding audits (López-Corona, 2026);
- software citation, dependency provenance or credit graphs (Druskat, 2019; FORCE11);
- the social certification and assimilation of mathematical proofs (De Millo, Lipton & Perlis; MacKenzie; Rosental);
- formal dependency networks and theorem graphs (Li et al., 2026; Kurgan et al., 2026).

The distinctive contribution is the source-pinned four-case comparison of how recognition, translation, technical integration, methodological diffusion and theorem-level assimilation diverge after formal verification, interpreted through a conditional Marx–Lacan–Žižek account of objectified labour and symbolic guarantee.

No priority claim is made. The next manuscript round should state this contribution narrowly and distinguish direct result reuse from artifact, infrastructure and method reuse.

## 7. Decision for manuscript revision

Retain Marx–Lacan–Žižek as the core framework. Use Bourdieu/Merton, Derrida, Hardwig and STS only for their distinct supporting tasks. Introduce post-verification circulation as an empirical middle-range model rather than a replacement philosophical theory.

The first manuscript revision round changes only the theoretical framework. The case sections, abstract and conclusion remain unchanged until that round is reviewed.


## 8. Empirical calibration of the theoretical roles

The four cases support retaining the selected framework, but they do not support applying every concept uniformly to every case.

| Theoretical resource | Strongest empirical anchor | Calibrated role |
|---|---|---|
| Marx: objectified labour / commodity fetishism | AlphaProof's distributed problem selection, proof search, human statement review, Lean formalization, exposition and repository integration; Navier–Stokes' downstream packaging and benchmarking | Explain how heterogeneous labour can become condensed into a portable proof artifact or solver credential. Do not claim that the artifact literally conceals all labour in every case. |
| Lacan: Big Other / subject-supposed-to-know | Institutional certification and solver attribution in Riemann and AlphaProof; formal status registers and named validation authorities | Explain how institutions and formal systems are positioned as guarantors, and how the solver/certificate is assigned a knowing position. The Big Other is the symbolic locus of authorization, not a person or software system. |
| Žižek: practical belief, fantasy and disavowal | The Navier–Stokes coexistence of explicit paper-to-Lean criticism with continued technical reuse is a possible site for testing; Riemann's ongoing reconstruction and LTE's semantic-audit practices provide counter-patterns | Keep the mechanism conditional. Acknowledged criticism plus continued use is not by itself disavowal. The analysis must show that the acknowledged gap is practically subordinated to the certificate and that this changes judgment, attribution or action. |
| Bourdieu / Merton: symbolic capital, priority and credit | AlphaProof author-contribution statements, solver attribution, Formal Conjectures status transitions, and the separation of original proof authorship from later reconstruction | Explain the conversion of recognition into credit, visibility and field position. |
| Derrida: archive, trace and iterability | Riemann's original/alpoge/main branches, pinned source versions, reconstruction maps, and the versioned Navier–Stokes benchmark | Explain how version selection, preservation and replay make some claims retrievable and authoritative. |
| Hardwig / STS | Expert validation, repository maintenance, audit, porting, review and library infrastructure across all four cases | Establish rational epistemic dependence and the material organization of knowledge production as the baseline against which ideology is diagnosed. |

### Revised theoretical judgment

The empirical record strengthens Marx and Lacan as the structural core and Bourdieu/Merton and Derrida as supporting accounts of recognition and archival stabilization. Žižek remains essential to the paper's distinctive explanatory mechanism, but the cases require a narrower claim: practical belief and disavowal are not presumed from the existence of formal verification, public attention, or continued artifact reuse. They must be demonstrated in a specific episode of acknowledged limitation and consequential reliance.

This means the paper should not argue that all four cases are examples of ideological fetishism to the same degree. They are comparative cases that expose different circulation paths and provide both positive and negative evidence for the proposed mechanism. The Navier–Stokes record supplies a particularly useful test of artifact reuse under acknowledged correspondence criticism; Riemann and LTE show that reconstruction and semantic auditability can remain active rather than being displaced.

The theoretical contribution is therefore a conditional account of how objectified labour and symbolic authorization can produce warrant-scope transfer, with Žižek explaining the practical persistence of that transfer only where the empirical conditions are present.
