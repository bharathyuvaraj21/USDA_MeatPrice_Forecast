# 📊 Forecasting Wholesale Meat Prices: Time Series Analysis on USDA Meat Price Trends

## 📘 Project Overview
This project analyzes wholesale meat price trends in the U.S. from 2000 to 2024 using USDA data. It applies advanced time series and machine learning forecasting models to predict future prices of various meat subtypes, aiding stakeholders in food production, trading, and policy decision-making. The study also explores price volatility, seasonality, and external economic and environmental influences.

---

## 🗃️ Data Sources
- USDA Livestock and Meat Domestic Data for monthly wholesale meat prices.  
- External data on weather (temperature, precipitation), disaster counts, economic indicators (CPI, unemployment, GDP), and feed commodity prices (corn, sorghum).

---

## ⚙️ Methodology

### 1. Data Collection and Integration
- Historical wholesale meat price data obtained from USDA covering multiple meat subtypes.  
- Collected external feature datasets: weather records, economic indicators, and disaster incidents.  
- Unified all datasets by monthly time alignment using "Year-Month" as a key.

### 2. Data Preprocessing
- Cleaned missing values and addressed zeros due to discontinued reporting periods.  
- Created new features including lagged price variables and combined economic/environmental factors.  
- Applied Min-Max scaling for uniform feature ranges, essential for model convergence.

### 3. Exploratory Data Analysis (EDA)
- Generated descriptive statistics to summarize price distributions and volatility.  
- Visualized seasonal trends and historical price fluctuations across meat subtypes.  
- Conducted correlation analyses between meat prices and external factors to identify influential variables.

### 4. Model Selection and Development
- Chose five models covering classical statistical and machine learning approaches:  
   - SARIMA to model seasonality and trends in stationary price series.  
   - Random Forest Regression to capture nonlinear relationships and interactions.  
   - Gradient Boosting Regression for sequential error correction and fine-tuning.  
   - Support Vector Regression (SVR) for regression with regularization and robustness.  
   - Long Short-Term Memory (LSTM) neural networks for modeling complex temporal dependencies.  
- Implemented hyperparameter tuning using grid search for optimized performance.

### 5. Model Training and Evaluation
- Stationarity tests applied to prepare time series data for SARIMA.  
- Lagged price features and external variables included to enhance learning.  
- Hyperparameter tuning conducted for all models to optimize predictive performance.  
- Split data into training and testing sets respecting time order.   
- Trained models with and without external features for comparative analysis.  
- Evaluated performances using R2 Score (variance explanation) and RMSE (average error magnitude).

### 6. Result Interpretation and Visualization
- Compared predictions versus actual prices across models and meat subtypes.  
- Highlighted LSTM with external features as best overall performer (R2 ~0.8962, RMSE ~0.01571 for boxed beef).  
- Noted SVR effectiveness without external features on imported boneless beef.  
- Acknowledged Gradient Boosting robustness in loins and drumsticks subtypes.  
- Identified key external features positively impacting forecast accuracy.

---

## 📈 Key Findings
- Time series deep learning (LSTM) outperforms classical SARIMA and ensemble models in capturing complex price dynamics.  
- Inclusion of external economic, weather, and commodity price data significantly enhances forecasts for many meat subtypes.  
- Price dynamics reflect major events like the COVID-19 pandemic, causing spikes and volatility in meat prices.

---

## 💡 Practical Implications
- Improved forecasting reliability supports risk mitigation, pricing strategies, and supply chain management.  
- Enables producers, retailers, and policymakers to anticipate market trends and adapt decisions proactively.

---

## 🚀 Future Work
- Explore integration of more diverse macroeconomic and consumer behavior datasets.  
- Develop hybrid ensemble models combining strengths of multiple forecasting techniques.  
- Extend forecasting frameworks to additional agricultural commodity markets for broader impact.

---


