# Healthcare Claims Analytics  
## Medicare Geographic Variation Analysis (2019–2023)

## Key Results

- Model explains ~66% of cross-county variation in Medicare spending
- Predicts per-capita spending within ~$751 on average (MAE)
- Identifies clinical risk and inpatient utilization as primary cost drivers

---

## Overview

This project analyzes drivers of geographic variation in standardized Medicare spending per capita across U.S. counties from 2019–2023 using CMS public data.

The objective was to identify demographic and utilization factors associated with higher Medicare spending and evaluate model performance using both statistical inference and out-of-sample validation.

---

## Data Source

**CMS Medicare Fee-for-Service Geographic Variation Public Use File (2014–2023)**

- County-level observations  
- Restricted to:
  - Years: 2019–2023  
  - Age level: All beneficiaries  
- Final modeling dataset: ~15,000 county-year observations  

---

## Problem Statement

Medicare spending varies significantly across geographic regions.  
This project investigates:

- Which beneficiary characteristics drive higher per-capita spending?
- How much variation can be explained using demographic and utilization metrics?
- How well does the model generalize to unseen data?

---

## Features Used

**Predictors:**

- Average beneficiary risk score  
- Average age  
- Dual-eligible percentage  
- Inpatient stays per 1,000 beneficiaries  
- ER visits per 1,000 beneficiaries  
- Acute hospital readmission percentage  

**Target Variable:**

- Standardized Medicare spending per capita  

---

## Methodology

### 1. Data Preparation

- Filtered to county-level observations  
- Restricted to 2019–2023  
- Selected relevant clinical and demographic variables  
- Converted all numeric fields and removed missing values  

### 2. Exploratory Data Analysis

- Distribution analysis of spending  
- Correlation heatmap  
- Multicollinearity assessment  

### 3. Statistical Modeling

- Applied log transformation to spending to reduce skewness  
- Estimated OLS regression to interpret coefficient effects  

### 4. Model Validation

- Train/test split (80/20)  
- Linear regression model  
- Evaluated using:
  - RMSE  
  - MAE  
  - Test R²  
- Residual diagnostics to assess model assumptions  

---

## Results

### Out-of-Sample Performance (Test Set)

- **R²:** ~0.66  
- **RMSE:** ~$1,040  
- **MAE:** ~$751  

### Key Findings

- Risk score is the strongest predictor of spending  
- Higher inpatient utilization significantly increases costs  
- Dual-eligible percentage shows a modest negative association  
- Model explains approximately two-thirds of geographic variation  

---

## Business & Policy Implications

- Risk adjustment is critical for cost forecasting  
- Utilization metrics strongly drive spending variation  
- Counties with elevated inpatient rates may warrant targeted interventions  
- Model provides a foundation for cost control and risk stratification strategies  

---

## Limitations

- Limited to CMS public variables  
- No socioeconomic or provider supply metrics  
- Linear model assumptions may not fully capture complex cost dynamics  

---

## Tools Used

- Python (Pandas, NumPy)  
- Statsmodels  
- Scikit-learn  
- Seaborn / Matplotlib  

- Git


## Executive Summary

A detailed executive-level summary is available here:

[View Executive Summary](reports/executive_summary.md)

