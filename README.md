# Temperature Forecasting using Prophet

## 1. Introduction
This project focuses on time series forecasting of daily minimum temperatures in Melbourne, Australia (1981-1990) using the Prophet model. The goal is to analyze historical temperature trends and make future predictions.

## 2. Data Overview

Dataset: "daily-minimum-temperatures-in-me.csv"

Number of records: 3,650

Columns:

Date: The date of the recorded temperature.

Daily Minimum Temperature: The lowest recorded temperature for that day.

No missing values were found, but there were issues with non-numeric temperature values.

## 3. Data Preprocessing

Converted the "Date" column to datetime format.

Renamed columns to match Prophet’s required format (ds for dates and y for values).

Addressed invalid entries in the temperature column (e.g., '?0.2'), replacing them with NaN and applying interpolation.

Converted temperature values to float for proper analysis.

## 4. Model Implementation (Prophet)

Installed and imported Prophet from prophet.

Split the data into training and testing sets.

Initialized and trained the Prophet model.

Generated future predictions for the next period.

Visualized the trends and seasonal patterns.

## 5. Issues Encountered and Fixes

Data Type Conversion Error: Some values were improperly formatted, leading to conversion errors.

Fix: Replaced invalid values with NaN and used interpolation.

Import Error: from Prophet import Prophet resulted in an error.

Fix: Used from prophet import Prophet.

## 6. Results & Insights

Forecasted daily minimum temperatures for future dates.

Identified seasonal trends and long-term variations.

Prophet effectively captured yearly seasonality and trends.

## 7. Conclusion & Recommendations

The Prophet model successfully predicted temperature trends.

Future work can include:

Evaluating model performance with RMSE.

Exploring alternative models like LSTMs or ARIMA.

Incorporating additional features like humidity and wind speed for better accuracy.
