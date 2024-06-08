# Data Analysis Process

## Business Task
1. Identify trends in smart device usage.
2. Find out applications of the trends.
3. Determine influence from the trends over marketing strategy.

## Data Sources
Original source: https://www.kaggle.com/datasets/arashnic/fitbit
Data source in this repository:
- `/fitbit_dataset/20160312-20160411/*.csv`
  - Data in this directory is not used for this analysis.
- `/fitbit_dataset/20160412-20160512/*.csv`
  - Data used for this analysis:
    - `dailyActivity_merged.csv`
    - `heartrate_seconds_merged.csv`
    - `sleepDay_merged.csv`
    - `weightLogInfo_merged.csv`

## Data Cleaning Process
1. Check if all relevant datasets have Id column.
2. Format each Date columnn to have the same name "Date" and same format.
   1. Format: "YYYY-mm-dd" or "YYYY-mm-dd hh:mm:ss" where hh is in 24h notation.
3. Drop irrelevant columns.
4. Drop duplicated rows.
5. Save cleaned data to `cleaned_data`