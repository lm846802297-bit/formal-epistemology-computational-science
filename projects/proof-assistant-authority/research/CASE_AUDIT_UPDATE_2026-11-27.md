# Case-audit update: new source evidence and corrections (27 November 2026)

**Purpose:** update the four Lean case studies using newly located public materials and exact repository source files. This addendum supersedes earlier statements where noted. It does not claim independent mathematical proof checking; source-level inspection is distinguished from building the repositories or adjudicating the mathematics.

## 1. Riemann hypothesis — correction: a substantial mathematical exposition now exists

### New source

**rh-lean-roadmap**, *The Riemann hypothesis and GRH for Dirichlet L-functions: a readable account of the Lean proof in Alpöge's archive*, version v44, Zenodo, 26 November 2026, DOI 10.5281/zenodo.24562451: https://doi.org/10.5281/zenodo.24562451. Project page: https://rh-lean-roadmap.github.io/rh-lean-roadmap/.

The project supplies a 497-page mathematical main text, 963 pages of longer proofs, a 122-page Lean-declaration index, and a seven-page roadmap. The index links statements to the modules and source lines that prove them. It explicitly says the mathematics is Alpöge's archive while the exposition is written by the roadmap project. Its README states that the organizer set editorial rules and several AI models wrote the text from Lean source and cross-checked it. Sixty-three proofs in Part VIII are marked “Proof (outline)” and point to the Lean declarations containing the complete proof.

### Institutional and technical status

The 21 November joint statement by Lean FRO and the Mathlib Initiative says they have “full confidence” in the proof, certify that both the RH statement and proof are correct, and explain four checks: the Mathlib RH statement was carefully vetted by Lean and number-theory experts; the archive compiles; the formal theorem matches the Mathlib statement under two independent comparison tools; and the exported proof passes several proof checkers, including Lean's kernel and independent implementations. Source: https://leanprover-community.github.io/blog/posts/riemann-hypothesis/.

Andrew Sutherland's MIT report records the detailed checks of the original 17-million-line archive: all 175,187 modules compile; the five headline theorems use only `propext`, `Classical.choice`, and `Quot.sound`; independent kernel/checker replay and statement comparison pass. Source: https://math.mit.edu/~drew/grh/.

The separate compact rewrite is a distinct artifact. Sutherland's 26 November report identifies commit `72fead10` of `lsernau/grh-lean`, 794 files and about 76,000 lines for the compact edition, Lean v4.35.0 and Mathlib commit `56a00585`; both readable and compact editions prove the same five theorem statements and pass the reported checks. Source: https://math.mit.edu/~drew/shortgrh/.

### Required correction to previous project wording

Earlier notes said there was “no human-readable mathematical paper” or “no human-readable argument.” That is now outdated and must not be repeated without qualification. A substantial readable mathematical exposition exists as of 26 November. However, it was written by several AI models from the Lean source and cross-checked, not presented as a conventional independently authored mathematical paper or a complete human read-through of the original archive. The Lean FRO/Mathlib joint statement is a genuine expert-community certification of the formal statement and proof, not merely a machine-only report. It also says that further mathematical activity is expected to explain the new ideas.

### Updated philosophical reading

- **Fantasy:** the combination of a formal certificate, community certification, and a 1,582-page exposition can make the proof appear fully settled and accessible. The analysis must distinguish the different kinds of certification and authorship.
- **Fetishism:** a headline may attribute the result to Claude/Lean, while the actual network includes Alpöge, Mathlib, Lean FRO, the roadmap team, AI exposition models, checker authors, and expert number theorists. The new exposition makes this distributed network more visible, not less.
- **Big Other:** the Lean FRO/Mathlib joint statement is an institutional act of authorization. It is not a final guarantee of every mathematical interpretation or social consequence. The case now shows a layered symbolic authority rather than simply “machine proof without human exposition.”
- **Counter-evidence:** explicit technical reports, community certification, source-linked exposition, and the disclosure of AI-written explanatory text all resist the claim that machine authority is wholly autonomous or that the proof remains inaccessible.

**Updated use:** a case of strong machine verification plus expert-community certification and AI-mediated exposition. It is especially useful for studying how institutional endorsement and explanatory media combine to make a technical result socially legible.

## 2. Navier–Stokes — exact source-level confirmation of two mismatches

### Primary critique

A. Bastounis, F. Circelli, and A. C. Hansen, “Navier–Stokes Lost in Translation: Why Lean Verification of AI Autoformalisation Does Not Guarantee Correct Natural Language Proofs,” arXiv:2610.08144v1 (6 October 2026): https://arxiv.org/abs/2610.08144.

The authors explicitly distinguish (i) compiling a Lean proof of a statement from (ii) faithfully translating an entire natural-language mathematical text. Their claim is about the correspondence of the published OpenAI paper and the Lean artifacts, not about a failure of Lean's kernel and not a proof that the underlying Navier–Stokes theorem is false. The authors expressly disclaim claims about the correctness of OpenAI's natural-language proof.

### Mismatch A: inverse estimate

