# Demand-Forecasting

### Goal
Develop a demand forecasting system for a short-term period (14 days) starting from 7 days after the last date in the data, for all product groups.

### Description:
1. Using the provided transaction data, create two forecasting models:
- Machine learning model.
- Classical time series forecasting model.
2. Provide justified comments regarding the choice of methods and approaches, explaining why you chose them.
3. Provide a script or notebook (.py/.ipynb) containing the technical solution and the ability to calculate the forecast for the future period (scoring).

### Expected result
A file with code (.py or .ipynb) that includes two forecasting models, explanations of method choices, and the ability to calculate the forecast for the future period.

##### Final thoughts
ARIMA could be advantageous for this task if individual product categories exhibit strong seasonal patterns or clear trends over time, but it may struggle with categories that have irregular sales patterns or are influenced by factors not captured in the time series alone.
XGBoost ability to handle categorical variables (like product categories) and derive complex interactions between features makes it well-suited for this dataset, potentially capturing nuanced relationships between product types, time-based features, and demand that ARIMA might miss.
XGBoost does not require a model for each of the categories, however I did it to achieve the best possible MAE per product category.