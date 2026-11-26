# EJPS LaTeX build status

**Date:** 2026-11-27  
**Status:** Source prepared; official-template compilation blocked. No PDF is claimed as generated or inspected.

## Local environment actually checked

- OS: Debian GNU/Linux 13 (trixie), x86_64.
- `pdflatex`: `/usr/bin/pdflatex`.
- `latexmk`: `/usr/bin/latexmk`.
- `xelatex`, `lualatex`, `pandoc`, `pdfinfo`, and `pdftotext`: available.
- `apacite.sty` and `apacite.bst`: available.
- `kpsewhich sn-jnl.cls`: no path returned; the Springer Nature class is not installed locally.

## Retrieval attempts

A real PDFLaTeX template smoke test was run with the required class declaration. The command exited with status 1 because `sn-jnl.cls` was not found. The exact output is preserved in `BUILD_LOG_TEMPLATE_MISSING.txt`.


1. Identified the official journal-article template ZIP on the Springer Nature LaTeX author-support page:
   https://www.springernature.com/gp/authors/campaigns/latex-author-support
2. Downloading the official ZIP into the current container failed.
3. A GitHub clone attempt failed with DNS resolution error: `Could not resolve host: github.com`.
4. No substitute or fabricated Springer class was used.

## Consequence

The anonymous source uses `\documentclass[pdflatex,sn-apa]{sn-jnl}`. The source is ready for the official template files, but the required class is unavailable in this environment. Therefore no successful Springer-template build, PDF generation, or visual inspection is claimed.

## Required build after the official template is obtained

Place `sn-jnl.cls` and any required template support files alongside `anonymous-manuscript.tex`, then run:

```sh
pdflatex -interaction=nonstopmode -halt-on-error anonymous-manuscript.tex
pdflatex -interaction=nonstopmode -halt-on-error anonymous-manuscript.tex
pdfinfo anonymous-manuscript.pdf
pdftotext anonymous-manuscript.pdf anonymous-manuscript.txt
```

Preserve the complete terminal output as the build log and inspect the PDF visually before submission.
