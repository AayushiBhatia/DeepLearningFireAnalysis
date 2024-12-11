# DeepLearningFireAnalysis
# Fire Incident Forecasting with Deep Learning  

This project evaluates the predictive effectiveness of three deep learning models—**LSTM**, **GRU**, and **Transformer**—for forecasting fire incidents in Thailand and Malaysia. By analyzing fire data from January 2012 to June 2024, the project aims to identify the most accurate model for trend prediction and fire management decision-making.

---

## Table of Contents  
- Dataset
- Models Evaluated  
- Metrics Used
- Key Results 
- Conclusion 
- Limitations 

---

## Dataset  
- **Regions**: Thailand and Malaysia  
- **Period**: January 2012 to June 2024 (150 monthly data points)  
- **Focus**: Monthly fire incident counts  

---

## Models Evaluated  
1. **Long Short-Term Memory (LSTM)**  
2. **Gated Recurrent Unit (GRU)**  
3. **Transformer**  

---

## Metrics Used  
The performance of each model was evaluated using:  
- **Mean Squared Error (MSE)**  
- **Root Mean Squared Error (RMSE)**  
- **Mean Absolute Error (MAE)**  
- **R² (Coefficient of Determination)**  

---

## Key Results  

### Thailand  
| Model       | MSE           | RMSE       | MAE       | R²       |  
|-------------|---------------|------------|-----------|----------|  
| LSTM        | 139,623,899.80 | 11,816.26  | 8,183.67  | 0.4700   |  
| GRU         | 67,029,380     | 8,187      | 6,409     | 0.713    |  
| Transformer | 2,752,006      | 1,658.92   | 1,334.25  | 0.9920   |  

### Malaysia  
| Model       | MSE       | RMSE   | MAE    | R²     |  
|-------------|-----------|--------|--------|--------|  
| LSTM        | 173,273.40 | 416.26 | 320.15 | 0.2567 |  
| GRU         | 630,695    | 794    | 631    | 0.361  |  
| Transformer | 21,045.21  | 145.07 | 142.16 | 0.9191 |  

---

## Conclusion  
The **Transformer model** demonstrated the best performance across all metrics for both Thailand and Malaysia:  
- **Thailand**: Achieved an R² score of **0.9920**, indicating it explained most of the variance in the data.  
- **Malaysia**: Achieved an R² score of **0.9191**, showing strong predictive capabilities.  

In comparison:  
- The **GRU model** performed moderately well, particularly in Thailand (R² = 0.713), but struggled with accuracy in Malaysia.  
- The **LSTM model** underperformed, with low R² scores and high error metrics in both regions.  

The **Transformer model** is recommended for time series forecasting in this context due to its superior accuracy and ability to capture trends effectively.  

---

## Limitations  
- **Extreme Value Errors**: All models struggle with predicting extreme values or sharp fluctuations.  
- **Outliers Sensitivity**: Predictions are influenced heavily by outliers in the dataset.  
- **Seasonality Misses**: Models occasionally fail to capture seasonal patterns accurately.  
- **Long-term Dependencies**: GRU and LSTM models showed difficulty in handling long-term trends and dependencies.  

---
