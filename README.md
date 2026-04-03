# Electricity Load Forecasting (Austria → Multi-Country)

## Project Overview

This project focuses on forecasting electricity load using historical data and machine learning / deep learning models.

We start with **Austria** and later extend the framework to multiple countries.

---

## Objective

* Forecast **24-hour ahead electricity load**
* Compare:

  * Statistical models
  * Machine Learning models
  * Deep Learning models
* Build a **scalable forecasting pipeline**

---

## Data

Source: Open Power System Data (OPSD)

* Country: Austria
* Time resolution: Hourly
* History: ~5 years

---

## Features

* Lag features (t-1, t-24, t-168)
* Rolling statistics (24h mean)
* Time features (hour, weekday, month)
* Holiday indicators
* Seasonal categories

---

## Models

### Baseline

* Naive forecast
* Linear Regression
* ARIMA / SARIMA

### Machine Learning

* Random Forest
* XGBoost
* MLP

### Deep Learning

* RNN
* LSTM
* GRU

---

## Evaluation Metrics

* MAE
* RMSE
* MAPE
* R²

---

## Project Structure

* `data/` → raw and processed datasets
* `notebooks/` → experiments and exploration
* `src/` → reusable pipeline code
* `configs/` → country-specific settings
* `results/` → outputs, plots, metrics

---

## Workflow

1. Data understanding (`notebooks/01_*`)
2. Feature engineering (`notebooks/02_*`)
3. Baselines (`notebooks/03_*`)
4. ML models (`notebooks/04_*`)
5. DL models (`notebooks/05_*`)

---

## Future Work

* Extend to multiple countries
* Add weather & renewable features
* Compare cross-country generalization


## Goal

Build a robust and scalable electricity load forecasting framework and analyze trade-offs between:

* Accuracy
* Interpretability
* Complexity
