# Time Series Analysis and Forecasting

This repository contains R code and datasets for time series analysis and forecasting. The analysis is performed on three different datasets: `electricity.csv`, `plastics.csv`, and `visitors.csv`. The goal is to understand the underlying patterns, trends, and seasonality in the data, and to develop forecasting models for future predictions.

## Files

1. **Timeseries.Rmd**: R Markdown file containing the code for time series analysis and forecasting.

2. **timeseriesknit.pdf**: Compiled PDF document generated from the R Markdown file, providing a detailed explanation of the analysis, model selection, and forecasting results.

3. **electricity.csv**: Dataset containing monthly electricity generation data.

4. **plastics.csv**: Dataset with monthly sales data for a plastic product.

5. **visitors.csv**: Dataset containing monthly visitor counts.

## Analysis Highlights

### Electricity Dataset

- **Decomposition:** The dataset is decomposed into trend, seasonal, and random components. The trend indicates a long-term increasing pattern, and seasonality is observed with peaks in summer and winter.

- **Transformation:** Box-Cox and log transformations are explored to stabilize variance and handle non-stationarity.

- **Modeling:** ARIMA models are fitted, and the best model (ARIMA(0,1,2)(3,1,0)) is selected based on AIC values and residual analysis.

- **Forecasting:** The selected model is used to forecast electricity generation for the next 180 months.

### Plastics Dataset

- **Seasonal Subseries Plot:** Seasonal patterns are identified, showing a spike in sales every August.

- **Classical Decomposition:** Decomposition is performed to reveal trend and seasonality. Outliers are introduced to demonstrate their impact on seasonally adjusted data.

- **Model Comparison:** Different forecasting models (Mean, Naive, Seasonal Naive, Drift) are compared using accuracy metrics. Seasonal Naive is identified as the most effective model.

### Visitors Dataset

- **Visual Inspection:** Time series plots, seasonal subseries plots, and autocorrelation function (ACF) plots are used to identify trends, seasonality, and outliers.

- **Transformations:** Box-Cox and log transformations are applied to stabilize variance.

- **Modeling:** ETS models and ARIMA models are fitted. The best model (ETS(A,N,M)) is selected based on AIC values.

- **Forecasting:** The selected model is used to forecast visitor counts for the next 16 months.

## Conclusion

- Accurate forecasting models are crucial for understanding and predicting trends in various datasets.

- Model selection should be based on a combination of visual inspection, statistical tests, and accuracy metrics.

- Continuous monitoring and retraining of models may be necessary for long-term forecasting accuracy.