# SI252 Reinforcement Learning — Homework 1

- `main.tex`: concise English solutions to Problems 1–10, including all subparts.
- `main.pdf`: compiled submission.
- The required Problem 10(b) concave-utility curve is drawn directly in TikZ; no external image files or shell escape are needed.

## Build

A standard TeX Live installation with pdfLaTeX and latexmk is sufficient (tested with TeX Live 2024).

```sh
latexmk -pdf -interaction=nonstopmode -halt-on-error -outdir=build main.tex
```

The result is `build/main.pdf`. Copy it to `main.pdf` when publishing. Generated auxiliary files and review images should not be committed.

## Revision notes

- Standardized headings, notation, tables, and page layout; removed repeated derivations while retaining key steps.
- Completed both directions of the MMSE orthogonality argument in Problem 2(e).
- Retained both required proofs in Problem 7 and covered degenerate Gaussian cases.
- Completed Problem 10(e)–(g): VNM expected utility, episodic reward construction, and the distinction between trajectory utility and Markov rewards.
- Corrected Problem 10(f): both schedules have average service `(6, 3)`, hence average-service utility `log(18)`; instantaneous cumulative utilities are `log(324)` and `log(100)`.
