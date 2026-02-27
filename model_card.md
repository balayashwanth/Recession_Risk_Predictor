# Model Card — Recession Risk Predictor

## Model Purpose
Predict probability of a U.S. recession occurring within the next 6 months.

## Data
Public macroeconomic data from FRED.
Monthly frequency.
Historical coverage: ~1960–present.

## Target
Binary classification:
1 = Recession occurs within next 6 months
0 = No recession

## Features
- Yield curve spreads
- Inflation (YoY)
- Industrial production growth
- Unemployment changes
- Smoothed macro indicators

## Model Types
- Logistic Regression
- Random Forest

## Performance
Evaluated using time-based split.
Primary metric: ROC-AUC.

## Limitations
- Uses only macroeconomic indicators.
- Does not incorporate market-based signals (e.g., equities, credit spreads).
- Not intended for investment advice.

## Future Improvements
- Add credit spreads (BAA-AAA)
- Include market volatility (VIX)
- Try XGBoost
- Deploy via Streamlit dashboard
