# Bias adjustment of multivariable heat-stress indices over southeastern South America

This repository contains the code used to evaluate bias-adjustment methods and adjustment strategies for multivariable heat-stress indices over southeastern South America (SESA).

The analysis considers wet-bulb temperature (WBT) and simplified wet-bulb globe temperature (sWBGT), using regional climate simulations from CORDEX/CORDEX-CORE and MSWX as observational reference.

## Reproducibility

The repository provides a reproducible example for one RCM simulation.

Processed data required to reproduce the example are archived on **Zenodo:** [10.5281/zenodo.22638510](https://doi.org/10.5281/zenodo.22638510)

CORDEX regional climate simulations are publicly available through the Earth System Grid Federation (ESGF). The notebook `01_example_load_data.ipynb` illustrates how the required CORDEX-CORE data can be accessed using the climate4R framework.

## Repository structure

- `notebooks/`: notebooks reproducing the analysis workflow

## Software environment

The analyses were performed using a Micromamba environment. The following files are provided to document the software configuration:

- `environment.yml`: Conda environment specification used as the starting point for the analyses.
- `environment-linux-64-explicit.txt`: Explicit specification of the Conda package versions and builds installed on Linux (linux-64).
- `R_installed_packages.csv`: List of the final R package versions used in the analyses.

The original Conda environment can be created with:

```bash
micromamba create -f environment.yml
```
For a more exact reproduction of the original Linux environment:

```bash
micromamba create -n heat-stress-ba-sesa -f environment-linux-64-explicit.txt
```
Some R packages were installed or updated directly within R after the Conda environment was created, as certain packages or required versions were not available through Conda. Consequently, the versions recorded in the Conda environment files may differ from those actually used in the analyses.

The final R package versions are documented in `R_installed_packages.csv`, including downscaleR 3.3.2, MBC 0.10-8, and HeatStress 1.0.8.1. These versions should be installed within the activated environment to reproduce the analyses.

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
https://doi.org/10.5281/zenodo.22638510

## Citation


