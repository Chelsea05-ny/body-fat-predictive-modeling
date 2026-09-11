# Predictive Modeling & Statistical Analysis of Body Fat Percentage

## Project Overview

This project applies statistical modeling and quantitative analysis to predict body fat percentage using physical characteristics collected from a sample of 50 gym members.

The analysis evaluates eight potential predictors:

* Age
* Weight
* Height
* Neck size
* Chest size
* Abdomen size
* Hip size
* Thigh size

The project uses multiple linear regression, hypothesis testing, ANOVA, correlation analysis, multicollinearity assessment, and stepwise regression to develop a more efficient predictive model.

**Tools:** Microsoft Excel
**Course:** QNT 2020 — Quantitative Analysis & Mathematical Modeling
**Institution:** Baruch College
**Project Type:** Team Project

---

## Objective

The objective was to develop a regression model capable of predicting a gym member's body fat percentage based on measurable physical characteristics.

The analysis followed a structured modeling process:

1. **Logic** — Evaluated individual relationships between predictors and body fat percentage using bivariate regression and scatter plots.
2. **Fit** — Developed a multiple linear regression model using all eight predictors.
3. **Parsimony** — Evaluated predictor significance using p-values and a 0.05 significance level.
4. **Stability** — Examined correlations between predictors to identify potential multicollinearity.
5. **Model Selection** — Applied forward and backward stepwise regression to refine the model.
6. **Improvement** — Tested an alternative binary encoding of age to determine whether it improved model performance.
7. **Prediction** — Applied the final regression equation to estimate body fat percentage for a sample gym member.

---

## Statistical Methods

### Bivariate Regression

Individual regression models were constructed to examine the relationship between each predictor and body fat percentage.

The analysis considered:

* Regression coefficients
* R²
* F-statistics
* Significance F
* Scatter plots

### Multiple Linear Regression

A multiple regression model was developed using all eight predictors. The initial model produced an **R² of 0.8412**, indicating that approximately 84% of the variation in body fat percentage was explained by the predictors included in the model.

### Hypothesis Testing & ANOVA

ANOVA and F-tests were used to evaluate the statistical significance of the regression model.

The analysis used a **0.05 significance level** and calculated the F-critical value in Excel using:

`F.INV.RT(0.05,8,41)`

The resulting F-critical value was approximately **2.17**, compared with an F-statistic of **27.14**, supporting the significance of the overall regression model.

### Multicollinearity Analysis

A correlation matrix was used to evaluate relationships among the predictor variables. The analysis identified substantial correlations between several predictors, indicating potential multicollinearity and motivating the removal of redundant variables from the final model.

### Forward Stepwise Regression

Forward stepwise regression was used to identify predictors that contributed significantly to the model.

The variables selected were:

1. **Abdomen**
2. **Weight**
3. **Thigh**

After these three variables were included, the remaining predictors did not meet the 0.05 significance threshold.

### Backward Stepwise Regression

Backward stepwise regression was also performed by sequentially removing predictors with higher p-values while evaluating model performance using Adjusted R².

The process ultimately removed:

* Chest
* Height
* Neck
* Hip
* Age

This resulted in the same three-predictor model consisting of **weight, abdomen, and thigh**.

---

## Final Model

The final regression model uses:

* Weight
* Abdomen size
* Thigh size

These variables were identified as the most significant predictors through the model-selection process.

The final model was used to predict body fat percentage for a sample gym member using the individual's measured physical characteristics.

---

## Key Skills Demonstrated

### Data Analysis

* Quantitative data analysis
* Statistical modeling
* Regression analysis
* Data interpretation
* Correlation analysis

### Statistical Techniques

* Multiple linear regression
* Bivariate regression
* ANOVA
* F-tests
* Hypothesis testing
* p-value analysis
* R² and Adjusted R²
* Multicollinearity assessment
* Forward stepwise regression
* Backward stepwise regression

### Technical Skills

* Microsoft Excel
* Regression analysis tools
* Excel statistical functions
* Data organization
* Formula-based analysis
* Data visualization

### Analytical Skills

* Feature selection
* Model refinement
* Predictor evaluation
* Statistical significance testing
* Comparative model evaluation
* Data-driven decision making

---

## Project Files

### `analysis/`

Contains the Excel workbook used to perform the regression analysis, statistical calculations, model-selection procedures, and prediction.

### `report/`

Contains the final written project report documenting the methodology, statistical analysis, findings, and final model.

---

## Key Takeaway

This project demonstrates how statistical modeling can be used to transform a dataset containing multiple physical characteristics into a more focused predictive model. Through regression analysis, hypothesis testing, correlation analysis, and stepwise feature selection, the project reduced the original eight predictors to three variables used in the final model.
