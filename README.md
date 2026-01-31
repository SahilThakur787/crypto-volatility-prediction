# crypto-volatility-prediction
Machine learning project to predict cryptocurrency market volatility using historical OHLC data, volume, and market capitalization, with EDA, feature engineering, and model optimization.
🚀 Cryptocurrency Volatility Prediction Using Machine Learning
📌 Project Overview

Cryptocurrency markets are highly volatile, making risk management a major challenge for traders and financial institutions. This project focuses on predicting cryptocurrency market volatility using historical market data and machine learning techniques.
Instead of predicting prices, the model forecasts volatility, which directly reflects market risk and instability.

🎯 Problem Statement

Cryptocurrency markets experience frequent and extreme price fluctuations. Accurate volatility prediction helps in:

Risk management

Portfolio allocation

Trading strategy development

The objective of this project is to build and optimize a machine learning model that predicts cryptocurrency volatility using historical OHLC prices, trading volume, and market capitalization.

🛠️ Tech Stack

Programming Language: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn

Machine Learning: Scikit-learn

Model Optimization: GridSearchCV

Model Saving: Joblib

Environment: Jupyter Notebook / Google Colab

📂 Dataset Description

The dataset contains historical market data for multiple cryptocurrencies with the following features:

Date

Cryptocurrency Name

Open Price

High Price

Low Price

Close Price

Trading Volume

Market Capitalization

The dataset supports multi-cryptocurrency analysis, not limited to Bitcoin.

🔎 Exploratory Data Analysis (EDA)

EDA was performed to understand market behavior and volatility patterns.

Key Insights:

Cryptocurrency prices are highly unstable and noisy

Daily returns show heavy-tailed distributions

Volatility exhibits clustering behavior

High trading volume and liquidity often coincide with high volatility

EDA results justified focusing on volatility prediction instead of price prediction.

⚙️ Feature Engineering

The following features were engineered to capture market dynamics:

Daily Returns – Percentage change in closing prices

Rolling Volatility (Target Variable) – Standard deviation of returns over a rolling window

Liquidity Ratio – Volume / Market Capitalization

Moving Averages – Trend smoothing indicators

Price Range Features – High–Low and Open–Close differences

🤖 Model Development
Algorithm Used

Random Forest Regressor

Why Random Forest?

Handles non-linear relationships well

Robust to noise and outliers

Suitable for complex financial data

The data was split using a time-based 70–30 train-test split to avoid data leakage.

📈 Model Evaluation

The model was evaluated using:

MAE (Mean Absolute Error)

RMSE (Root Mean Squared Error)

R² Score

Observations:

The model captures overall volatility trends

Performs better during stable market periods

Extreme volatility spikes remain difficult to predict

🔧 Model Optimization

Hyperparameter tuning was performed using GridSearchCV to improve performance.

Tuned Parameters:

Number of trees (n_estimators)

Maximum depth (max_depth)

Minimum samples per split and leaf

The optimized model showed improved stability compared to the baseline model.

📊 Results

Actual vs Predicted volatility plots show close trend alignment

Optimized model provides smoother and more reliable predictions

Demonstrates practical applicability for volatility forecasting
