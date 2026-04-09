# Statistical Analysis and Modeling

This repository presents an overview of fundamental statistical concepts and modeling approaches using MATLAB.

## Contents
- Multiple linear regression analysis
- Logistic regression analysis
- Multicollinearity (correlation matrix, VIF, condition index)
- Interaction effects in regression models
- Multiple comparison (Type I/II error, FWER, FDR)
- Basic causal inference using correlation structure

## Focus
This project emphasizes:
- Understanding relationships between variables
- Interpreting statistical model outputs
- Identifying potential issues such as multicollinearity
- Applying statistical reasoning to model evaluation

## Methods
- Ordinary Least Squares (OLS)
- Logistic Regression
- Variance Inflation Factor (VIF)
- Correlation analysis
- Hypothesis testing
- Multiple comparison correction methods

## Analysis Summary

### Regression Analysis
A multiple linear regression model was used to examine the relationship between variables. Some predictors showed meaningful associations with the outcome, while others did not contribute significantly.

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

## Notes
This work was conducted as part of a technical assessment during an internship.  
The repository focuses on conceptual understanding and interpretation rather than implementation.

All datasets and proprietary materials are not included.
