# Arctic Amplification: Clouds and Feedback Mechanisms

This repository contains analysis scripts and notebooks developed during the **Arctic Amplification (AC)³** Winter School organized by the (AC)³ project and the University of Helsinki (2023). The project focuses on the role of clouds in Arctic feedback mechanisms, specifically examining how changes in surface temperature respond to radiative forcing.

## Scientific Context

Arctic Amplification refers to the phenomenon where the Arctic warms at a rate faster than the global average. This project evaluates the **Climate Feedback Parameter ($\lambda$)** and its role in the temporal evolution of surface temperature change ($\Delta T_s$).

### Process Overview

The project implements a zero-order energy balance model to simulate the response of the ocean mixed layer to climate forcing:

$$\Delta T_s(t) = \frac{ERF}{\lambda}\left[exp\left(\frac{\lambda}{C}t\right)-1\right]$$

Where:
- **$ERF$**: Effective Radiative Forcing ($W/m^2$).
- **$\lambda$**: Climate feedback parameter ($W/m^2 K$).
- **$C$**: Heat capacity of the ocean mixed layer (calculated for a 100m column).
- **$t$**: Time evolution.

## Key Features

1. **Energy Balance Modeling**: Calculation of the ocean mixed layer heat capacity and simulation of temperature trajectories under varying forcing scenarios.
2. **Gregory Analysis**: Implementation of the Gregory method to estimate ERF and $\lambda$ from model output (abrupt-4xCO2 vs. piControl experiments) using linear regression.
3. **Model Evaluation**: Comparative analysis of MPI-ESM1-2-LR climate model data.

## Requirements

- Python 3.x
- NumPy
- Matplotlib
- NetCDF4 / Xarray (for climate model data handling)

## Usage

The main analysis is contained within `Project_Work_final.ipynb`. The notebook is structured into tasks that guide the user through the mathematical derivation, numerical implementation, and scientific interpretation of the results.
