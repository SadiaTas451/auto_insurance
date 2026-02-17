# Auto Insurance Pricing (US) — Regression Analysis

## Overview
This project explores how different customer + coverage features affect quoted auto insurance cost in the United States.
Using a cleaned Allstate-style dataset, I perform exploratory analysis and build multiple linear regression (OLS) models.

## Dataset
File: `Allstate-cost-cleaned.csv`

Key columns include:
- `state`, `group_size`, `homeowner`, `car_age`, `car_value`, `risk_factor`
- `age_oldest`, `age_youngest`, `married_couple`
- prior coverage: `C_previous`, `duration_previous`
- coverage options: `A, B, C, D, E, F, G`
- target: `cost`

## Methods
- Exploratory Data Analysis (scatterplots, boxplots, etc.)
- One-hot encoding for categorical variables (coverages, car value, state/region)
- Baseline OLS regression with train/test split
- Feature selection: state → region aggregation
- Multicollinearity check using VIF
- Optional feature engineering (squared terms + interactions)

## Results (what to write after you run it)
- Report R² / Adjusted R²
- Mention the strongest predictors (largest magnitude coefficients + significant p-values)
- Note any counterintuitive signs and possible reasons (coding, correlations)

## How to Run
1. Clone/download this repo
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
