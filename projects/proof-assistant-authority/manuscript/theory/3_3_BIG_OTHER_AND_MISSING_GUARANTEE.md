# 3.3 The Big Other and the Missing Guarantee

**Status:** theory-chapter research draft; conceptual distinctions follow Lacan and Žižek and are not claims that software literally occupies a psychoanalytic position.

## 1. The problem of the final guarantor

A formal proof assistant can provide a highly specific guarantee. Lean's kernel checks whether a proof term establishes a formal proposition under specified definitions, axioms, and a trusted computing environment. This is a genuine achievement. Yet the check does not itself guarantee that the formal proposition captures the intended mathematical problem, that the assumptions are appropriate, that the result is significant, or that institutions and public communicators accurately represent what has been established.

The question is therefore not whether a guarantee exists at all. A local technical guarantee plainly exists. The question is whether a society can find a final guarantee that secures the whole chain of knowledge and its own procedures of authorization.

Lacan's formula “there is no Other of the Other” addresses precisely the absence of such a final symbolic guarantor. In Seminar VI, session of 8 April 1959, Chapter XVI, “There Is No Other of the Other,” Lacan states that no signifier in the Other can guarantee the truth or authenticate the signifying chain. In Bruce Fink's 2019 published English translation, the relevant chapter begins at p. 291 and the key passage appears at p. 353. The corresponding French edition gives the passage at p. 108.

The claim does not mean that no institutions, rules, or authorities exist. It means that the symbolic order has no ultimate signifier outside itself that can guarantee its complete consistency.

## 2. The Big Other is not a machine or an institution

In Lacanian theory, the Big Other names the symbolic locus of language, law, norms, and recognition. It cannot be reduced to an empirical person or a particular organization. Žižek explains this distinction in *The Sublime Object of Ideology*: the Big Other is the symbolic order beyond empirical others (1989, pp. 102–105), while the order itself is barred or inconsistent rather than a closed totality (pp. 136–138).

The paper must therefore avoid the formulation “Lean is the Big Other.” Lean is a software system, not the symbolic order. Nor should a university, journal, scientific community, or company simply be identified with the Big Other. Each is an empirical institution that may participate in the symbolic practices through which scientific claims are authorized.

The more precise hypothesis is that Lean can be **positioned as a technical credential within a symbolic order that seeks a guarantee of scientific knowledge**. Its outputs may be invoked as signs that a claim has passed an objective and reproducible procedure. The social meaning of this credential depends on the wider network of experts, institutions, norms, and public communication in which it is embedded.

## 3. The subject-supposed-to-know is a different concept

Lacan's subject-supposed-to-know is developed in Seminar XI, Chapter XVIII, “Of the Subject Who Is Supposed to Know, of the First Dyad, and of the Good,” pp. 230–235 in Alan Sheridan's translation. Lacan states that when a subject-supposed-to-know is posited, transference is established (p. 232). The discussion concerns the analyst's position in the analytic relation and the attribution of knowledge within transference. Lacan also says that the analyst does not present himself as a god and cannot claim absolute knowledge.

This concept is not a generic synonym for trust in experts, institutions, or software. It cannot justify diagnosing ordinary members of the public as being in transference with Lean. At most, it offers a carefully limited analogy for examining how a knowing position is attributed to an expert, institution, or technical credential.

The distinction is important for the paper's argument:
- the **Big Other** concerns the symbolic locus of authority and recognition;
- the **subject-supposed-to-know** concerns a transferential attribution of knowledge to a subject;
- **Lean** is neither of these, but may be represented as a technical sign within a wider symbolic order.

## 4. Why a missing guarantee can still have real effects

The absence of a final guarantor does not dissolve social authority. Social practices continue to rely on credentials, procedures, experts, institutions, and forms of recognition. A scientific result may be accepted because a university announces it, a journal publishes it, a mathematical community discusses it, and a formal checker verifies a proof term. These practices are real and can be rationally warranted.

The Lacanian question concerns the temptation to treat one element in this chain as if it could close the chain from outside. A visible technical procedure can be invested with the role of an ultimate arbiter precisely because it appears to be less dependent on human judgment than ordinary expert testimony. Its reproducibility makes it an attractive candidate for the role of a final guarantee.

But Lean's guarantee remains internal and conditional: it certifies a proof term relative to a formal proposition and environment. It cannot certify the appropriateness of every definition, the intended meaning of the theorem, the empirical relevance of a model, the novelty of a result, or the correctness of all institutional judgments. There is no further Lean theorem that can guarantee, once and for all, that every such relation is correctly established.

## 5. The paradox of technical assurance

The paradox is not that Lean is unreliable. The paradox is that the stronger and more reproducible a local guarantee becomes, the more tempting it may be to treat it as a guarantee of the whole epistemic order.

The Riemann case tests this proposition because extensive independent checking coexists with the absence of a complete human read-through and a conventional explanatory paper at the relevant date. The Navier–Stokes case tests it because kernel acceptance of formal declarations does not settle their correspondence to a separate natural-language proof. The Erdős case tests it in the opposite direction: the published account makes the formal benchmark, human statement validation, and need for expert review relatively visible. The Liquid Tensor case shows how Lean's authority can be embedded in a transparent collaborative network.

## 6. The ideological function of the missing guarantee

Žižek's analysis of the Big Other and fantasy helps explain how a social order can function as if a guarantee existed even though no complete guarantor is available. In *The Sublime Object of Ideology*, the Big Other is not a fully consistent authority; fantasy can function as a screen that fills or conceals the lack in the Other (1989, pp. 136–138). Elsewhere Žižek analyzes how an element that embodies a lack can be perceived as a transcendent guarantee of meaning (pp. 109–110).

Applied to Lean, the hypothesis is that the machine-checked proof can become a visible point at which the social order appears to secure scientific truth. The technical check is real, but the symbolic function may exceed it. The machine is not the missing guarantor; it is one object through which the social order may stage the appearance that such a guarantor is available.

## 7. Provisional thesis

**Lean can acquire symbolic authority not because it is the Big Other, but because it can be positioned as a technical credential within a scientific order that seeks a final guarantor. The Lacanian point is that no such final guarantor exists: the formal check is real and valuable, but its authority remains conditional on semantic, human, and institutional relations that cannot be closed by the kernel itself.**

This argument must not be used to dismiss warranted trust in formal verification. It explains the symbolic function that a genuine technical guarantee may acquire, and it remains open to cases in which public communication preserves the limits of that guarantee.
