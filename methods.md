


# Methodology

## Compare parameters for inclusion in models to test

* Find model of each “size” with best RSS
* Calculate chosen metric for each
* Pick the “best” model

Perform AIC, BIC, Adjusted R^2

Compare models with ExtractAIC

## Model

* Family: Linear (using the lm(*) function)
    * Check Assumptions
        * Linear - Fitted vs. Residual plot, Scatterplot
        * Independent or IID - hard to test for
        * Normally distributed - The Q-Q Plot, Histograms, Shapiro-Wilk
        * Equal Variance - Fitted vs. Residuals plot, BP Test
    * Dig into parameters for
        * Residual diagnostics
        * Outlier diagnostics
        * Interaction
* Form
    * Predictors - which ones?  
    * Transformations - Take log of some predictors?
    * Interactions - Two-way interactions of predictors?
* Fit
    * Minimizing the least square error RMSE



## Test train split

Set.seed(420) to reproduce.

Some integer representing 80%

Split into two parts.


## Selected Models - Detect over-fitting and under-fitting

Compare the selected models with LOOCV

If a larger model has a higher RMSE-LOOCV then we want the smaller model.

There is a function for this in: https://www.coursera.org/learn/stat-420/lecture/xiK3R/cross-validation-in-r

Compare models with ANOVA

## Test-train output

Create a table for the output on the test and the training data.

