# SI252 Reinforcement Learning — Homework 1

- `main.tex`: English solutions to Problems 1–10, including all subparts. Problems 2–9 retain the detailed derivations. Problems 1 and 10 use shorter, simpler explanations; Problem 10 follows the supplied T10 notes and retains the required proofs and calculations.
- `main.pdf`: compiled submission.
- The required Problem 10(b) concave-utility curve is drawn directly in TikZ; no external image files or shell escape are needed.

## Build

A standard TeX Live installation with pdfLaTeX and latexmk is sufficient (tested with TeX Live 2024).

```sh
latexmk -pdf -interaction=nonstopmode -halt-on-error -outdir=build main.tex
```

The result is `build/main.pdf`. Copy it to `main.pdf` when publishing. Generated auxiliary files and review images should not be committed.

## Revision notes

- Simplified Problems 1 and 10 with plain English, concrete examples, and less repeated explanation. Problems 2–9 and the page layout are unchanged from the detailed edition.
- Restored the original detailed derivations for Problems 1–9 rather than using the earlier eight-page abridgment. Only immediately duplicated conclusions and minor wording issues were removed.
- Applied light formatting changes: readable 11pt text, consistent question headings, page headers, and line breaks for long equations.
- Translated Problem 10 from the supplied T10 notes, preserving their reasoning and the AM–GM approach to the weighted allocation; filled in proof steps where the notes gave hints.
- Completed both directions of the MMSE orthogonality argument in Problem 2(e).
- Retained both required proofs in Problem 7 and covered degenerate Gaussian cases.
- Completed Problem 10(e)–(g): VNM expected utility, episodic reward construction, and the distinction between trajectory utility and Markov rewards.
- Corrected Problem 10(f): both schedules have average service `(6, 3)`, hence average-service utility `log(18)`; instantaneous cumulative utilities are `log(324)` and `log(100)`.
