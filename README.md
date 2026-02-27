# 📉 Recession Risk Prediction Using Yield Curve & Macro Indicators

## 📌 Project Overview
This project predicts the probability of a U.S. recession occurring within the next 6 months using macroeconomic indicators and yield curve spreads.

The model uses publicly available data from the Federal Reserve Economic Data (FRED) database.

## 💡 Motivation
The yield curve (especially the 10Y–2Y and 10Y–3M spread) has historically been a strong predictor of recessions. 
This project builds a simple, interpretable machine learning model to estimate forward-looking recession risk.

## 📊 Data Sources (FRED)
- DGS10 – 10-Year Treasury Yield
- DGS2 – 2-Year Treasury Yield
- DGS3MO – 3-Month Treasury Yield
- UNRATE – Unemployment Rate
- CPIAUCSL – Consumer Price Index
- INDPRO – Industrial Production
- USREC – NBER Recession Indicator (binary target)

Data pulled from:
https://fred.stlouisfed.org

## 🏗 Feature Engineering
- Yield spreads (10Y–2Y, 10Y–3M)
- 3-month moving averages
- YoY inflation %
- YoY industrial production %
- 3-month unemployment change
- Forward-looking label: recession within next 6 months

## 🤖 Models Used
- Logistic Regression (interpretable baseline)
- Random Forest (non-linear classifier)

## 📈 Evaluation
- Time-based train/test split
- ROC-AUC metric
- Confusion matrix
- Probability risk curve visualization

## 🚀 How to Run
1. Open the notebook in Google Colab
2. Run all cells
3. Dataset will be generated automatically
4. Latest recession probability will be displayed

## 📁 Output
- `recession_ml_dataset.csv`
- Probability curve chart
- Current estimated recession risk

## 🧠 Skills Demonstrated
- Time-series feature engineering
- Macroeconomic data modeling
- Forward-label construction
- Financial ML
- Model evaluation (ROC-AUC)
- Reproducible data pipeline

---
