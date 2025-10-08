# 📈 Sales Forecasting using ARIMA & SARIMA

📖 **Overview**  
This project applies **Time Series Forecasting** techniques using **ARIMA** and **SARIMA** models to predict future sales based on past monthly data.  
The goal is to understand patterns and seasonality in the dataset and forecast upcoming sales values.

🧠 **Skills Demonstrated**  
- Time series data preprocessing and indexing with Pandas  
- Building and training **ARIMA** and **SARIMA** models  
- Forecasting and comparing predicted vs actual sales  
- Visualization of model performance using Matplotlib  

🧰 **Tools Used**  
Python, Pandas, Statsmodels, Matplotlib  

⚙️ **Model Details**  
- **ARIMA Model:** (p=2, d=1, q=1)  
- **SARIMA Model:** (p=2, d=1, q=1)(P=2, D=1, Q=1, s=12)  

🚀 **Results**  
- **ARIMA Forecast (Next 6 Months):**  
  Showed stable continuation of trend with slight fluctuations.  
- **SARIMA Forecast (Next 6 Months):**  
  Captured seasonal variations more effectively compared to ARIMA.  

📊 **Visualization**  
The plot below compares **Actual Sales**, **ARIMA Forecast**, and **SARIMA Forecast**, illustrating how SARIMA accounts for seasonal trends.  

📂 **Notebook**  
See [`ARIMA_&_SARIMA.ipynb`](./ARIMA_&_SARIMA.ipynb)
