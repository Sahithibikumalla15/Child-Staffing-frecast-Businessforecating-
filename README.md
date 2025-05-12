# Child Saving Institute - Business Forecasting Project

This project leverages statistical and machine learning methods to forecast staffing needs at the Child Saving Institute (CSI), a nonprofit childcare organization. Accurate forecasting ensures compliance with child-to-staff ratios while reducing unnecessary labor costs.

# TEAM MEMBERS
Sahithi Bikumalla
Vikas Kumar Reddy Buchammagari
Mahmuda Akhter Nishu

## Objectives

- *Clean and structure raw attendance data* from multiple Excel sources into a usable 30-minute interval format.
- *Convert attendance to staffing needs* using age-group-specific staff-to-child ratios.
- Generate:
  - *Typical Week Forecast* (average staffing pattern across weekdays).
  - *Next Calendar Week Forecast* (staff needs predicted for the upcoming Monday–Friday).
- Compare forecasting models:
  - *ARIMA*
  - *Random Forest Regressor*
  - *XGBoost Regressor*
- Evaluate model performance using:
  - MAE (Mean Absolute Error)
  - RMSE (Root Mean Squared Error)
  - MAPE (Mean Absolute Percentage Error)

## Data

- *Combined_ECEC_Spellman_DecodedRoom.csv*: Cleaned data with date, time, room, age group, number of children, and computed staff needed.
- *Featured CSVs*: Feature-enriched versions with time-based features (hour, weekday, timestamp, etc.) for ML models.

## Notebooks & Scripts

- Businessforecasting project.ipynb (this file includes data cleaning,typical weekforecast, Next week forecast , model evaluation)

## Visualizations

- Line plots: Daily staff needs per 30-min interval.
- Heatmaps: Weekly staff demand across weekdays and time blocks.
- Feature importance charts for ML models.

## Dependencies

```bash
pip install pandas numpy scikit-learn xgboost matplotlib seaborn holidays statsmodels
