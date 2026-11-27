# Detailed analysis of Chen & Jia (2026): public trust and AI disclosure

**Project:** *In Lean We Trust? The Ideology of Machine-Checked Proofs in Science*  
**Source:** Catherine Chen and Xinle Jia, “When researchers use AI: public trust, ethical judgments, and the perceived value of academic research,” *AI and Ethics* 6 (2026), article 223. Published 26 March 2026. DOI: https://doi.org/10.1007/s43681-026-01039-w  
**Evidence cut-off:** 27 November 2026  
**Status:** full article inspected; OSF preregistration and replication repository identified. This memo reports the article's design and findings; raw-data reanalysis is not yet performed.

## 1. Research question and design

Chen and Jia ask how disclosure of generative-AI use in academic research affects public evaluations of researchers and their work. Their preregistered experiment recruited 806 participants through Prolific. Quota sampling was used to reflect the U.S. population's demographic composition for gender, age, and ethnicity. Participants were randomly assigned to one of six disclosure conditions. They were not shown an actual research paper; they read a scenario describing an academic paper and its authors' AI-use statement.

The six conditions were:

| Condition | N | Disclosed contribution |
|---|---:|---|
| No AI | 126 | Authors conducted research without generative AI |
| Language polishing | 128 | AI assisted with language polishing |
| Language polishing + clarification | 150 | AI polished language; theoretical framing, hypotheses, analyses, and interpretation were entirely human |
| Theoretical assistance | 120 | AI helped with framing, literature review, and hypothesis generation; methods and coding were human |
| Methodological assistance | 148 | AI helped with statistical analyses and coding; theory and hypotheses were human |
| Both theoretical + methodological | 134 | AI helped with both intellectual/theoretical and methodological tasks |

The experiment distinguishes disclosure of AI involvement in intellectual work from disclosure of AI involvement in methodological work. It also tests whether clarifying retained human intellectual contribution changes perceptions.

## 2. Outcomes measured

The study measured ten outcomes on normalized 0–1 scales:
- trust in the researchers;
- trust in the findings;
- perceived researcher skillfulness;
- perceived research quality;
- interest in the research;
- perceived importance;
- perceived usefulness;
- willingness to share;
- perceived ethicality;
- perceived transparency.

This is important for our project: trust in the researcher and trust in the findings are separate outcomes. The paper does not treat “trust in science” as a single undifferentiated variable.

## 3. Main findings

### 3.1 Human-only versus extensive AI involvement

The No-AI condition had the highest mean on all ten outcomes. The Both-Assistance condition had the lowest mean on the eight outcomes for which directional hypotheses were specified, and also the lowest mean perceived ethicality. Table 1 reports the adjusted OLS contrasts:
- No-AI relative to other groups: coefficients of +0.11 to +0.24 across outcomes, all statistically significant (p<.01 or p<.001).
- Both-Assistance relative to other groups: coefficients of -0.10 to -0.20 across outcomes, with perceived transparency the exception to the “lowest mean” pattern.

This supports a broad public penalty for disclosure of extensive AI involvement. It does not show that people reject AI in all scientific roles.

### 3.2 Theoretical versus methodological assistance

