# Analytical test: cynical versus fetishistic disavowal in machine verification

**Project:** *In Lean We Trust? The Ideology of Machine-Checked Proofs in Science*  
**Date:** 27 November 2026  
**Status:** operational research memo based on Jack Black (2025); not a finding that any case already exhibits disavowal.

## 1. Why the distinction matters

The paper studies a possible situation in which actors know that Lean verifies a formal proposition under specified assumptions, yet a public or institutional practice continues to invest the phrase “Lean-verified” with a wider guarantee. It would be imprecise to label every such case “cynical ideology.”

Jack Black (2025), “Examining the Mechanism of Disavowal and Its Two Forms: Cynical Disavowal and Fetishistic Disavowal,” *Theory & Psychology* 35(1), 117–135, DOI 10.1177/09593543241308199, argues that cynical and fetishistic disavowal should be distinguished. Cynical disavowal involves a manipulative distance and obscuring the gap between belief and action. Fetishistic disavowal can acknowledge the objective state of affairs while maintaining the fetishistic attachment that manages the lack in the Other.

## 2. Working distinction for this project

### Cynical disavowal

An actor or institution explicitly recognizes that the Lean check is limited, but strategically maintains a broader public claim or practice while keeping a knowing distance from the overstatement.

**Minimum evidence required:**
1. A clearly attributable statement acknowledging the exact verification limit.
2. A later or contemporaneous statement/practice by the same actor or institution that exceeds that limit.
3. Evidence that the discrepancy is not simply corrected by surrounding context, a headline/body distinction, or an ordinary compression.
4. A reason to attribute the two statements to a connected communicative practice; otherwise code only an inconsistency in the public record, not cynical intent.

### Fetishistic disavowal

An actor may openly know that Lean checks only a formal proposition and that semantic, empirical, or institutional questions remain, while still treating the formal-verification credential as the object through which a broader sense of certainty is sustained. The limitation is not necessarily hidden; the fetish object helps manage or cover the lack despite acknowledged knowledge.

**Minimum evidence required:**
1. Explicit recognition of the relevant limitation.
2. Continued practical or symbolic investment in Lean as a broader guarantee.
3. Evidence that the investment persists even when the limitation is available and understood within the same discourse or institutional practice.
4. A demonstrated displacement of the need for semantic or collective judgment onto the technical credential.

This is the more promising hypothesis for the paper's central claim, but it remains difficult to establish from public texts alone. Audience research or interviews would be needed to establish how readers themselves understand and use the credential.

## 3. Do not confuse disavowal with ordinary justified reliance

A researcher may state that Lean does not establish empirical adequacy and still appropriately rely on Lean for the formal theorem it checks. This is not disavowal. Nor is it fetishism simply because the machine is trusted.

The key question is whether the formal credential is asked to do more symbolic work than its technical warrant supports. If public communication accurately confines the claim to the formal proposition and makes the human semantic bridge explicit, code it as warranted reliance or transparent mediation.

## 4. Application to the four cases

| Case | Evidence relevant to disavowal | Current status |
|---|---|---|
| Riemann | FRO/Mathlib certification, public scope statements, AI-authored exposition, and continuing references to the result as a solution | No cynical disavowal established; test whether the formal credential is fetishistically invested despite explicit distinctions among certification, exposition, and broader acceptance |
| Navier–Stokes | OpenAI announcement and Lean release; independent critique identifies formal-to-natural-language mismatches; later public responses acknowledge the mismatch | Acknowledged limitation plus continued claim requires exact actor-level timeline; no cynical intent inferred. Strong candidate for studying fetishistic persistence of the Lean credential |
| Erdős | *Science* paper reports expert statement validation; exact linked files for #26/#741 differ in target or provenance, while auxiliary lemmas/correct proofs exist elsewhere | Current evidence supports artifact-provenance scrutiny, not cynical disavowal. Test whether the institutional “Lean proof” label obscures exact file/claim relation |
| Liquid Tensor | Explicit public attention to definition correctness and readable sanity-check examples | Counter-case: visible semantic validation weakens the claim that the machine credential disavows its conditions |

## 5. Coding outcomes

Use one of five codes for each text/event:

- `WARRANTED_SCOPE`: statement accurately describes what Lean checks.
- `TRANSPARENT_MEDIATION`: statement identifies relevant human, semantic, and institutional work.
- `SCOPE_ENLARGEMENT`: statement makes a broader claim than the formal artifact alone warrants, without sufficient context.
- `FETISHISTIC_DISAVOWAL_CANDIDATE`: explicit awareness of limits coexists with sustained symbolic investment in a broader guarantee.
- `CYNICAL_DISAVOWAL_CANDIDATE`: evidence suggests a knowing, strategic gap between acknowledged limits and continued overextended practice.

These are analytic codes, not psychological diagnoses. `CANDIDATE` is intentional: public evidence may justify a hypothesis but not a conclusion about unconscious motives.

## 6. Consequence for the paper

The central concept remains **the ideological fetishism of formal verification**. Cynical disavowal is not a required mechanism and should not be forced onto any case. Fetishistic disavowal may better explain how the technical credential retains symbolic force even when its limits are openly acknowledged. Black (2025) provides a useful refinement, but the paper's overall theoretical framework remains Žižek's critique of ideology.