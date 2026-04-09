# Statistical Analysis and Causal Inference

This repository explores fundamental statistical modeling concepts, including regression analysis, multicollinearity diagnostics, hypothesis testing, and causal inference. The project emphasizes analytical reasoning and the interpretation of statistical model outputs.

## 📌 Key Topics
- **Regression Analysis**: Multiple linear regression and logistic regression for binary outcomes
- **Multicollinearity**: Diagnostics using correlation matrix, Variance Inflation Factor (VIF), and condition index
- **Interaction Effects**: Modeling complex relationships and interpretation in nonlinear models
- **Multiple Comparison**: Addressing multiplicity issues using Familywise Error Rate (FWER) and False Discovery Rate (FDR)
- **Causal Inference**: Identifying variables and validating structures through causal graphs and d-separation

## 🛠 Methodology
- **Ordinary Least Squares (OLS)** and **Maximum Likelihood Estimation (MLE)**
- Diagnostics: VIF, condition index, and correlation matrix
- Hypothesis testing: Type I/II error control, Bonferroni correction, Holm procedure
- Causal analysis: partial correlation and conditional independence testing

## 📊 Analysis Summary

### Regression & Multicollinearity
A multiple linear regression model was utilized to examine relationships between variables. Multicollinearity diagnostics indicated no significant issues, suggesting predictors contributed independently.

A logistic regression model was also applied to identify significant predictors for binary outcomes.

### Interaction & Multiple Comparison
Interaction terms were introduced to capture how the effect of one variable depends on another.

The analysis also addressed the multiplicity problem, where conducting multiple tests increases the risk of false discoveries. Approaches such as FWER and FDR were considered to balance statistical power and error control.

### Causal Inference
A causal graph framework was used to infer relationships based on correlation structure.

Variables were identified through correlation patterns and validated using conditional independence tests, including partial correlation and d-separation.

## 📝 Notes
- **Implementation**: Analysis was conducted using MATLAB
- **Context**: This work was completed as part of a technical assessment during a research internship
- **Data Privacy**: Proprietary datasets and assignment materials are not included

## 📚 References
- Montgomery, D. C., et al. (2021). *Introduction to Linear Regression Analysis*
- Pearl, J., et al. (2016). *Causal Inference in Statistics: A Primer*
- Ai, C., & Norton, E. C. (2003). *Interaction terms in logit and probit models*