The critique compares OpenAI's natural-language paper, Lemma 8.6, equation (8.19), with the Lean declaration `norm_derivativeWord_inverse_le` in `NavierStokes/SmoothFamilyTorusInverse.lean`, at OpenAI repository commit `f9e8bc5b38b6e212696e8a30e3e91517af887bbd` (paper pp. 4–7; source lines 1059–1080).

- Natural-language paper: an output estimate with (m) torus derivatives requires (m+4) input derivatives.
- Lean declaration: the hypotheses require `w.length + 5` derivatives to control the corresponding derivative word.
- The critique explains the difference through the summability estimate used: the natural-language proof uses a convergent two-dimensional series with exponent 3, whereas the Lean code uses a series with exponent 4, producing the extra derivative.

The source file at the pinned commit was fetched and the theorem's two hypotheses explicitly contain `w.length + 5`. This independently confirms the code-side fact reported by the critique. It does not independently adjudicate whether the natural-language (m+4) estimate is mathematically valid.

### Mismatch B: pressure-flux estimate

The critique compares natural-language equation (10.19) with `exists_uniform_actual_pressure_flux_bound` in `NavierStokes/R3/PressureFlux.lean`, at the same repository commit (paper pp. 8–11; declaration line 576).

- Natural-language bound: expressed in terms of the localized velocity quantity (B_R), with a factor of the form ((B_R+1)B_R^{1/2}/R) plus the (R^{-3/4}B_R^{3/4}) term.
- Lean bound: includes the additional localized gradient quantity (A_R), a factor ((B_R^{1/2}+1)(A_R/R+1/R^2)), and an (R^{-7/4}B_R^{3/4}) term.
- The proofs also use different decompositions and estimates (Riesz-transform/Sobolev route versus the natural-language approach).

The critique says these bounds are difficult to compare directly; it notes that the Lean bound is ultimately used in a proof where the relevant difference (w) is shown to vanish, so the final role of the estimate must be read in the full Lemma 10.5 argument. Therefore do not summarize this as “Lean proves a false bound” or as a simple numerical weakening. The precise conclusion is that the Lean declaration is not a line-by-line faithful formalization of the stated natural-language estimate and proof strategy.

### Updated philosophical reading

Navier–Stokes remains the strongest candidate for examining the ideological enlargement of a technical credential, but the claim must be precise: a valid Lean proof of formal declarations cannot, by itself, certify that those declarations are a faithful translation of every statement and argument in the separate natural-language paper. The source-level mismatch is now confirmed in the exact pinned files. This supports analysis of semantic mediation being displaced by the machine credential; it does not establish intentional concealment or cynical disavowal.

## 3. Erdős / AlphaProof Nexus — source-level audit reveals specific artifact mismatches

### Scope and method

The *Science* paper reports nine results among 353 formalized Erdős statements and 44 among 492 OEIS conjectures. It says that experts checked the correspondence between each solved Lean statement and the original question. The primary repository is `google-deepmind/alphaproof-nexus-results`, commit `42f344cfa9d57154f36e6b9bef1f71760a438c54` (the result files were added on 19 May 2026). The paper's preprint v2 is arXiv:2605.22763v2.

The following specific discrepancies are documented by the Erdős Problems research library (updated 13 October 2026), which read the relevant preprint pages and Lean files statically but did not build the files or claim independent mathematical review: https://erdosproblems.ai/wiki/library/additive_combinatorics/tsoukalas_2026_advancing_mathematics_research_ai_driven_formal_proof_search.

### Erdős #125 — linked variant and original forum artifact

The paper links `erdos_125.variants.positive_lower_density.lean` as the Lean proof of the statement that the sum of the base-3 and base-4 digit sets has lower density zero. The exact file exists at the cited AlphaProof results commit and its `target_theorem_0` proves `answer(False) ↔ 0 < (A + B).lowerDensity`, which corresponds to the claimed negative answer to positive lower density. The independent library notes that the proof first posted in the March 2026 erdosproblems.com thread is a different Lean file with different lemmas. Thus the linked artifact is a formal proof of the relevant statement, but not the same file as the original forum proof. Source: https://erdosproblems.ai/wiki/library/additive_combinatorics/tsoukalas_2026_advancing_mathematics_research_ai_driven_formal_proof_search/erdos_125.

### Erdős #26 variant — top-level target differs, but an auxiliary lemma proves the prose claim

The paper's prose proof (Appendix B.4, pp. 38–40) gives a sequence whose shifted multiples have upper density below 3/4 for every shift. The linked Lean file `erdos_26.variants.tenenbaum.lean` at the results commit has a top-level `target_theorem_0` that formalizes the negation of a Tenenbaum variant using lower density below 1/2, so its target statement is not identical to the prose theorem.

However, source inspection also finds an auxiliary lemma `multiples_card_bound` proving a uniform pointwise count bound of at most 37/90·X for every shift and every X, together with the constructed sequence's strict monotonicity and divergent reciprocal sum. This pointwise bound is stronger than the prose upper-density bound below 3/4 and is sufficient to establish the prose claim. Therefore this is a mismatch in the top-level formal target, but not evidence that the file fails to contain a proof of the prose result. We must not call it a failed formalization.

