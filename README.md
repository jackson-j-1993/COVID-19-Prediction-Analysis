# COVID-19-Prediction-Analysis
A healthcare data analysis and predictive modeling project that studies Johns Hopkins University COVID-19 data to forecast future confirmed cases and deaths for India. 

## Problem Statement

The purpose of this project is to study the COVID-19 data published by Johns Hopkins University and prepare a complete analysis report. Along with the analysis, the project also builds predictive models to forecast future confirmed cases and deaths for a selected country. For this project, **India** was selected as the country for analysis and prediction. India was chosen because it has a large COVID-19 history and its trend includes different pandemic phases, making it highly useful for both analysis and forecasting.

## Project Objectives

*   Prepare a complete data analysis report on the given COVID-19 dataset.
*   Forecast confirmed cases and deaths for a fixed future period.
*   Compare multiple machine learning models and recommend the best model.
*   Provide suggestions to the government health department based on the forecast.
*   Document the challenges faced and the techniques used to handle them.

## Datasets

The project utilizes two time-series datasets from Johns Hopkins University:
*   `time_series_covid19_confirmed_global.csv`
*   `time_series_covid19_deaths_global.csv`

These files contain country-wise cumulative COVID-19 confirmed cases and death cases recorded across multiple dates. 

### Data Transformation
The original wide-format datasets (where dates were represented as columns) were transformed into a clean time-series format with dates as rows for analysis and prediction. The final prepared dataset includes the following metrics:
*   Date
*   Confirmed Cases
*   Death Cases
*   Daily Confirmed Cases (calculated by subtracting the previous day's cumulative cases from the current day's)
*   Daily Death Cases
*   Mortality Rate (calculated as `Death Cases / Confirmed Cases * 100`)

## Tech Stack & Libraries

The following Python libraries are required for data handling, visualization, model building, and evaluation:
*   **pandas:** For working with tables, CSV files, and data transformation.
*   **numpy:** For numerical calculations.
*   **matplotlib & seaborn:** For creating charts and visualizing cumulative/daily trends.
*   **scikit-learn (`sklearn`):** For building and comparing machine learning models, including `LinearRegression`, `RandomForestRegressor`, and `GradientBoostingRegressor`, as well as evaluating them using metrics like Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared.
