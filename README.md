# Video-Game-Sales-Forecast
Market Forecasting: Methodology and Rationale
To provide actionable insights into future trends in the gaming industry, I developed a five-year forecast (2017–2021) for global annual video game sales using the vgsales.csv dataset.

Why forecasting?
Understanding historical sales is valuable, but anticipating market direction is crucial for publishers, investors, and strategists seeking to make informed decisions in a rapidly evolving industry.

How it was done:

Data Aggregation:
I aggregated annual global sales from 1980 to 2016, ensuring data completeness and temporal consistency by converting the year column to a PeriodIndex.

Model Selection:
To capture both long-term trends and cyclical effects, I employed a SARIMA (Seasonal ARIMA) model, using automated parameter selection (auto_arima) with annual seasonality (5-year cycles).

Model Fitting & Forecasting:
The SARIMAX model was fit to historical data, and forecasts were generated for the next five years, with confidence intervals to quantify uncertainty.

Interpretation:
The resulting forecast indicated a projected decline in global sales, highlighting potential challenges and opportunities for industry stakeholders.

This rigorous time series approach ensures the forecast is both statistically sound and directly relevant for strategic planning.
You can review the full implementation and code in the market_forecasting.ipynb notebook.
