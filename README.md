# Bias adjustment of multivariable heat-stress indices over southeastern South America

This repository contains the code used to evaluate bias-adjustment methods and adjustment strategies for multivariable heat-stress indices over southeastern South America (SESA).

The analysis considers wet-bulb temperature (WBT) and simplified wet-bulb globe temperature (sWBGT), using regional climate simulations from CORDEX/CORDEX-CORE and MSWX as observational reference.

## Reproducibility

The repository provides a reproducible example for one RCM simulation.

Processed data required to reproduce the example are archived on Zenodo:

**Zenodo:** 10.5281/zenodo.22638510

CORDEX regional climate simulations are publicly available through the Earth System Grid Federation (ESGF). The notebook `01_example_load_data.ipynb` illustrates how the required CORDEX-CORE data can be accessed using the climate4R framework.

## Repository structure

- `notebooks/`: notebooks reproducing the analysis workflow

## Bias-adjustment methods

The repository includes examples for:

- EQM (univariate)
- MBCr (multivariate)


Both direct and indirect adjustment strategies are considered.

## Data availability

CORDEX data:
https://cordex.org/data-access/cordex-cmip5-data/cordex-cmip5-esgf/

MSWX:
https://www.gloh2o.org/mswx/

Processed MSWX and CORDEX data for the reproducibility example:
10.5281/zenodo.22638510

## Citation


