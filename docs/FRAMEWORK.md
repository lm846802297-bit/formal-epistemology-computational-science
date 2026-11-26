# A Warrant Architecture for Formalized Physics (v0.1)

For formal system F, assumptions A, and proposition phi, a proof assistant checks:
$$ A \vdash_F \varphi. $$
Subject to soundness of F and its trust base, this establishes a formal consequence of A. It does not alone establish that A captures the intended physical theory, that phi has the intended interpretation, or that a model describes an actual target:
$$ A \vdash_F \varphi \quad\not\Rightarrow\quad W \models \varphi. $$

## Claim types
- **C_F — formal:** derivability in a specified system.
- **C_M — model-internal:** the interpreted proposition holds in a specified model. Transfer from C_F requires theorem correspondence, full hypothesis instantiation, and correct interpretation.
- **C_W — target-world:** a claim is warranted for a physical target and domain. It requires a purpose-sensitive model-to-target relation and appropriate evidence.
- **C_E — explanatory:** the result is explained, not merely established; this may require proof tracking and explanatory correspondence.

## Two tracks
**Deductive:** informal statement -> theorem correspondence -> formal proposition/assumptions -> kernel-checked proof -> interpreted model-internal claim.

**Model/evidence:** target/domain -> observation, experiment, prior theory -> model construction -> validation/inferential assessment -> model-to-target warrant.

The tracks may converge on a warranted physical claim. Their warrants are not interchangeable; their conjunction is not assumed universally sufficient.

## Conditional audit schema
$$ V_F \land C_T \land A_M \land I_M \land R_{MW}(D) \land E_D $$
Here V_F is formal validity; C_T adequate theorem correspondence; A_M satisfaction of all hypotheses by model M; I_M correct interpretation in M; R_MW(D) a justified model-target relation for purpose/domain D; E_D domain-appropriate evidence. This is diagnostic, not a theorem or universal sufficient condition.

## Relation to prior work
DeDeo and Duede (2026) develop correspondence and proof tracking. Meadows et al. (2026) study semantic drift in physics autoformalization. The candidate extension begins after adequate formalization: interpretation of physical structures, instantiation of theorem hypotheses, and transfer from model-internal results to target-world claims. Knuuttila's artifactual account cautions against requiring every model to literally represent a target.

## Open questions
1. Is theorem correspondence distinct from physical interpretation?
2. Which model-target relations fit idealized theoretical physics?
3. When can a theorem about a formal model count as scientific knowledge without direct empirical testing?
4. Does proof tracking support truth-warrant, explanatory warrant, or both?
5. How should imported libraries, typeclass assumptions, and foundational axioms enter the audit?
6. Can a claim-to-evidence ledger aid judgment without mechanizing it?