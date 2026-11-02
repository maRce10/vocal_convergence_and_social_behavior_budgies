# Vocal convergence and social behavior in budgerigars

[![Website](https://img.shields.io/badge/website-analysis%20report-408AB4)](https://marce10.github.io/vocal-convergence-social-behavior-budgies/)
[![Publish website](https://github.com/maRce10/vocal-convergence-social-behavior-budgies/actions/workflows/publish.yml/badge.svg)](https://github.com/maRce10/vocal-convergence-social-behavior-budgies/actions/workflows/publish.yml)

Statistical analysis of how social interactions (proximity, affiliative and agonistic interactions) and vocal convergence influence each other in budgerigars (*Melopsittacus undulatus*).

## Website

The rendered analysis report, with code, results and figures, is available at **[marce10.github.io/vocal-convergence-social-behavior-budgies](https://marce10.github.io/vocal-convergence-social-behavior-budgies/)**:

- [Statistical analysis](https://marce10.github.io/vocal-convergence-social-behavior-budgies/scripts/stats_v06_energy.html): energy distances with bootstrap measurement error, social data aligned to the acoustic blocks recorded at the same time, acoustic change and cross-lagged Bayesian models, and robustness checks

## Repository structure

```
_quarto.yml, index.qmd, styles.css      Quarto website configuration (cached code results in _freeze/)
_figure-download.html                   Adds a download button below each figure
.github/workflows/publish.yml           GitHub Actions workflow that builds the website and deploys it to GitHub Pages
scripts/
  stats_v06_energy.qmd                  Statistical analysis (latest version)
  qmd.css                               Style sheet for the rendered report
output/figures/                         Figures shown on the website
```

The website is built from the cached results in `_freeze/`, so GitHub Actions does not need R or the data. To update it, render the website locally (`quarto render`) and commit `_freeze/` together with the edited `.qmd` files.
