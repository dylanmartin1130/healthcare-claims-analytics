# Executive Summary  
## Medicare Geographic Variation Analysis (2019–2023)

### Objective

This analysis evaluates drivers of variation in standardized Medicare Fee-for-Service spending per capita across U.S. counties between 2019 and 2023. The goal is to distinguish structural cost drivers from potentially modifiable utilization patterns using multivariate regression modeling.

---

## Data & Methodology

County-level Medicare Geographic Variation Public Use File data (CMS) was used for years 2019–2023. The dependent variable was standardized Medicare spending per capita.

A multivariate OLS regression model was constructed using demographic, risk, and utilization variables. Multicollinearity was assessed using Variance Inflation Factors (VIF), and a log transformation of spending was applied to improve model stability and interpretability.

The final model explains approximately 55% of cross-county spending variation (R² ≈ 0.55), which is strong performance for cross-sectional healthcare cost modeling.

---

## Key Findings

### 1. Clinical Risk Is the Primary Structural Driver

Average beneficiary risk score is the strongest predictor of Medicare spending. Higher disease burden meaningfully increases per capita cost.

This confirms that underlying health status is the dominant structural determinant of regional spending variation.

---

### 2. Population Aging Independently Increases Spending

Average beneficiary age is positively associated with spending. Even after controlling for risk score, aging populations drive additional cost.

Demographic composition plays a significant role in geographic variation.

---

### 3. Inpatient Utilization Is a Major Operational Cost Lever

Inpatient covered stays per 1,000 beneficiaries are strongly associated with higher spending.

Simulation modeling indicates that a 5% reduction in inpatient utilization corresponds to approximately $160 reduction per beneficiary annually.

For a county with 20,000 Medicare beneficiaries, this equates to over $3 million in potential annual cost impact.

This suggests inpatient utilization intensity is a meaningful operational intervention target.

---

### 4. Emergency Department Utilization Has Incremental Impact

Emergency visits per 1,000 beneficiaries are positively associated with spending, though with smaller magnitude compared to inpatient utilization.

---

### 5. Dual Eligibility Effects Are Mediated by Risk

After controlling for risk score and utilization intensity, dual eligibility percentage does not independently increase spending. This suggests socioeconomic vulnerability primarily influences cost through health status rather than direct cost amplification.

---

## Model Diagnostics

- Log transformation improved model stability and reduced skew.
- Multicollinearity was addressed through VIF assessment.
- Predicted vs. actual analysis demonstrated strong alignment in mid-spending counties with expected dispersion at extreme cost levels.
- Model residual patterns are consistent with healthcare cost data behavior.

---

## Implications for Policy and Healthcare Organizations

Geographic Medicare spending variation is driven by two major categories:

1. Structural Factors  
   - Disease burden  
   - Aging population  

2. Operational Factors  
   - Inpatient care intensity  
   - Acute utilization patterns  

While structural factors are largely non-modifiable in the short term, utilization intensity represents a measurable and potentially actionable lever under value-based care frameworks.

Targeted strategies focused on reducing avoidable hospital admissions may produce measurable fiscal impact while maintaining quality of care.

---

## Conclusion

This analysis demonstrates how structured regression modeling and utilization simulation can inform healthcare cost strategy decisions. By separating structural drivers from modifiable operational factors, policymakers and healthcare organizations can better prioritize intervention efforts.

The methodology reflects applied healthcare analytics practices used in payer analytics, value-based care strategy, and medical economics analysis.

