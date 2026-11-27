# EJPS submission preparation

This directory contains working submission artifacts, not a final upload package.

- `anonymous-manuscript.tex`: blind manuscript source; no author block or identity metadata.
- `title-page-template.tex`: separate Title Page with placeholders; fill only with author-approved details.
- `AUTHOR_SOURCE_VERIFICATION_CHECKLIST.md`: 23 original-source checks, all pending author completion.
- `AI_USE_DECLARATION_AUTHOR_APPROVAL.md`: author-confirmed AI-use disclosure, inserted into the manuscript and separate Title Page.
- `EJPS_SUBMISSION_CHECKLIST.md`: author and technical acceptance criteria.
- `BUILD_STATUS.md`: actual local environment and build status.

## Official instructions checked on 2026-11-27

- Double-blind peer review; remove identifying information from manuscript and associated files; supply a separate Title Page.
- Original research articles: approximately 5,000–15,000 words.
- Abstract: 150–250 words; keywords: 4–6.
- Author–date citations; APA 7; full DOI links where available.
- References should be works cited in the text and published or accepted for publication.
- LaTeX is accepted for mathematical content; Springer Nature's LaTeX template is recommended.
- Do not use subfolders in the uploaded LaTeX source package.
- LLM use must be documented in Methods or a suitable alternative part of the manuscript. Springer Nature's general AI guidance also requests an AI Use Declaration at the end of the paper.

Official pages:
- https://link.springer.com/journal/13194/submission-guidelines
- https://www.springernature.com/gp/authors/campaigns/latex-author-support

## Build limitation

The official Springer Nature template archive could not be downloaded into the current container because outbound DNS/network access is unavailable. PDFLaTeX and latexmk are installed, but `sn-jnl.cls` is not installed locally. Therefore no successful Springer-template build or PDF inspection is claimed. See `BUILD_STATUS.md`.
