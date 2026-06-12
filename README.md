# Real-time PM2.5 Concentration Forecasting System

A real-time air quality forecasting platform designed to predict PM2.5 concentrations using statistical and deep learning models within a Big Data architecture. The system integrates data streaming, distributed processing, model inference, and interactive visualization to provide continuous air quality monitoring and forecasting.

## Live Demo

**Dashboard:** 

[![Streamlit App](https://img.shields.io/badge/Streamlit-Demo-red?logo=streamlit)](https://pm25-forecast-dashboard.streamlit.app/)

## System Architecture

Kafka → Spark Structured Streaming → Forecasting Models → Cassandra → Streamlit Dashboard

The platform continuously ingests air quality data, processes streaming records using Apache Spark, generates PM2.5 forecasts, stores prediction results in Cassandra, and visualizes outputs through an interactive dashboard.

## Key Features

### Real-Time Data Processing

* Stream ingestion and processing using Apache Kafka and Spark Structured Streaming.
* Continuous generation of PM2.5 predictions from incoming environmental measurements.
* Scalable architecture suitable for high-volume sensor data.

### Forecasting Models

Implemented and evaluated multiple forecasting approaches:

**Statistical Models**

* AutoRegressive (AR)
* SARIMA
* Holt-Winters
* Prophet

**Deep Learning Models**

* Vanilla LSTM
* Stacked LSTM
* Bidirectional LSTM
* CNN-LSTM
* GRU
* Hybrid Deep Learning Model

Model performance is evaluated using:

* RMSE (Root Mean Squared Error)
* MAE (Mean Absolute Error)
* MAPE (Mean Absolute Percentage Error)

### Interactive Dashboard

* Real-time PM2.5 prediction interface.
* Actual vs Predicted visualization.
* Comparative model performance analysis.
* Forecast quality metrics and trend monitoring.
* Dataset and pipeline overview.

## Dataset

**Source:** Air Quality India Dataset (Kaggle)

* 29,531 observations
* 26 cities across India
* Data period: 2015–2020
* Air pollutant measurements including PM10, NOx, NO2, NH3, and PM2.5

## Technology Stack

| Layer                | Technologies                           |
| -------------------- | -------------------------------------- |
| Programming Language | Python                                 |
| Data Streaming       | Apache Kafka                           |
| Stream Processing    | Apache Spark Structured Streaming      |
| Data Storage         | Apache Cassandra                       |
| Forecasting          | Statsmodels, Prophet, TensorFlow/Keras |
| Visualization        | Streamlit                              |

## Project Outcomes

* Developed an end-to-end real-time forecasting pipeline for air quality monitoring.
* Compared traditional statistical forecasting techniques with deep learning architectures.
* Demonstrated the integration of Big Data technologies for real-time environmental analytics.
* Delivered an interactive dashboard for monitoring and evaluating forecast performance.
