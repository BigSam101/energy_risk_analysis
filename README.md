# Energy System Risk Analysis with PyPSA-Eur

This repository contains analysis code for electricity system modelling
using PyPSA and PyPSA-Eur, with a focus on uncertainty and risk in
long-term power system planning.

The repository includes regional case studies (e.g. SE–DE–DK, Belgium)
and methodological experiments related to system costs, prices,
and flexibility under uncertain conditions.

## Scope
- Deterministic baseline optimisation
- Scenario-based stochastic analysis
- Expected value and risk metrics
- Conditional Value-at-Risk (CVaR)
- Stress-scenario assessment
- Sensitivity analysis of system flexibility (e.g. demand response, storage)

## Methodology
Uncertainty is represented using a discrete scenario-based framework with
explicit probabilities. Risk is quantified using expected values and
Conditional Value-at-Risk (CVaR).

Full Monte Carlo re-optimisation is deliberately avoided in favour of
scenario-based risk metrics to ensure computational tractability for
large-scale energy system models.

## Repository Structure
- `notebooks/` – Jupyter notebooks for analysis and case studies
- `scripts/` – Reusable helper functions and analysis utilities
- `figures/` – Exported plots

## Requirements
- Python 3.10+
- PyPSA / PyPSA-Eur
- HiGHS or Gurobi solver

## Notes
This repository is part of an ongoing capstone project.
Large input data and solved network files are not included and must be
generated separately using PyPSA-Eur.

