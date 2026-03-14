# XLV Volatility & Sentiment Machine Learning Model

## Overview

This project explores whether market uncertainty and public sentiment can help 
predict short-term price movements in the **Health Care Select Sector SPDR ETF (XLV)**.

The core hypothesis is that defensive sectors such as **Healthcare, Utilities, and Consumer Staples** 
tend to attract capital during periods of economic uncertainty. 
By combining financial market indicators with public sentiment data, we attempt 
to build a machine learning model that predicts the **direction of XLV price movements over the next five trading days**.

The model is framed as a **binary classification problem**:

- **1** --> XLV price increases over the next 5 days  
- **0** --> XLV price decreases over the next 5 days  

The goal of the project is not to build a production trading strategy, but to 
demonstrate the **machine learning workflow used in quantitative finance research**, 
including data preparation, feature engineering, model optimization, and evaluation.

---

## Data Sources

This project combines several different types of data:

### Market Data
- **XLV ETF price data**
- Used to compute the target variable (5-day forward return direction)

### Market Volatility
- **CBOE Volatility Index (VIX)**
- Used as a proxy for market uncertainty

### Public Sentiment
- **Google Trends data for the search term "recession"**
- Used as a measure of public concern about economic downturns

---

## Machine Learning Task

The model attempts to predict:

> Whether XLV will move **up or down over the next 5 trading days**

This is implemented as a **binary classification problem**.

The workflow includes:

1. Data preprocessing and cleaning  
2. Feature engineering and selection  
3. Model training and hyperparameter tuning  
4. Overfitting and underfitting detection  
5. Model evaluation and performance comparison  

---

## Project Structure

xlv-volatility-sentiment-ml
│
├── data/
│ └── raw_data_files
│
├── notebooks/
│ └── project_starter.ipynb
│
├── results/
│ └── model_outputs
│
├── README.md
└── requirements.txt


---

## Key Concepts Explored

This project demonstrates several core machine learning techniques commonly used in financial modeling:

- Feature engineering with macro indicators
- Binary classification for price direction prediction
- Hyperparameter tuning
- Model evaluation and validation
- Detection of overfitting and underfitting
- Combining financial data with alternative datasets

---

## Important Disclaimer

This project is for **educational and research purposes only**.

The model presented here is not intended to be used as a real trading strategy. 
Financial markets are complex systems and any real investment strategy would require 
far more rigorous testing, including:

- transaction costs
- slippage
- walk-forward testing
- risk management
- portfolio construction

---

## Possible Extensions

Several improvements could be explored in future iterations:

- Adding additional macroeconomic indicators
- Incorporating news sentiment data
- Testing alternative ML models (XGBoost, Random Forest, Neural Networks)
- Using rolling walk-forward validation
- Building a full trading backtest framework

---

## Author
Wayne Bartlett
Data Science & Machine Learning research project exploring the intersection of 
**financial markets, volatility indicators, and public sentiment signals**.