### Erdős #741(i) and #741(ii) — two linked-file mismatches

The paper's prose states the upper-density theorem for part (i): if A+A has positive upper density, then A splits into two parts whose sumsets both have positive upper density. The Lean file linked for part (i), `erdos_741.parts.i.lean` at the AlphaProof results commit, instead proves `answer(False)` for the exact-density reading using `HasPosDensity`, where the natural density must exist and be positive. Its counterexample is the exact-density variant later named `erdos_741.variants.exact_density`.

The correct upper-density theorem exists in the upstream Formal Conjectures file as `erdos_741.variants.upper` at commit `9d492049e42167b0d2fd58a9e91da3bf160172b5`. The AlphaProof results repository's linked file is the exact-density counterexample, not this upper-density theorem.

For part (ii), the preprint's Appendix B.4 explicitly links `erdos_12.parts.ii.lean` (arXiv:2605.22763v2, pp. 37–38), a file for Problem 12 rather than Problem 741. The Problem 741 page identifies this as a wrong-file link. The appropriate Problem 741 part (ii) proof is in the mo271/formal-conjectures fork at commit `486bc8afae062b6711cd16d3466d651ee2880a52`; the upstream Formal Conjectures file at commit `9d259649abe0b02d7a25f7589b872db679b35e21` records the theorem and points to that proof.

Thus the two #741 links in the preprint appendix are problematic, but the appropriate formal proofs exist elsewhere. This is a source-citation/provenance problem, not evidence that no proof exists.
### Significance for the case

These are not kernel failures: the files may be valid Lean proofs of the formal statements they encode. They are problems of artifact-to-claim correspondence and publication provenance. The paper's claim of expert statement validation and the repository's linked files must therefore be evaluated separately. The independent library is a secondary source with explicit limits: it read the preprint v2 and code statically, did not build the proofs, and did not claim specialist adjudication. We have independently fetched the cited #125, #26, and #741(i) files at the pinned commit and confirmed their target theorem statements at source level, but have not rebuilt them.

### Updated philosophical reading

AlphaProof is no longer a simple clean counter-case of transparent human mediation. The paper describes a human validation step, but the linked artifacts show that the public evidence chain can still contain statement/version mismatches. This makes the case highly relevant to epistemic fetishism: the public label “Lean-verified” may conceal the need to check whether the exact Lean file attached to a published claim proves the exact prose theorem. The case also illustrates why institutional peer review and public audit are separate layers.

## 4. Liquid Tensor Experiment — stronger counter-case through explicit semantic safeguards

The 15 July 2022 completion announcement states the theorem and lists mathematical, formalization, technical, library, and institutional contributors. More importantly, Adam Topaz's 14 October 2022 post explicitly raises the semantic problem: how can the community be confident that the definitions introduced in Lean are correct? It gives examples of pathological possibilities (for example, defining `Ext` to be zero) and explains that the project built a readable `examples` folder as sanity checks so mathematicians with limited Lean experience could inspect the definitions and gain reasonable confidence in the formal statement.

Sources: https://leanprover-community.github.io/blog/posts/lte-final/ and https://leanprover-community.github.io/blog/posts/lte-examples/.

This makes Liquid Tensor a stronger counter-case than previously described. It does not merely credit collective labour; it explicitly makes the semantic validity of the formal definitions a public object of scrutiny and constructs supporting checks to help non-Lean mathematicians evaluate them. The case can test whether visible semantic mediation resists the appearance of autonomous machine authority.

## 5. Cross-case revision

| Case | New finding | Revised role in theory test |
|---|---|---|
| Riemann | Expert-community certification plus a 1,582-page AI-written exposition now exists | Tests how machine verification, institutional endorsement, and AI-mediated explanation combine; no longer described as lacking a readable account |
| Navier–Stokes | Exact source-level m+4/m+5 and pressure-flux discrepancies are confirmed in pinned Lean files | Strongest case for the gap between kernel validity and faithful correspondence to a separate written proof |
| Erdős | #26 and #741(i) linked Lean artifacts do not exactly match their prose theorem statements; #125 linked file matches a variant but differs from original forum file | Strong case for artifact provenance and scope control; no longer a clean transparency counter-case |
| Liquid Tensor | Project explicitly built definition sanity checks to address semantic validity for mathematicians | Strong counter-case showing formal verification can be embedded in visible human semantic scrutiny |

## 6. Inference limits

1. None of the discrepancies establishes that Lean's kernel accepted an invalid proof.
2. None of the Navier–Stokes discrepancies alone proves the underlying PDE theorem false.
3. The AlphaProof discrepancies concern the exact correspondence between prose claims and cited artifacts; they do not establish that all nine results are invalid or that no correct Lean proof exists elsewhere.
4. The Riemann exposition is AI-written and cross-checked; it is a readable mathematical account, not by itself evidence of independent human mathematical acceptance of every argument.
5. Public texts establish representations and institutional acts, not population-level public belief or unconscious motives.
6. Cynical ideology remains unestablished. The current evidence supports analysis of fantasy, fetishistic representation, and symbolic authorization, but not a claim of deliberate disavowal.