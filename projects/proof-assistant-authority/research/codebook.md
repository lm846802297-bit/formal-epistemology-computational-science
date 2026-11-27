# Coding guide for the Lean-focused study

Every record must preserve exact public wording, source artifact, locator, date/version, Lean theorem/definition/hypotheses, review status, and reason for classification.

## 1. Claim-scope code
- **Accurate:** explicit claim is supported by the cited Lean artifact and does not imply a broader target.
- **Reasonable compression:** details omitted but surrounding context preserves intended scope or sufficient qualification.
- **Ambiguous:** materially different readings remain possible or relevant evidence is missing.
- **Substantive scope expansion:** claim attributes a stronger conclusion to Lean verification than the formal artifact and documented semantic bridge establish. Identify the exact missing inferential link.

## 2. AI and human contribution code
Record whether AI:
1. proposed a conjecture;
2. found a proof strategy or key lemma;
3. generated a natural-language proof;
4. generated a Lean proof;
5. translated a natural-language proof into Lean;
6. searched or verified an existing Lean proof;
7. worked in a human-AI collaborative workflow.

Separately record human tasks: problem selection, theorem formulation, formalization design, proof repair, semantic validation, mathematical interpretation, review, and communication.

## 3. Lean verification dimensions
Code separately:
- formal theorem statement and namespace;
- definitions, imported libraries, axioms, and assumptions;
- kernel/build acceptance;
- use of admitted placeholders or additional axioms;
- reproducibility and pinned commit;
- independent proof-term checker or comparator results;
- semantic correspondence to the intended mathematical claim;
- human mathematical understanding and exposition;
- peer review and institutional recognition.

Never collapse these into one “Lean verified” binary.

## 4. Public framing and reception
For each media or public-discussion text, code:
- authority source emphasized: Lean/kernel, AI model, named mathematician, research team, university, company, journal, mathematical community;
- certainty frame: claim, breakthrough, proof, solved, certified, accepted, still under review;
- human-labour visibility: foregrounded, backgrounded, omitted, explicitly acknowledged;
- public interpretation: awe/excitement, trust, scepticism, anxiety, institutional distrust, confusion about formal checking, distinction between checking and understanding, or other;
- source type: representative survey, expert interview, institutional announcement, professional media, general media, self-selected online discussion.

## 5. Rival explanations
Record ordinary shorthand, genre conventions, legitimate reliance on expert testimony, explicit qualifications elsewhere, institutional reputation, audience literacy, and ambiguity. Strong wording is not automatically distortion.

## 6. Inference limits
- Public texts establish representations and invitations to trust, not actual belief.
- Self-selected online posts establish that an interpretation exists, not its prevalence.
- General trust surveys establish background attitudes, not causal effects of a Lean announcement.
- No unconscious motive, transference, or ideological attachment may be attributed to an individual from wording alone.
- Ideological analysis requires repeated relations among public claims, practices, and institutions, not isolated rhetoric.
