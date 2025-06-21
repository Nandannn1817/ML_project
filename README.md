# 📈 Yes Bank Monthly Stock Price Prediction

This project analyzes the historical stock price data of Yes Bank with the goal of understanding trends, exploring key financial indicators, and building regression models for monthly closing price prediction.

---

## 📌 Problem Statement

The objective of this project is to perform **time-series analysis and prediction** on the monthly stock price data of Yes Bank. We aim to:
- Analyze past trends using EDA and data wrangling techniques
- Visualize patterns in stock movements
- Build regression models to predict monthly closing prices using features like Open, High, Low, etc.

---

## 📂 Dataset Overview

The dataset consists of Yes Bank stock data with the following columns:
- `Date`: The month-end date
- `Open`: Opening stock price
- `High`: Highest stock price during the month
- `Low`: Lowest stock price during the month
- `Close`: Closing stock price
- `Year`, `Month`, `Month_Name`: Extracted date components
- `High_Low_Diff`, `Open_Close_Diff`: Engineered features for volatility and price change

---

## ⚙️ Tech Stack

- **Language**: Python
- **IDE**: Google Colab
- **Libraries**:
  - `pandas`, `numpy` for data handling
  - `matplotlib`, `seaborn` for visualization
  - `sklearn` for modeling and evaluation

---

## 🔎 Steps Followed

1. **Data Loading & Preprocessing**:
   - Removed duplicates and handled nulls
   - Converted data types and stripped column names
   - Created new derived features for better modeling

2. **Exploratory Data Analysis (EDA)**:
   - Statistical summary (`.describe()`, `.info()`)
   - Unique value check
   - Missing value visualization
   - Time-series plotting of Close price
   - Correlation heatmap between variables

3. **Feature Engineering**:
   - Created `High_Low_Diff` and `Open_Close_Diff` to capture volatility
   - Extracted `Month`, `Year` and `Month_Name` for temporal analysis

4. **Visualization**:
   - Line chart: Monthly Closing Prices Over Time
   - Correlation heatmap (Open, High, Low, Close, etc.)
   - Additional charts can be added for deeper analysis

5. **Model Building** (To Be Extended):
   - Linear Regression and other regressors (Random Forest, XGBoost, etc.)
   - Model evaluation using R² Score, RMSE, MAE

---

## 📊 Sample Insights

- Significant variations in monthly closing prices were observed, indicating volatility.
- Strong correlation between `Open`, `High`, `Low`, and `Close`, justifying multivariate regression.
- Months like March and October showed sudden spikes or drops due to market events.

---

## 🚀 Future Scope

- Implement advanced time-series models (ARIMA, LSTM)
- Include external indicators (volume, news sentiment)
- Deploy as a web app/dashboard using Streamlit or Flask

---

## 📁 Folder Structure
├── data_YesBank_Stock.csv # Input dataset

├── Sample_ML_Submission.ipynb # Complete Jupyter Notebook (Google Colab)

├── README.md # Project overview

