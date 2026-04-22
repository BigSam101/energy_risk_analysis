# Energy System Risk Analysis with PyPSA-Eur

This repository contains analysis code for large-scale electricity system
modelling using PyPSA and PyPSA-Eur, with a focus on uncertainty,
renewable integration, and system-level risk.

The work combines regional case studies (Sweden–Germany–Denmark) with
methodological experiments to evaluate how variability in demand and
renewable generation affects system costs, electricity prices, and
reliance on backup generation.

## Scope
- Deterministic baseline optimisation
- Scenario-based stochastic analysis
- Expected value and risk metrics
- Conditional Value-at-Risk (CVaR)
- Stress-scenario assessment
- Sensitivity analysis of system flexibility (e.g. demand response, storage)

## Methodology
Uncertainty is represented using a discrete scenario-based framework with
explicit probabilities applied to key drivers such as demand, wind, and
solar availability.

Risk is quantified using:
- Expected system cost
- Price distribution metrics
- Conditional Value-at-Risk (CVaR)

The approach prioritises computational tractability by using scenario-based
optimisation instead of full Monte Carlo re-optimisation.

## Key Insights
- Renewable variability significantly impacts system cost and price risk
- Low renewable availability scenarios drive system stress and cost spikes
- Risk metrics (e.g. CVaR) provide additional insight beyond expected values
- System flexibility plays a critical role in mitigating uncertainty

## Repository Structure
- `notebooks/` – Jupyter notebooks for analysis and case studies
- `scripts/` – Reusable helper functions and modelling utilities
- `figures/` – Exported plots used for interpretation and reporting

## Requirements
- Python 3.10+
- PyPSA / PyPSA-Eur
- HiGHS or Gurobi solver

## Notes
This repository is part of an ongoing capstone project.

Large input datasets and solved network files are not included due to size
and reproducibility constraints. Results can be reproduced by running the
PyPSA-Eur workflow with the appropriate configuration.
