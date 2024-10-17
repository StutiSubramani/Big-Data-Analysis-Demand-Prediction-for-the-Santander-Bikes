# Demand Prediction for the Santander Bikes across London

## Project Overview

This is a machine learning-driven project aimed at forecasting the demand and revenue for Santander Cycles, London's public bike-sharing service. By leveraging historical cycling data, weather conditions, and public transport proximity, this project seeks to optimize bike availability and operational efficiency. It provide actionable insights to support sustainable urban mobility by encouraging eco-friendly transportation and improving resource allocation.

## Objectives

Predict demand for Santander bikes across London, considering environmental factors, public transport proximity, and seasonal trends.
Forecast revenue from bike rentals to help optimize pricing strategies and operational decisions.
Support urban mobility planning by analyzing the integration of cycling with public transportation networks, offering suggestions for enhancing commuter experience and sustainability.

## Methods

Data Integration: Collected and preprocessed large datasets using PySpark on Google Cloud Platform (GCP). 
Key data sources include:
Cycling usage: Historical hire data for Santander Cycles.
Weather conditions: To capture weather impact on cycling behavior.
Transport proximity: Geospatial data from BigQuery GIS to analyze the effect of nearby bus and tube stations on bike usage.
#### Exploratory Data Analysis (EDA): 
Performed extensive EDA to uncover patterns and correlations between cycling demand, weather conditions, and proximity to public transport. Geospatial analysis highlighted key commuter hotspots and interdependence between cycling and public transport.
#### Machine Learning Models:
Demand Prediction: Models including Gradient Boosted Trees (GBT), Random Forests, and Linear Regression were used, with GBT achieving the highest accuracy in capturing the complex non-linear relationships.
Revenue Forecasting: Time-series models such as SARIMA, ARIMA, and LSTM were implemented. The SARIMA model provided the most accurate revenue forecasts with the lowest RMSE.

## Key Results

For demand prediction, the Gradient Boosted Trees (GBT) model delivered the highest accuracy, achieving an RMSE of 435.066, surpassing both Linear Regression and Random Forest models. In revenue forecasting, the SARIMA model performed the best with an RMSE of 321.350, closely followed by the LSTM model at 327.863. These predictive models offer crucial insights for optimizing bike availability, refining revenue strategies, and enhancing sustainable urban mobility in London.

## Data Source

The datasets used in this project are publicly available on BigQuery, including:

Cycle Hire Data: 12 variables covering historical bike hires (~9.4 GB)
Cycle Stations Data: Information about bike station locations and usage

## Tools & Technologies

Big Data Processing: PySpark on GCP
Geospatial Analysis: BigQuery GIS
Machine Learning: Gradient Boosted Trees (GBT), Random Forests, ARIMA, SARIMA, and LSTM models.

### Link of the Dataset: 
https://console.cloud.google.com/bigquery?p=bigquery-public-data&d=london_bicycles&page=dataset&project=angular-stacker-408217&ws=!1m5!1m4!4m3!1sbigquery-public-data!2slondon_bicycles!3scycle_hire 

