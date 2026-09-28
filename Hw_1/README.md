# SI252 Reinforcement Learning — Homework 1

- `main.tex`: English solutions to Problems 1–10, including all subparts. The latest author revision is preserved, with the missing Problem 10(b) figure restored and small correctness/wording fixes.
- `main.pdf`: compiled submission.
- The required Problem 10(b) concave-utility curve is drawn directly in TikZ; no external image files or shell escape are needed.

## Build

A standard TeX Live installation with pdfLaTeX and latexmk is sufficient (tested with TeX Live 2024).

```sh
latexmk -pdf -interaction=nonstopmode -halt-on-error -outdir=build main.tex
```

The result is `build/main.pdf`. Copy it to `main.pdf` when publishing. Generated auxiliary files and review images should not be committed.

## Latest review

- Checked all ten problems and their requested subparts; restored the omitted utility-curve sketch in Problem 10(b).
- Clarified that increasing utility and strict concavity are separate assumptions; maximizing minimum service gives equal rates in this specific feasible set.
- Stated VNM independence in its standard two-way form and clarified the distinction between the VNM theorem and the RL reward hypothesis.
- Replaced “quantize a goal” with “express a goal numerically,” clarified the fixed reward rule on the augmented state, and stated the finite-second-moment assumption in Problem 2(c).
- Recompiled the revised document: 27 pages, with no LaTeX errors, warnings, or over/underfull boxes.

## Earlier revision notes

- Simplified Problems 1 and 10 with plain English, concrete examples, and less repeated explanation, while retaining the detailed derivations in Problems 2–9.
- Restored the original detailed derivations for Problems 1–9 rather than using the earlier eight-page abridgment. Only immediately duplicated conclusions and minor wording issues were removed.
- Applied light formatting changes: readable 11pt text, consistent question headings, page headers, and line breaks for long equations.
- Translated Problem 10 from the supplied T10 notes, preserving their reasoning and the AM–GM approach to the weighted allocation; filled in proof steps where the notes gave hints.
- Completed both directions of the MMSE orthogonality argument in Problem 2(e).
- Retained both required proofs in Problem 7 and covered degenerate Gaussian cases.
- Completed Problem 10(e)–(g): VNM expected utility, episodic reward construction, and the distinction between trajectory utility and Markov rewards.
- Corrected Problem 10(f): both schedules have average service `(6, 3)`, hence average-service utility `log(18)`; instantaneous cumulative utilities are `log(324)` and `log(100)`.
