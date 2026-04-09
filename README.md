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

This project explores fundamental statistical modeling concepts, including regression analysis, multicollinearity, hypothesis testing, and causal inference.

### Regression Analysis

A multiple linear regression model was used to examine the relationship between physical characteristics and performance outcomes. The analysis indicated that certain variables showed meaningful associations with the dependent variable, while others did not contribute significantly.

To ensure the reliability of the model, multicollinearity diagnostics were conducted. Based on correlation analysis, variance inflation factors (VIF), and condition indices, no significant multicollinearity issues were detected, suggesting that the predictors contributed independently to the model.

A logistic regression model was also applied to analyze binary outcomes. Some predictors were found to have significant effects on the probability of the outcome, while others did not demonstrate statistically meaningful relationships.

### Multicollinearity

Multicollinearity refers to high correlations among independent variables, which can lead to unstable coefficient estimates and misleading interpretations. :contentReference[oaicite:0]{index=0}  

Potential causes include:
- Data collection constraints
- Model specification issues
- Redundant or highly correlated predictors

To diagnose multicollinearity, several methods were considered:
- Correlation matrix analysis
- Variance Inflation Factor (VIF)
- Eigenvalue and condition index analysis

### Interaction Effects

Interaction terms were introduced to examine how the effect of one variable changes depending on the level of another variable. These terms allow the model to capture more complex relationships between predictors.

However, interpretation requires caution, particularly in nonlinear models, where interaction effects may vary across different values of the variables.

### Multiple Comparison

When conducting multiple hypothesis tests, the probability of making false discoveries increases. :contentReference[oaicite:1]{index=1}  

Two types of statistical errors were considered:
- Type I error: rejecting a true null hypothesis
- Type II error: failing to reject a false null hypothesis

To address multiple comparison problems, the following concepts were reviewed:
- Familywise Error Rate (FWER)
- False Discovery Rate (FDR)

FWER controls the probability of making at least one Type I error, while FDR controls the expected proportion of false positives among rejected hypotheses.

### Causal Inference

A causal graph framework was used to infer relationships among variables based on their correlation structure. :contentReference[oaicite:2]{index=2}  

Variables were identified by examining:
- Strength of correlations
- Conditional independence relationships
- Structural assumptions from causal graphs

Additional validation was performed using conditional correlation (partial correlation) to test independence under specific conditions.

---

## Summary

Overall, this project demonstrates how statistical modeling techniques can be used to:
- Analyze relationships between variables
- Evaluate model validity
- Interpret statistical results
- Infer potential causal structures from data

The focus is on conceptual understanding and analytical reasoning rather than implementation.

## Notes
This work was conducted as part of a technical assessment during an internship.
The repository focuses on conceptual understanding and interpretation rather than implementation.

All datasets and proprietary materials are not included.
