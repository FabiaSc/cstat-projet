# Computational Statistics - House Prices Project - Group 3
Maillefer Leila, Schreyer Fabia, Strübi Loan

## Objective  
This project analyzes factors influencing house prices using statistical methods learned in our course. Our goals were to identify key predictors and build interpretable models trying to forecast house prices.

## Data Preprocessing  
- Initial exploration of the dataset;  
- Missing values handling; 
- Converted categorical variables to binary dummy variables via one-hot encoding;
- Selected relevant features by combining correlation filtering and Recursive Feature Elimination (RFE) - (narrowing from 81 to 10 key variables).

## Statistical Analysis & Modeling  
- Tested hypotheses on individual variables to confirm their relevance;
- Applied a \(2^5\) fractional factorial design and ANOVA to explore main effects and interactions among binarized features;
- Built multiple regression models:  
  - **Model 1**: Factorial regression on grouped means (binarized variables);
  - **Model 2**: Linear regression on original variables with log-transformed target;
  - **Model 3**: Enhanced Model 2 with polynomial terms and refined variable selection.

## Time Series Analysis  
- Aggregated sale prices monthly to build a time series spanning 55 months;
- Conducted stationarity tests (ADF) and seasonal decomposition;
- Fitted SARIMA models on both raw and smoothed data to capture temporal trends and seasonality;
- Compared models for stability and predictive performance, finding the smoothed SARIMA(0,1,1) model trying to balance responsiveness and robustness.

## Results  
- The regression models, especially Model 3, showed good predictive power and statistical validity;
- The SARIMA models complemented the analysis by incorporating temporal dynamics;
- Test predictions from both regression models aligned well with expected price distributions.

## Conclusion  
This project applied a range of statistical techniques to understand and predict house prices. The results offer an interpretable framework that meets our objectives effectively.
