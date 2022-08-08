# 3_Chicago_Bivariate_Linear_Regression

## Project: Linear Regression (Bivariate)

### Skills and Tools

1. Utilize method of moments to develop a sophisticated comprehension of the slope and intercept parameters from a bivariate linear model.
2.  Evaluate bivariate linear model parameters and goodness of fit through the use of t-statistics, confidence intervals, and R-squared calculation.
3. Define the assumptions of linear regression, and explore how potential violations can be identified and subsequently correct perform hypothesis testing on linear model results.

     * Interperate Bivariate Linear Regression
     * Evaluate Bivariate Linear Regression
     * Assumptions of the Linear Model
     * Correlation vs. Causation

### Context
The linear model is a foundational statistical tool that enables performance of supervised modelling (creating a function that maps one or more explanatory variables to a specific target variable). Using the linear model, evaluate the correlation between pairs of variables and quantify the effect one variable has on another.

### Problem Statement
Develop linear model given the following:

1. City Regression:
    * Report and interpret the slope coefficient for salary.
    * Report and interpret the intercept coefficient for salary. 
    * Report the t-statistic and p-value for salary. 
    * Report and interpret the R-squared value.    
2. Suburb Regression
    * Report and interpret the slope coefficient for salary.
    * Report and interpret the intercept coefficient for salary. 
    * Report the t-statistic and p-value for salary. 
    * Report and interpret the R-squared value.
3. Compare and contrast the effect of salary of jewelry spend in these two different populations. Explain the difference in the slope coefficients in the two regressions?

### Algorithm Methodology
1. Load and Plot Both Sets of Data

2. City Regression:
    * Perform Regression / Obtain Summary (coefficients, T-stat, P-Value and R^2)
    * Plot Regression Line.
    * Verify Linearity of Model (against defining assumptions)
        - Normality of Residuals
           * Plot Histogram of Residuals
           * Plot Residuals against Predicted Jewelry Expenditure
           * Normal Q-Q Plot of Residual Values
        - Homoscedasticity - Constant Variance
    * Determine Confidence Level for B1
    * Evaluate Model Stability: Repeatedly Sample Data (Create 1,000 train/test splits)
        
        Do-Loop:
        - Create train/test sample
        - Perform linear regression model on training data
        - Save B1 coefficient
        - Calculate R^2 for test sample as squared correlation between Y from test and
            predicted values for test sample (Y^hat). Calculate % decrease.
        
        Post Do-Loop:
        - Histogram and Summary of drop in R^2
        - Evaluate B1 parameter / Build 95% Confidence Level
        - Conclusion
       
3. Suburb Regression:
    * Perform Regression / Obtain Summary (coefficients, T-stat, P-Value and R^2)
    * Plot Regression Line.
    * Verify Linearity of Model (against defining assumptions)
        - Normality of Residuals
            * Plot Histogram of Residuals
            * Plot Residuals against Predicted Jewelry Expenditure
            * Normal Q-Q Plot of Residual Values
        - Homoscedasticity - Constant Variance
    * Determine Confidence Level for B1
    * Evaluate Model Stability: Repeatedly Sample Data (Create 1,000 train/test splits)
        
        Do-Loop:
        - Create train/test sample
        - Perform linear regression model on training data
        - Save B1 coefficient
        - Calculate R^2 for test sample as squared correlation between Y from test and predicted values for test sample (Y^hat). Calculate % decrease.
        
        Post Do-Loop:
        - Histogram and Summary of drop in R^2
        - Evaluate B1 parameter / Build 95% Confidence Level
        - Conclusion
      
4. Model Comparison: City vs. Suburb


### Results
All code to complete this work is found in the attached [notebook](Module5_Homework.R) or with pictures [Word File](Module5_Homework.docx).



