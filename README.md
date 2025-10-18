# Health Expenditure Analysis
# Overview

This project analyzes the determinants of total health expenditure per capita using cross-country data. The study investigates the relationship between health expenditure, GDP per capita, and the share of population aged 65 and older. The analysis includes linear regression modeling, diagnostic tests, and functional form adjustments to ensure robust results.

# 1. Data Exploration

Loads a dataset containing health expenditure, GDP, and percentage of population aged 65+.

Explores the scale and distribution of variables.

Plots bivariate relationships to visually inspect correlations between health expenditure and GDP, and health expenditure and the elderly population share.

# 2. Linear Regression Model

Estimates a linear model where health expenditure depends on GDP and the proportion of elderly population.

Presents regression results in a tabular format.

Assesses statistical significance of individual variables using t-tests.

Conducts F-tests to evaluate joint significance of explanatory variables.

# 3. Diagnostic Tests

Tests for heteroskedasticity using graphical methods and the Breusch-Pagan test.

If heteroskedasticity is present, robust standard errors are computed and compared to the original model.

Uses the RESET test to check the functional form of the model.

Identifies potential outliers that may influence regression results.

# 4. Model Adjustment

Based on diagnostic tests, a logarithmic transformation is applied to health expenditure and GDP to improve linearity and model fit.

Compares original and transformed models to ensure functional form is appropriate.

#Key Findings

GDP per capita is highly significant in explaining health expenditure.

The proportion of elderly population is not individually significant in the baseline model.

Heteroskedasticity is present, requiring robust standard errors.

Logarithmic transformations improve model fit and functional form.

Outlier countries exist at both extremes, potentially influencing results.

# Tools and Packages Used

dplyr, readr – Data manipulation and loading

ggplot2, lattice – Visualization of relationships and model diagnostics

stargazer – Tabular presentation of regression results

lmtest – Diagnostic tests including Breusch-Pagan and RESET
