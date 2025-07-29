# # COSI GRB bn081207680 – Binning and TS Map Pipeline

This repository provides a complete workflow for the analysis of GRB `bn081207680` using COSI DC3 simulated data. It includes data binning into Compton Data Space (CDS), background modeling, and Test Statistic (TS) map computation based on a Poisson likelihood framework.

## Files Included

| File Name                                      | Description |
|-----------------------------------------------|-------------|
| `GRB_bn081207680_Binning_Full_Auto.ipynb`     | Automates download and binning of GRB photon data |
| `GRB_bn081207680_binned_O3.hdf5`              | Binned GRB event data in CDS format |
| `Total_BG_binned_O3.hdf5`                     | Binned background data from 3-month exposure |
| `inputs_grb.yaml`                             | Configuration file for GRB binning |
| `input_bg.yaml`                               | Configuration file for background binning |
| `Parallel_TS_map_computation_bn081207680.ipynb` | TS map computation using `FastTSMap` and Poisson likelihood |

## Features

- Automated binning of GRB and background events using official COSI response and orientation data
- YAML-based configuration for reproducible preprocessing
- Poisson-likelihood-based TS map generation using `cosipy.FastTSMap`
- Parallelized computation over HEALPix sky pixels
- Spectral modeling via `astromodels` (e.g., Band function)
- Outputs significance maps for GRB localization and flux evaluation



