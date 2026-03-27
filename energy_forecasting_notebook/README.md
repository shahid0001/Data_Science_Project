# 🔋 Energy Consumption Time Series Forecasting

## 📌 Objective
The goal of this project is to forecast short-term household energy consumption using historical time-based data. By leveraging time series models, we aim to accurately predict future electricity usage patterns.

---

## 📊 Dataset
- **Name:** Individual Household Electric Power Consumption Dataset  
- **Source:** UCI Machine Learning Repository  
- **Link:** https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption  

---

## ⚙️ Project Workflow

### 1. Data Preprocessing
- Parsed date and time into a single datetime column  
- Converted power consumption values to numeric format  
- Handled missing values appropriately  

### 2. Time Series Resampling
- Resampled data into **hourly intervals** to improve analysis and modeling  

### 3. Feature Engineering
Extracted key time-based features:
- Hour of the day  
- Day of the week  
- Weekend indicator  

### 4. Models Implemented
- ARIMA (AutoRegressive Integrated Moving Average)  
- Prophet  
- XGBoost  

### 5. Evaluation Metrics
- **MAE (Mean Absolute Error)**  
- **RMSE (Root Mean Squared Error)**  

---

## 📈 Results

| Model     | MAE     | RMSE    |
|----------|--------|--------|
| ARIMA    | 0.6359 | 0.7904 |
| Prophet  | 0.9897 | 1.1761 |
| XGBoost  | 0.7850 | 0.9887 |

✅ **Best Model: ARIMA** (Lowest MAE & RMSE)

---

## 📊 Visualization
- Plotted **Actual vs Forecasted Energy Consumption**  
- Compared predictions across all models for performance analysis  

---

## 🚀 Key Learnings
- Understanding time series forecasting techniques  
- Importance of feature engineering in temporal data  
- Comparing models using evaluation metrics  
- Recognizing patterns in time-based datasets  

---

## ⚠️ Requirements

Install required dependencies using:

```bash
pip install pandas numpy matplotlib scikit-learn statsmodels prophet xgboost
```

---

## 📌 Future Improvements
- Hyperparameter tuning for better model performance  
- Incorporating deep learning models (LSTM, GRU)  
- Using external factors like weather data for improved accuracy  

---

## 👨‍💻 Author
Your Name
