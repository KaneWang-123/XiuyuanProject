# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a theoretical physics paper reading and research repository. It contains LaTeX source files for arXiv papers, primarily in high energy physics (flavor symmetries, non-invertible symmetries, string compactifications, strong CP problem).

## Conventions

### Paper storage
- Papers are stored as folders named by their arXiv ID (e.g., `arXiv-2402.12453v1`) until read, after which the folder is renamed to the paper's title.
- Some papers arrive as a single `.tex` file with no folder (e.g., `arXiv-0806.4748v2`).
- The main tex file is typically named `draft.tex` or `draft_arXiv.tex`.

### Reading papers
- Always read the LaTeX source directly — it preserves all equations and structure.
- The abstract and title are near the top of the `.tex` file, before `\begin{document}` or just after `\maketitle`.
- For large `.tex` files (>10,000 tokens), read in chunks of ~150 lines at a time using `offset` and `limit`.

### Outputting explanations
- When asked to explain something with equations, produce an HTML file using MathJax for rendering (see `explanation_Ng_Nc.html` as a template). The user opens these directly in a browser.
- Use `https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js` as the MathJax CDN.

## Current Papers

| Folder / File | Title | Topic |
|---|---|---|
| `arXiv-2409.05270v1/` | *Yukawa textures from non-invertible symmetries* | Non-invertible symmetries → Yukawa textures for quarks/leptons; NNI texture from $\mathbb{Z}_M$ + gauged $\mathbb{Z}_2$ |
| `Non-Invertible Peccei-Quinn Symmetry.../` | *Non-Invertible Peccei-Quinn Symmetry and the Massless Quark Solution to the Strong CP Problem* | Non-invertible PQ symmetry from fractional instantons in $(SU(3)_C \times U(1)_H)/\mathbb{Z}_3$; $SU(9)$ color-flavor unification; strong CP solution |
| `arXiv-0806.4748v2` | *Magnetized orbifold models* | Magnetized D-brane compactifications on orbifolds |