The methodological-assistance group had numerically higher means than the theoretical-assistance group on all eight directional outcomes, but none of those eight differences was statistically significant. Effect sizes were small (Cohen's d approximately 0.03–0.22). Trust in researchers approached but did not reach conventional significance (B=0.06, t=1.92, p=.06).

Perceived ethicality also did not differ significantly between the two groups (B=0.06, p=.10). Perceived transparency was higher in the methodological condition (B=0.07, t=2.21, p=.03).

**Interpretation:** the study does not establish a robust general preference for methodological AI over theoretical AI on trust and quality outcomes. It does show a transparency difference. The abstract's broad statement that respondents were “more positive” about methodological use should be read alongside these nonsignificant outcome-by-outcome contrasts.

### 3.3 Human-contribution clarification

Adding an explicit statement that the authors retained responsibility for theory, hypotheses, analyses, and interpretation improved several outcomes relative to the language-polishing-only disclosure. It increased trust, perceived skillfulness, perceived quality, interest, usefulness, willingness to share, ethicality, and transparency in specified comparisons. The clarification did not uniformly erase the AI-use penalty; the No-AI condition remained higher on some measures.

This is highly relevant to our project: the visibility of human intellectual labour and accountability can affect public evaluations. However, the manipulation concerns a textual disclosure, not an independently verified account of who actually did the work.

### 3.4 AI experience and general trust in science

The interaction between AI-use frequency and disclosure condition was positive for all ten outcomes; six interactions reached statistical significance (trust in researchers, interest, importance, willingness to share, perceived ethicality, and transparency), and two were marginal (quality and usefulness). The authors say H5 was partially supported.

Self-reported AI knowledge and general trust in science did not significantly moderate the effects. The moderation pattern should not be simplified to “frequent users always trust AI more”: the authors report that formal comparisons between “very” and “extremely” frequent users were nonsignificant, with very small cells in the extremely frequent category (e.g. N=16 in the No-AI condition and N=9 in the Both-Assistance condition).

## 4. What the experiment establishes

The random assignment supports a causal inference about the effect of the *disclosure wording* on participants' immediate evaluations in this scenario. In particular:
1. AI involvement in both theoretical and methodological tasks reduces evaluations relative to a no-AI description.
2. Explicitly preserving human intellectual responsibility improves evaluations relative to a bare language-polishing disclosure.
3. The data do not establish a statistically robust trust penalty for theoretical assistance relative to methodological assistance across the eight main outcomes.
4. Personal AI-use frequency moderates some responses; self-reported AI knowledge and general trust in science do not.

## 5. What it does not establish

- It does not study Lean, Coq, formal verification, proof assistants, or machine-checked mathematical claims.
- It does not compare a machine-verified AI proof with an unverified AI proof.
- Participants did not read an actual paper or inspect any evidence about a real research team's contribution.
- The sample is a quota-based Prolific online sample designed to match selected U.S. demographics; it is not a probability sample of the entire U.S. public, and still less a global public sample.
- The study measures immediate self-reported perceptions, not long-term trust, actual acceptance of scientific findings, or behavior.
- It cannot establish that machine verification increases or decreases public trust.
- It cannot establish ideological fantasy, fetishism, or cynical disavowal.

## 6. Implications for *In Lean We Trust?*

The most useful finding is not simply “the public distrusts AI.” It is that public evaluation is sensitive to **where AI enters the knowledge-production chain** and whether human intellectual contribution and accountability remain visible.

This suggests a distinction among:
- AI as a language editor;
- AI as a methodological assistant;
- AI as a generator of theoretical framing or hypotheses;
- AI as a producer of a proof or result;
- a proof assistant as a verifier of a formal proposition;
- experts and institutions as assessors of semantic correspondence and significance.

The Chen–Jia experiment manipulates the first four categories only in broad research-disclosure form. Our four mathematical cases make the latter two categories visible. A direct bridge between the two literatures is therefore a research hypothesis, not an established finding.

## 7. Relation to Žižek and Hardwig

Hardwig explains why a non-expert can rationally rely on expert testimony and collective epistemic labour without personally checking every proof. Chen–Jia adds evidence that audiences evaluate the credibility of this labour partly through representations of who contributed intellectually and who remains accountable.

A Žižekian account could add an analysis of how the social product of this labour is represented: does the public account make the machine appear as an autonomous source of knowledge, or does it preserve the network of human and institutional mediation? But the experiment itself does not measure unconscious investment in an authority, ideological fantasy, or fetishism.

## 8. Reproducibility materials

- Preregistration and data/code repository: https://osf.io/grxv3
- Article: https://doi.org/10.1007/s43681-026-01039-w

A later quantitative reanalysis should use the OSF data and code, reproduce the main contrasts and moderation results, and report confidence intervals and multiplicity handling. No new public survey is required for the current phase.
