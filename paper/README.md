# nanoGenRec Technical Report

This directory contains the nanoGenRec technical report and its build files.

## Files

| File | Purpose |
|------|---------|
| `nanogenrec.tex` | Main technical report source. |
| `references.bib` | Verified bibliography entries used by the draft. |
| `check_paper_consistency.py` | Repository-local consistency checker for author placeholders, citations, figures, and copied experiment numbers. |
| `figures/` | Figures copied from repository experiment artifacts for a self-contained report build. |

## Build

From this directory:

```bash
pdflatex nanogenrec
bibtex nanogenrec
pdflatex nanogenrec
pdflatex nanogenrec
```

Run the repository consistency checks from the repository root:

```bash
python3 paper/check_paper_consistency.py
```

The PDF is intended as a project technical report for open-source release and portfolio use.
