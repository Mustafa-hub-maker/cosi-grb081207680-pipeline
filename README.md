# COSI GRB bn081207680 – Binning & TS Map Pipeline

This repository contains a complete analysis workflow for the COSI GRB `bn081207680`. It includes automated binning of photon and background data into Compton Data Space (CDS) and prepares inputs for likelihood-based Test Statistic (TS) map generation.

---

## Files Included

| File Name                            | Description                                        |
|-------------------------------------|----------------------------------------------------|
| `GRB_bn081207680_Binning_Full_Auto.ipynb` | Notebook for automating data download and binning |
| `GRB_bn081207680_binned_O3.hdf5`    | Binned GRB event data (CDS format)                |
| `Total_BG_binned_O3.hdf5`           | Binned background data from 3-month dataset       |
| `inputs_grb.yaml`                   | GRB binning configuration                         |
| `input_bg.yaml`                     | Background binning configuration                  |

---

## Features

- Automates COSI DC3 data preparation and binning
- Uses COSI response files and mission orientation data
- Generates HDF5-format binned data for GRB and background
- Compatible with `FastTSMap` for TS map analysis

