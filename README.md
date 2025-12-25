# Hourly Price Forward Curve (HPFC)
## Market-consistent two-stage modelling for power risk and valuation

![hpfc](figures/hpfc.png)
[Full technical documentation (PDF)](docs/hpfc_doc.pdf)

## Executive Summary
This project develops a market-consistent Hourly Price Forward Curve (HPFC) for electricity markets, designed for risk measurement, valuation, and scenario analysis.
The model exactly preserves traded weekly forward prices while producing a stable, interpretable, and auditable hourly structure.

## Target use cases:
* Trading desks  
* Risk management 
* Portfolio valuation & PnL attribution 
* Load & generation exposure analysis

## Problem Statement
Electricity forwards are typically quoted at weekly or monthly granularity, while risk and P&L are driven by hourly price dynamics.
Naïve disaggregation introduces:
* Arbitrage violations
* Instability
* Loss of market consistency

## Objective:
Construct an hourly curve that is:
* Fully consistent with observed market prices
* Structurally constrained
* Suitable for downstream risk models

## Methodology Overview
A two-stage linearized framework separates shape from price level, improving robustness and interpretability.

### Stage 1 — Intraday Shape Modelling
* Normalize prices by weekly base levels
* Estimate hourly peak/off-peak profiles
* Seasonal bucketing to capture:
- Solar generation impact
- Weekday / weekend effects
* Shape estimation performed under explicit linear constraints

### Stage 2 — Weekly Price Reintroduction
* Rescale normalized shapes using observed weekly forward prices
* Guarantees exact preservation of traded market levels

## Key Model Properties
* Market consistency: Weekly base prices are preserved exactly (no arbitrage)
* Stability: Linearized estimation avoids overfitting and regime instability
* Interpretability: Clear separation of shape drivers vs price level
* Auditability: Deterministic, constraint-based construction suitable for risk governance

## Validation & Diagnostics
* Hourly reconstruction vs observed spot prices
* Shape stability across seasons
* Sensitivity to solar production regimes

## Outcome:
The model produces smooth, realistic hourly profiles while maintaining strict alignment with forward market inputs.

## Implementation
* Language: Python
* Core stack: NumPy, pandas, SciPy
* * Focus: Transparency over black-box optimization
* Design: Modular, fully reproducible pipeline

Focus: Transparency over black-box optimization
