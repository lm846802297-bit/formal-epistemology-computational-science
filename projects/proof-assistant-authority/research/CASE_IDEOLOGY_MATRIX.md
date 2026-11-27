# Ideological-mechanism matrix for the four cases

**Project:** *In Lean We Trust? The Ideology of Machine-Checked Proofs in Science*  
**Cut-off:** 27 November 2026  
**Status:** provisional interpretive coding. “Supported” means that public materials make a mechanism analytically plausible, not that an unconscious process has been empirically demonstrated.

## 1. Coding principles

The three Žižekian concepts are not synonyms:
- **Ideological fantasy:** a narrative or practice that stages a guarantee of certainty and organizes how subjects relate to an otherwise difficult or inconsistent social reality.
- **Fetishism:** a social relation or collective process appears as an autonomous property of an object. In this project, ask whether collective epistemic labour appears as machine-owned certainty.
- **Cynical ideology/disavowal:** known limitations coexist with a practice that continues to reproduce the authority or fantasy. Evidence must establish both awareness and continued practical reliance; mere presence of a caveat is insufficient.

Do not label every trust relation ideological. A scope-preserving public statement, a correctly checked theorem, or rational deference to experts can be epistemically justified.

## 2. Case matrix

| Case | Ideological fantasy | Epistemic fetishism | Cynical ideology | Counter-evidence / alternative |
|---|---|---|---|---|
| Riemann — Claude + Lean | Plausible: the image of machine certification as a visible guarantee for a historically unresolved problem | Possible: “Claude/Lean solved RH” can compress a large human-machine and institutional process into machine agency | Not established: experts publicly state the limits and call for human understanding; no evidence that audiences knowingly ignore them in practice | Multiple independent proof checkers provide real technical assurance; named mathematicians, formalization contributors, and Mathlib/Lean institutions remain visible in parts of the coverage |
| Waring — GPT-6.2 Astra | Plausible but weak: AI authorship and AI self-refereeing may stage an autonomous knowledge-production loop | Possible: the AI is presented as both producer and referee, while authors' rewriting and disciplinary expertise can recede | Not established: no evidence that authors or readers knowingly disavow the lack of independent review | Authors explicitly disclose the AI role and their rewriting; the preprint is visibly unreviewed, and the claim has not been established by an external certificate |
| Navier–Stokes — OpenAI + Lean | Strong analytical candidate: the public “AI proof + Lean verification” narrative can suggest a final guarantee of a Millennium-level claim | Strongest candidate: the authority of the formal system can stand in for semantic correspondence between Lean declarations and the separate natural-language paper | Not established: the mismatch is publicly debated and OpenAI acknowledges it; evidence of continued knowingly inflated reliance would still be needed | The Lean kernel may validly check its formal statements; the independent critique is about non-faithful translation and weaker/different estimates, not a kernel failure or a refutation of the theorem |
| Erdős — AlphaProof Nexus | Possible: the “AI solves open Erdős problems” narrative can symbolize autonomous mathematical discovery | Limited / mixed: proof-search labour is distributed across LLMs, Lean, formal statement repositories, and expert validation | Not established | The *Science* paper discloses denominators, human statement checks, and the need for expert review; independent audit qualifies novelty and statement history |

## 3. Detailed provisional judgments

### 3.1 Riemann hypothesis

The public object of trust is not simply Claude. It includes the Lean kernel, Mathlib's formal statement, independent proof checkers, MIT and Waterloo checking, and the human mathematician who directed and interpreted the work. Public experts explicitly distinguish successful compilation from semantic identification with RH and from human understanding of the proof.

**Best current interpretation:** a real formal certification becomes a highly visible symbol of mathematical certainty, while expert discourse simultaneously resists treating it as equivalent to complete human understanding. The case is useful for studying the coexistence of technical confidence and conceptual opacity. It does not yet support a claim that the public blindly transfers authority to AI.

### 3.2 Waring's problem

The paper states that GPT-6.2 Astra carried out the work, that the authors rewrote it, and that GPT-6.2 Astra refereed it. This creates an unusual public attribution loop. The main issue is not machine verification; no Lean certificate or independent review is documented at the cut-off.

**Best current interpretation:** a test case for the social representation of AI as both producer and evaluator of knowledge. The “AI refereed AI” description can be read as a fantasy of autonomous self-validation, but the preprint status and explicit disclosure may also make the lack of external authority visible. Public reception is still too thin to infer a social effect.

### 3.3 Navier–Stokes

The repository metadata says the formalization is complete for its declared statements and self-assessed. Bastounis, Circelli, and Hansen identify differences between some natural-language estimates and Lean declarations. Their critique explicitly does not decide whether the natural-language proof or underlying result is correct.

**Best current interpretation:** the strongest case for fetishism as a *representational structure*: a valid formal proof can be used as a visible token of authority even though a further semantic bridge is required to show that it certifies the claims in a separate paper. This is not a claim that OpenAI or the public knowingly disavows the mismatch. The critical object is the public/institutional relation between formal validity and source-text correspondence.

### 3.4 Erdős / AlphaProof Nexus

The paper reports 9 of 353 formalized Erdős statements and 44 of 492 OEIS conjectures, describes human validation of the formal statements, and explicitly says expert review remains necessary for informal AI proofs. A public expert panel and an independent secondary audit add qualifications about cost, statement history, and novelty.

**Best current interpretation:** a counter-case to the strongest fetishism thesis. The research account makes the division of labour visible and treats formal verification as a filter for human review. Questions remain about how media headlines compress denominators and formalized subsets, but the primary paper itself is comparatively explicit.

## 4. Cross-case result

The cases do not support one uniform mechanism. The provisional pattern is:
- Riemann: strong technical guarantee, mixed public interpretation, explicit human-expertise mediation.
- Waring: AI self-attribution and self-refereeing without external proof certification.
- Navier–Stokes: formal correctness and semantic correspondence become visibly separable.
- Erdős: formal search and checking are embedded in a disclosed human-AI research workflow.

The strongest general hypothesis is therefore not “society trusts the machine.” It is:

**Machine verification can become a symbolic credential within a broader social order of scientific authority; whether this credential becomes fetishized depends on whether the human, semantic, and institutional conditions of its relevance remain visible.**

## 5. What would be needed to support cynical ideology?

For any case, a cynical-ideology claim would require evidence of:
1. a relevant actor or institution explicitly acknowledging the limitation;
2. continued communication or institutional practice that relies on a stronger guarantee;
3. a reason to think this is more than ordinary shorthand, a temporary simplification, or an accurate statement whose qualifications appear elsewhere.

Public texts can establish the coexistence of qualification and practice, but not unconscious motives. To make claims about public audiences knowingly disregarding limitations, reader interviews or experiments would be needed.
