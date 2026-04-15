# CLAUDE.md — XiuyuanProject

## Project overview
Literature reading and research notes for a collaboration with Xiuyuan, focused on:
- **Non-invertible symmetries** and their applications to flavor physics
- **Strong CP problem** — non-invertible PQ symmetry, massless quark solution
- **String compactifications** — magnetized D-brane models, orbifold constructions, Yukawa textures

## Output format
**Always produce HTML with MathJax** for explanations, notes, and calculations.
Only use `.tex` when Zekai explicitly requests it.
MathJax CDN: `https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js`
Style reference: `explanation_Ng_Nc.html`

## Repository structure

### Papers
| Folder | arXiv | Title | Topic |
|---|---|---|---|
| `Yukawa textures from non-invertible symmetries/` | 2409.05270 | *Yukawa textures from non-invertible symmetries* | Kobayashi, Otsuka, Tanimoto — non-invertible $\mathbb{Z}_M$ + gauged $\mathbb{Z}_2$; NNI texture for quarks/leptons |
| `Non-Invertible Peccei-Quinn Symmetry and the Massless Quark Solution to the Strong CP Problem/` | 2402.12453 | *Non-Invertible Peccei-Quinn Symmetry and the Massless Quark Solution to the Strong CP Problem* | Córdova, Hong, Koren — non-invertible PQ symmetry, $SU(9)$ color-flavor unification, fractional instantons, strong CP |
| `Magnetized orbifold models` | 0806.4748 | *Magnetized orbifold models* | Abe, Kobayashi, Ohki — zero-modes on $T^6/(\mathbb{Z}_2\times\mathbb{Z}'_2)$ with magnetic fluxes, three-family models |

Main `.tex` file is typically named `draft.tex` or `draft_arXiv.tex`.

### HTML explanation files
| File | Contents |
|---|---|
| `explanation_Ng_Nc.html` | Why non-invertible PQ symmetry (arXiv:2402.12453) requires $N_g = N_c = 3$ |
| `explanation_magnetized_orbifold.html` | Full explainer: magnetized orbifold models, zero-mode counting, Yukawa selection rules, three-family models |
| `explanation_orbifold.html` | Orbifold construction basics |
| `explanation_orbifold_fermion_phase.html` | Fermion phase structure on orbifolds |
| `explanation_gauge_fields_on_orbifold.html` | Gauge fields on orbifold background |

## Reading papers
- Read LaTeX source directly — preserves all equations and structure
- Abstract and title are near the top of `.tex`, before `\begin{document}` or just after `\maketitle`
- For large files (>10,000 tokens), read in chunks of ~150 lines using `offset` and `limit`

## Paper storage convention
- On arrival: folder named by arXiv ID (e.g. `arXiv-2402.12453v1/`)
- After reading: rename folder to paper's full title
- Single `.tex` files (no folder): rename file to the paper title

## Git / GitHub
Remote: `KaneWang-123/XiuyuanProject`  
Branch: `master`
Do not commit `.DS_Store` (covered by `.gitignore`).
