# Statistical Analysis and Causal Inference

This repository documents my implementation and interpretation of statistical models using MATLAB, based on simulated datasets. The focus is not on predictive performance, but on understanding how model structure, statistical assumptions, and data relationships affect interpretation.

---

## 📌 Overview

I performed regression analysis, multicollinearity diagnostics, hypothesis testing under multiple comparisons, and causal inference using correlation structure and conditional independence.

All analyses were conducted on simulated datasets provided for a technical assignment.

---

## 📊 Regression Analysis

### Multiple Linear Regression

I constructed a multiple linear regression model to explain jump height (y) using:

* x1: height
* x2: weight
* x3: language score

#### Results

* Height (x1): significant positive effect (p < 0.001)
* Weight (x2): significant negative effect (p < 0.001)
* Language score (x3): not significant (p = 0.902)

#### Interpretation

The results indicate that jump height is primarily determined by physical variables (height and weight), while language score does not have a statistically meaningful relationship with the outcome.

---

### Multicollinearity Diagnostics

To ensure the reliability of coefficient interpretation, I examined multicollinearity:

* Correlation matrix: all |r| < 0.1
* Variance Inflation Factor (VIF): all < 5
* Condition index: between 1.00 and 1.09

#### Interpretation

These results indicate no significant multicollinearity. Therefore, each predictor contributes independently, and coefficient estimates can be interpreted without instability concerns.

---

## 📈 Logistic Regression

I constructed a logistic regression model to predict infection status (binary outcome):

* x1: body temperature
* x2: cough frequency
* x3: public exposure

#### Results

* Temperature (x1): significant (p < 0.001)
* Cough frequency (x2): significant (p < 0.001)
* Public exposure (x3): not significant (p = 0.3425)

#### Interpretation

Physiological variables (temperature and cough frequency) are strong predictors of infection probability, whereas behavioral exposure (public visits) is not statistically significant in this dataset.

---

## ⚠️ Multiple Comparison

When testing multiple hypotheses simultaneously, Type I error increases as the number of tests increases.

To address this, I examined:

* Familywise Error Rate (FWER): controls probability of at least one false positive
* False Discovery Rate (FDR): controls proportion of false positives

#### Interpretation

FWER provides stricter control but can reduce statistical power, while FDR allows more discoveries at the cost of tolerating some false positives.

---

## 🔗 Causal Inference

### Variable Identification

The dataset contains seven variables following a predefined causal graph, where only θ is labeled. The remaining variables were identified based on correlation structure.

Using correlation analysis:

* Variable with strongest correlation with θ → identified as **s**
* Intermediate correlations used to infer **v**
* Remaining variables assigned based on relational structure

Final mapping:

* x6 = s
* x1 = Us
* x3 = v
* x5 = Uv
* x2 = r
* x4 = Ur

---

### Validation using Conditional Independence

To validate the inferred structure, I tested conditional independence using partial correlation.

#### Chain structure (θ → s → v)

* partialcorr(θ, v | s) ≈ 0
  → confirms conditional independence

#### Collider structure (r → v ← s)

* partialcorr(r, s | v) > 0
  → dependence induced after conditioning

#### Interpretation

The results are consistent with causal graph rules (chain and collider structures), supporting the validity of the inferred variable identities.

---

## 🛠 Implementation

* Environment: MATLAB
* Methods:

  * Ordinary Least Squares (OLS)
  * Logistic regression
  * Correlation analysis
  * Variance Inflation Factor (VIF)
  * Condition index
  * Partial correlation

---

## 📝 Notes

* The dataset is simulated and does not reflect real-world phenomena
* The focus of this project is on interpretation and reasoning, not prediction
* All conclusions are limited to the given data structure

---

## 📚 References

* Montgomery, D. C., et al. (2021). *Introduction to Linear Regression Analysis*
* Pearl, J., et al. (2016). *Causal Inference in Statistics: A Primer*
* Ai, C., & Norton, E. C. (2003). *Interaction terms in logit and probit models*

---
