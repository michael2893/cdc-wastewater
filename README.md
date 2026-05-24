[![DOI](https://zenodo.org/badge/1248443754.svg)](https://doi.org/10.5281/zenodo.20368030)

### Summary

Bayesian analysis of CDC wastewater viral data to understand how population size affects SARS‑CoV‑2, RSV, and Influenza‑A concentrations.

This project applies Bayesian hierarchical models to over 1,200 wastewater surveillance sites from the CDC’s National Wastewater Surveillance System (NWSS). 

 - Model 1 – Hierarchical linear regression – Quantify how viral activity (measured by the WVAL metric) varies across individual sites and states, and whether population size explains any of that variation.
 - Model 2 – Dirichlet regression – Examine how the relative proportions of SARS‑CoV‑2, Influenza‑A, and RSV change with population size, using a multivariate compositional model.

#### Key findings

Between‑site variance is larger than between‑state variance – contrary to my initial hypothesis that state‑level testing policies would drive more variation.
Population size has a modest positive effect on overall viral concentration (β₁ HDI: 0.028–0.153).
Dirichlet model suggests that population size affects the share of each pathogen differently, though the effect is small in magnitude.
Models converged well (ˆR = 1.0) with high effective sample sizes.

#### Reproducibility

All code (Python, PyMC, Pandas) is provided as a Jupyter notebook. The report (PDF) includes full derivations, prior justification, posterior summaries, and trace plots. A requirements.txt file and data‑cleaning steps are included for full reproducibility.

## Data Source

Centers for Disease Control and Prevention. (2024). *National Wastewater 
Surveillance System (NWSS) Public Concentration Data*. U.S. Department of 
Health & Human Services. https://www.cdc.gov/nwss/

## Citation

If you use or reference this work, please cite it as:

Michael Terranova. (2026). *Bayesian hierarchical modeling of multi-pathogen 
wastewater surveillance across 1,200+ CDC NWSS sites*. GitHub. 
https://github.com/michael2893/cdc-wastewater
