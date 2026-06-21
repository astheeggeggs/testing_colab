# CLAUDE.md

## Purpose

This repo holds **teaching practicals** (Jupyter notebooks) for the **SMARTbiomed
summer school** course on statistical genetics. The notebooks are designed to run
on **Google Colab** and are launched directly from GitHub via "Open in Colab"
badges (the repo is published as `astheeggeggs/testing_colab`).

The teaching goal is **understanding what happens under the hood**, not plug-and-play
use of existing software. Each practical should start simple and end with several
open-ended, more challenging questions for students who progress quickly. Students
have access to an answer sheet to check their work during or after class.

## Course context

The notebooks support the **Thursday "Summary statistics methods"** day (afternoon
sessions led by Nik), plus rare-variant material. The relevant sessions are:

- **Session 3 — Genetic correlation**: cross-trait (bivariate) LDSC, interpreting
  `rg`, and its pitfalls (low-h2 traits, `rg` ≠ causation, opposing local
  correlations cancelling, no cross-ancestry `rg`).
- **Session 4 — Meta-analysis**: fixed-effects inverse-variance-weighted (IVW)
  meta-analysis, when to use random effects, and the Cauchy combination test for
  correlated tests.
- **Heritability** (morning, led by Duncan): building intuition for how LDSC
  estimates SNP `h2`, S-LDSC, assumptions and pitfalls.
- **Rare-variant testing**: Fisher's exact tests and gene-based burden/SKAT tests
  via SAIGE-Gene.

## Notebooks

- `LDSC_Practical_1_h2.ipynb` — SNP heritability ($h^2_{\text{SNP}}$) estimation via
  univariate LD Score Regression.
- `LDSC_Practical_2_rg.ipynb` — Genetic correlation ($r_g$) estimation via bivariate
  LDSC (using `GenomicSEM`).
- `rare_variant_Fisher.ipynb` — Fisher's exact tests on a bipolar exome-sequencing
  subset (BipEx data).
- `rare_variant_SAIGE.ipynb` — Gene-based rare-variant association testing with
  SAIGE-Gene.

## Conventions

- **Runtime**: Notebooks use a **Python** Colab runtime but most analysis is in
  **R**, executed via the `%%R` cell magic (`rpy2`). The SAIGE notebook installs
  software from source using `pixi`.
- **Data**: Datasets are pulled into the Colab session (e.g. `/content/...`) from
  public Google Drive folders using `gdown`. Data has been pre-QC'd.
- **Audience**: 20–40 students per class. Keep explanations intuitive; surface the
  underlying math/equations rather than hiding them behind tooling.
- Each notebook opens with a Colab badge pointing at the GitHub-hosted copy — keep
  these in sync with the repo/branch name if it changes.
