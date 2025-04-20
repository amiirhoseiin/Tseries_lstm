Air Quality Detection using Time Series Analysis

This project explores time series forecasting techniques for predicting air quality using models like ARIMA, Prophet, and LSTM. It includes detailed preprocessing steps, stationarity checks, and model comparison based on forecasting accuracy.
📌 Project Overview

The primary objective of this notebook is to:

    Evaluate stationarity using the Augmented Dickey-Fuller (ADF) test.

    Apply differencing techniques if needed to achieve stationarity.

    Compare various forecasting models for Air Quality Index (AQI), including:

        Multiple Linear Regression (MLR)

        ARIMA

        Prophet

        LSTM

📊 Key Features

    📉 ADF Test: Checks the stationarity of the AQI time series.

    🔄 Differencing Strategy: Applies first or seasonal differencing based on visualizations and statistical tests.

    🧠 Model Training: Trains and compares multiple models to select the best based on MAPE (Mean Absolute Percentage Error).

    📦 Forecasting with Scalecast: Manages forecasting workflows with the scalecast package.

🧪 Libraries Used

This notebook makes use of the following libraries:

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from statsmodels.tsa.stattools import adfuller
from statsmodels.tsa.arima.model import ARIMA
from statsmodels.graphics.tsaplots import plot_acf, plot_pacf
from scalecast.Forecaster import Forecaster
from sklearn.metrics import mean_absolute_percentage_error
from tensorflow.keras.callbacks import EarlyStopping
from prophet import Prophet

📁 Project Structure

    Data Loading: Reads AQI data from Excel files.

    Exploratory Data Analysis (EDA): Visual inspection and decomposition of time series.

    Stationarity Testing: Performs ADF tests with iterative differencing.

    Modeling: Builds and trains LSTM, ARIMA, MLR, and Prophet models.

    Evaluation: Compares models using test set performance and visual plots.

🧠 Why This Project Matters

Air pollution is a critical public health concern. Accurate forecasting of air quality:

    Helps citizens plan daily activities safely.

    Assists policymakers in environmental decision-making.

    Enables proactive healthcare measures during pollution spikes.

By combining deep learning, classical time series models, and automated forecasting frameworks, this project demonstrates a robust methodology for predicting environmental metrics.
