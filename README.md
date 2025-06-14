**CPI Forecasting Using Machine Learning**

This project focuses on forecasting the Consumer Price Index (CPI) for India using historical data from September 2016 to April 2025. The aim is to build a reliable model that can predict future CPI trends for the next 6 months using machine learning and time series techniques.

*Project Structure*  
├── data/  
│   ├── combined_cpi_data.csv &emsp;&emsp;&emsp; # Cleaned historical CPI dataset  
│   ├── weighted_cpi.csv &emsp;&emsp;&emsp;&emsp;&emsp; # CPI calculated with weights dataset  
│   ├── featured_cpi.csv &emsp;&emsp;&emsp;&emsp;&emsp;&emsp; # Feature-engineered dataset  
│   └── cpi_forecast_6months.csv &emsp;&emsp; # Forecasted CPI output  
├── notebooks/  
│   ├── 01_data_cleaning.ipynb &emsp;&emsp;&emsp;&emsp;&emsp; # Data-cleaning notebook  
│   ├── 02_exploratory_analysis.ipynb &emsp;&emsp; # EDA notebook  
│   ├── 03_feature_engineering.ipynb &emsp;&emsp;# Feature-engineering notebook  
│   ├── 04_model_training.ipynb &emsp;&emsp;&emsp;&emsp; # Model-training notebook  
│   ├── 05_forecasting.ipynb &emsp;&emsp;&emsp;&emsp;&emsp;&emsp; # Forecasting notebook  
│   └── 06_summary_dashboard.ipynb &emsp;&emsp; # Summary notebbok with final results  
├── README.md &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp; # Project overview and instructions  

*Features Engineered*
- CPI_pct_change – Month-over-month percentage change
- CPI_yoy_change – Year-over-year change
- Lag_1, Lag_2, Lag_3 – Lagged CPI values
- CPI_roll_mean_3, CPI_roll_std_3 – 3-month rolling stats
- Month_sin, Month_cos – Seasonal encoding

*Models Used*
- **Random Forest Regressor** for CPI forecasting
- Evaluation Metrics:
  - **RMSE**: 0.30
  - **MAE**: 0.25

*Forecast Output*:  
Forecasted Weighted CPI for the next 6 months (May–Oct 2025) using the trained model, saved in cpi_forecast_6months.csv.

*Key Takeaways:*
- The model can capture seasonality and trend from CPI data well.
- Feature engineering significantly improves model performance.
- Forecasts can assist policymakers and analysts in anticipating inflation changes.

*Future Work*  
- Subgroup-wise CPI forecasting
- Hyperparameter tuning
- Use of advanced models (e.g., XGBoost, LSTM)

**Author**  
Aiswarya Lakshmi P R  
Intern at Ministry of Statistics and Programme Implementation (MoSPI)  
MSc in Survey Research & Data Analytics  
International Institute for Population Sciences (IIPS), Mumbai  
