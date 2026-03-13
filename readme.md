# Electricity Demand Prediction Project

## Overview

This project analyzes electricity demand and weather data to explore patterns and build features that help predict electricity demand. The goal is to understand how weather variables such as temperature, wind, and precipitation influence daily electricity usage.

The project combines electricity grid data with weather observations and performs exploratory data analysis (EDA) to identify relationships between variables before building predictive models.

---

## Data Sources

### Electricity Demand Data

Source: U.S. Energy Information Administration (EIA)

Contains daily information such as:

* Electricity demand value
* Balancing authority regions
* Time period information

### Weather Data

Source: NOAA weather stations

Weather variables include:

* AWND – Average wind speed
* PRCP – Precipitation
* TAVG – Average temperature
* TMAX – Maximum temperature
* TMIN – Minimum temperature

---

## Dataset Columns

| Column      | Description                          |
| ----------- | ------------------------------------ |
| period      | Time period of electricity data      |
| subba       | Sub balancing authority              |
| subba-name  | Name of the sub balancing authority  |
| parent      | Parent balancing authority           |
| parent-name | Parent authority name                |
| timezone    | Timezone of the record               |
| value       | Electricity demand (target variable) |
| DATE        | Weather observation date             |
| STATION     | Weather station ID                   |
| NAME        | Weather station name                 |
| AWND        | Average wind speed                   |
| PRCP        | Precipitation                        |
| TAVG        | Average temperature                  |
| TMAX        | Maximum temperature                  |
| TMIN        | Minimum temperature                  |

---

## Data Processing Steps

1. Load electricity and weather datasets
2. Convert date columns to datetime
3. Clean missing values
4. Remove unnecessary columns
5. Merge electricity demand data with weather data on date
6. Filter the dataset to the desired time range

---

## Feature Engineering


### Time-Based Features

* Month
* Day of week

These help capture seasonal and weekly patterns in electricity usage.

---

## Exploratory Data Analysis (EDA)

EDA was performed to understand the dataset and identify relationships between variables.

Key analyses include:

* Summary statistics
* Missing value analysis
* Distribution of electricity demand
* Correlation analysis between features
* Scatter plots comparing weather variables and electricity demand

### Visualizations

The project includes the following visualizations:

* Correlation heatmap
* Histogram of electricity demand
* Temperature vs demand scatter plot
* Feature correlation bar chart

These visualizations help identify which variables may be useful predictors.

---


## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib

---

## Future Work

Potential next steps for the project include:

* Building machine learning models to predict electricity demand
* Testing models such as Linear Regression, Random Forest, SVM, and Neural Networks

---

## Author

Timothy Mai
