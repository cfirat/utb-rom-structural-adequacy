# Structural Adequacy of Reduced-Order Models for Underground Thermal Battery Dynamics

This repository contains the corrected reduced-order modelling workflow used for the manuscript:

**Structural Adequacy of Reduced-Order Models for Underground Thermal Battery Dynamics**

The code compares one-state, cascade two-state, and physically coupled two-state reduced-order models (ROMs) for a public high-fidelity underground thermal battery (UTB) benchmark. The workflow includes benchmark preprocessing, common-grid interpolation, spectral and autocorrelation diagnostics, differential-evolution calibration, temporal holdout evaluation, and automatic generation of manuscript tables and figures.

## Main Features

- Benchmark-consistent preprocessing of nonuniform UTB thermal-response data
- Interpolation of thermal observables onto a common hourly forcing grid
- Calibration/holdout split: years 1–3 for calibration and years 4–5 for holdout evaluation
- One-state aggregate ROM
- Cascade two-state ROM
- Physically coupled two-state ROM
- Exact analytical hourly integration under piecewise-constant forcing
- Multi-seed differential-evolution calibration
- Physical-unit RMSE, MAE, $$R^2$$, Durbin-Watson, and combined RMSE metrics
- Corrected fixed-prediction residual bootstrap intervals
- Automatic generation of manuscript-ready tables and figures

## Repository Structure

```text
notebooks/      Main corrected notebook
src/            Modular Python implementation of preprocessing, ROMs, calibration, and metrics
scripts/        Optional command-line scripts for reproducing results
data/           Instructions for obtaining the public benchmark data
docs/           Additional reproduction notes
