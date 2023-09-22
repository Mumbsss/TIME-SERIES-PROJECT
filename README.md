# TIME-SERIES-PROJECT
### BUSINESS UNDERSTANDING
Real estate investment is a significant financial decision that requires careful analysis and strategic planning. In this project, we embark on a comprehensive exploration of real estate investment opportunities in four diverse and dynamic cities: Chicago, New York, Houston, and San Francisco. Our aim is to provide valuable insights and data-driven guidance to potential real estate investors who are considering property investments in these cities over the next decade.

The project involves a multifaceted approach, encompassing data collection, preprocessing, time series analysis, and forecasting. We begin by sourcing and preparing real-world data, focusing on key metrics such as Return on Investment (ROI), property values, and rental income. Using advanced statistical techniques, including the ARIMA model, we analyze historical ROI data to uncover trends, patterns, and potential risks associated with real estate investments in each city.
### PROBLEM STATEMENT
Real estate investment is a complex and potentially lucrative endeavor, with numerous factors influencing the decision-making process. Investors seeking to allocate their capital in the real estate markets of major cities face several critical challenges and uncertainties. We have been therefore appointed by an investor as a Data scientist to give them insights to their overarching problem addressed by this project can be defined as follows:

Investor Uncertainty and Risk Mitigation: Investors are often confronted with uncertainty about where and when to invest their resources in real estate properties. Decisions regarding property acquisition and management must navigate a dynamic landscape of market conditions, economic trends, regulatory changes, and shifting investor goals. Moreover, the longevity of real estate investments, often spanning years or even decades, necessitates a forward-looking approach that mitigates risks while maximizing returns.
There are other subquestions to be addressed which include:

ROI Assessment: Investors need reliable methods to assess the historical performance of potential real estate investments, particularly Return on Investment (ROI). Understanding ROI trends is crucial for predicting future returns and making informed investment choices.

Risk Identification: Investors must identify and evaluate the risks associated with specific cities or regions. Factors such as economic stability, market volatility, regulatory changes, and unforeseen events can significantly impact the return on investment.

Long-Term Planning: Investors require insights into long-term ROI trends to make strategic investment decisions that align with their financial goals, whether they prioritize capital appreciation, rental income, or a balanced approach.

Diversification Strategy: Determining the optimal allocation of resources across multiple cities is a complex task. Investors seek guidance on how to diversify their portfolios to manage risk effectively while optimizing returns.

Market Conditions: An understanding of current and projected market conditions in chosen cities is crucial. Factors like property values, rental yields, demand, and supply directly influence investment decisions.
### BUSINESS OBJECTIVES
The objective of this project is to address the problem of investor uncertainty and risk mitigation in real estate investments by providing data-driven insights, forecasting, and analysis. By doing so, we aim to assist the investors in making informed decisions regarding property investments in the four selected cities over the next decade.
### Key Deliverables:

Historical ROI analysis for each city.

Identification and assessment of potential risks associated with real estate investments.

Long-term ROI forecasts to aid strategic planning.

Recommendations on diversification strategies.

Insights into current market conditions in Chicago, New York, Houston, and San Francisco
### Success Criteria:

The success of this project will be measured by its ability to provide investors with actionable information, enabling them to make well-informed real estate investment decisions that align with their financial objectives, risk tolerance, and time horizons. Success will also be gauged by the project's capacity to enhance investors' understanding of the selected cities' real estate markets and how they evolve over time.
###  DATA UNDRSTANDING

Our data set is the Zillow dataset. The Data set collected is from the year 1996 to 2018.

The data has 8 features;

RegionID
RgionName
City
State
Metro
CountyName
SizeRank
Time
Value
### MODEL IMPLEMENTED
We made use of the ARIMA model
### EVALUATION
ROI
### Interpreting Results
## Model Information:

Dependent Variable (Dep. Variable): This is the variable you are trying to predict or model, which is 'ROI' in this case.

No. Observations: The number of data points used in the model, which is 162.

Model: The type of model used, which is ARIMA(1, 1, 1). This represents an AutoRegressive Integrated Moving Average model with orders (p=1, d=1, q=1).

Date: The date and time when the model was run.


## Summary Table:

The summary table provides coefficients for the ARIMA model.

ar.L1: The coefficient for the autoregressive (AR) lag 1 term. In your model, it's 0.0405.

ma.L1: The coefficient for the moving average (MA) lag 1 term. In your model, it's -0.9947.

sigma2: The estimated variance of the model's residuals, which is 3.319e+10.
AIC, BIC, and HQIC:

These are information criteria used for model comparison and selection.

AIC (Akaike Information Criterion): AIC is a measure of how well the model fits the data while penalizing complexity. Lower AIC values are preferred.

BIC (Bayesian Information Criterion): Similar to AIC but with a stronger penalty for model complexity. Lower BIC values are preferred.

HQIC (Hannan-Quinn Information Criterion): Another information criterion for model selection. Like AIC and BIC, lower values are preferred.

## Ljung-Box (L1) (Q) and Jarque-Bera (JB):

These are statistical tests and diagnostics to check the model's assumptions.

Ljung-Box (L1) (Q): A test for autocorrelation in the residuals. In your case, it's 0.00, which suggests that there is no significant autocorrelation in the residuals.

Jarque-Bera (JB): A test for the normality of the residuals. In your case, it's 13.48, with a low p-value (0.00), indicating that the residuals may not be normally distributed
## Heteroskedasticity (H):

This tests for heteroskedasticity, which is the presence of non-constant variance in the residuals. In your case, the result is 1.50, which is not extremely high.

## Skew and Kurtosis:

Skew measures the asymmetry of the residuals, and kurtosis measures the "tailedness" of the distribution. In your case, skew is 0.16, and kurtosis is 1.62.

## Interpretation:

The ARIMA(1, 1, 1) model has been fitted to the ROI data.

The coefficients for AR(1) and MA(1) are estimated as 0.0405 and -0.9947, respectively. These coefficients are relatively small, indicating that the influence of the previous value and the previous error on the current ROI is modest.

The estimated variance of the residuals is 3.319e+10.

The Ljung-Box test does not show significant autocorrelation in the residuals, suggesting that the model captures the temporal dependencies well.

The Jarque-Bera test indicates that the residuals may not be normally distributed, which could be an area for further investigation.

Overall, this ARIMA model has been fitted to your ROI data, and the results suggest that it captures the temporal dependencies to some extent

### RECOMMENDATIONS

Exploring different ARIMA orders (p, d, q) to see if a better-fitting model can be found.

Testing alternative time series models such as SARIMA or more complex models.

Investigating data transformations or detrending techniques to address potential non-stationarity or distributional issues in the data.

Conducting out-of-sample forecasting and evaluating the model's predictive performance on new data to assess its practical utility.
