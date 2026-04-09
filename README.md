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

### Regression Analysis
A multiple linear regression model was used to examine the relationship between variables. Some predictors showed meaningful associations with the outcome, while others did not contribute significantly.

The analysis focused on interpreting variable significance and model stability rather than predictive performance.

Multicollinearity diagnostics, including correlation analysis and VIF, indicated no significant issues, suggesting that predictors contributed independently.

A logistic regression model was also applied to analyze binary outcomes, where certain variables were identified as significant predictors.

### Multicollinearity
Multicollinearity refers to high correlations among independent variables, which can lead to unstable coefficient estimates and misleading interpretations.

Potential causes include:
- Data collection constraints
- Model specification issues
- Redundant or highly correlated predictors

To diagnose multicollinearity:
- Correlation matrix analysis
- Variance Inflation Factor (VIF)
- Eigenvalue and condition index analysis

### Interaction Effects
Interaction terms were introduced to examine how the effect of one variable changes depending on another variable.

These allow the model to capture more complex relationships, though interpretation requires caution, especially in nonlinear models.

### Multiple Comparison
When conducting multiple hypothesis tests, the probability of false discoveries increases.

- Type I error: rejecting a true null hypothesis  
- Type II error: failing to reject a false null hypothesis  

To address this:
- Familywise Error Rate (FWER)
- False Discovery Rate (FDR)

FWER controls the probability of at least one false positive, while FDR controls the proportion of false positives.

### Causal Inference
A causal graph framework was used to infer relationships between variables based on correlation structure.

Variables were identified through:
- Strength of correlations
- Conditional independence
- Structural assumptions

Validation was performed using partial correlation to assess conditional independence.

### Summary
This project demonstrates how statistical modeling techniques can be used to:
- Analyze relationships between variables
- Evaluate model validity
- Interpret statistical results
- Infer potential causal structures

The focus is on conceptual understanding and analytical reasoning rather than implementation.

## 📝 Notes
- **Implementation**: Analysis was conducted using MATLAB  
- **Context**: This work was completed as part of a technical assessment during a research internship  
- **Data Privacy**: Proprietary datasets and assignment materials are not included  

## 📚 References
- Montgomery, D. C., et al. (2021). *Introduction to Linear Regression Analysis*  
- Pearl, J., et al. (2016). *Causal Inference in Statistics: A Primer*  
- Ai, C., & Norton, E. C. (2003). *Interaction terms in logit and probit models*  
