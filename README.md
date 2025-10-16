# 📊 Forecasting Wholesale Meat Prices: Time Series Analysis on USDA Meat Price Trends

## 📘 Project Overview
This project analyzes wholesale meat price trends in the U.S. using USDA data from 2000 to 2024. It applies advanced time series forecasting and machine learning models to predict future prices of various meat subtypes, supporting informed decision-making for stakeholders in food production, trading, and policy. The project explores price volatility, seasonality, and the influence of external economic and environmental factors.

---

## 🗃️ Data Sources
- USDA Livestock and Meat Domestic Data for wholesale monthly meat prices.  
- External datasets including weather (temperature, precipitation), disaster counts, economic indicators (CPI, unemployment rate, GDP), and feed commodity prices (corn, sorghum).

---

## ⚙️ Methodology
- **Data Preprocessing:**  
  Cleaning missing and zero values, feature engineering (time and external factors), integration of multiple datasets by month, and normalization using Min-Max scaling.

- **Exploratory Data Analysis:**  
  Descriptive statistics, price distribution histograms, seasonal and trend decomposition showing volatile market events like the COVID-19 pandemic impact.

- **Modeling Approaches:**  
  - SARIMA for capturing seasonal and trend components in stationary data.  
  - Random Forest Regression for robust nonlinear relationships via an ensemble of decision trees.  
  - Gradient Boosting Regression for sequential improvement of prediction accuracy.  
  - Support Vector Regression (SVR) targeting nonlinear regression with margin optimization.  
  - Long Short-Term Memory (LSTM) neural network to model long-term dependencies and complex sequences.

---

## 🧪 Model Training and Evaluation
- Stationarity tests applied to prepare time series data for SARIMA.  
- Lagged price features and external variables included to enhance learning.  
- Hyperparameter tuning conducted for all models to optimize predictive performance.  
- Evaluation metrics:  
  - R2 Score (Coefficient of Determination) to assess variance explained.  
  - RMSE (Root Mean Squared Error) to measure average prediction error magnitudes.

---

## 📈 Key Results
- The LSTM model with integrated external features demonstrated the best forecasting accuracy overall, particularly for boxed beef cutout subtype, achieving an R2 score of 0.8962 and RMSE of 0.01571.  
- SVR without external features performed well for imported boneless beef.  
- Gradient Boosting showed robustness for loins and drumsticks.  
- External features such as CPI, feed prices, and weather conditions contributed positively but were model and subtype dependent.  
- Price trends reflected significant impact from major events like the COVID-19 pandemic causing price volatility.

---

## 💡 Practical Implications
- Reliable price forecasts help in risk management, pricing strategies, and supply chain stability for agriculture and food industries.  
- Insights assist policymakers and market participants in understanding price drivers and planning for future market conditions.

---

## 🚀 Future Work
- Incorporate additional macroeconomic and consumer behavior data.  
- Develop hybrid models combining strengths of different forecasting methods.  
- Extend forecasting to other agricultural commodities for broader applicability.
licability.
