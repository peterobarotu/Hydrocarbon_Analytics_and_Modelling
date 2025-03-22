## **Overview**  
This repository contains a comprehensive analysis and forecasting framework for Nigeria’s crude oil and gas production. It includes data analytics, statistical modeling, and machine learning techniques to evaluate production trends, OPEC quota compliance, market dynamics, and future projections.  

The work leverages historical data from NUPRC, NMDPRA, and OPEC reports to analyze key industry patterns, identify inefficiencies, and provide actionable insights. The forecasting models use both traditional time series techniques and machine learning to improve prediction accuracy.  

## **Key Objectives**  
- **Production Analysis:** Monthly, yearly, and year-on-year (YoY) analysis of Nigeria’s hydrocarbon production.  
- **Market & Policy Evaluation:** Assessing Nigeria’s compliance with OPEC quotas and revenue implications of production trends.  
- **Machine Learning Forecasting:** Implementing ARIMA, XGBoost, and hybrid models to predict future production trends.  
- **Structural Insights:** Offshore vs. onshore production comparison, contract types (JV, PSC, SR), and regression analysis between hydrocarbon (HC) and associated gas (AG).  

---

## **1. Production Analysis**  
We analyzed Nigeria’s crude oil and natural gas production using monthly and yearly datasets from the Nigerian Upstream Petroleum Regulatory Commission (NUPRC) and the Nigerian Midstream and Downstream Petroleum Regulatory Authority (NMDPRA).  

- **Comparison of actual production vs. OPEC quota.**  
- **Evaluation of key terminals influencing overall output.**  
- **Yearly, monthly, and YoY comparisons to detect trends and anomalies.**  
- **Analysis of offshore vs. onshore production patterns and contract types (JV, PSC, SR).**  

### **Findings:**  
- Nigeria has consistently produced below its allocated OPEC quota.  
- Significant production volatility, especially in 2022, due to operational challenges.  
- Key terminals like Bonny and Forcados have a major impact on the overall daily average production.  

---

## **2. Market & Economic Insights**  
To assess Nigeria’s ability to capitalize on global oil price movements, we examined how production trends align with oil price fluctuations and OPEC policies.  

- **2022 Oil Price Surge and Revenue Loss:** Despite high oil prices, Nigeria's low production levels led to missed revenue opportunities.  
- **Impact of Force Majeure Events:** Examined disruptions from vandalism, repairs, and regulatory shutdowns on production stability.  
- **NMDPRA Gas Supply Report Analysis:** Identified imbalances in Nigeria’s gas supply, comparing domestic sales, export volumes, and gas flaring levels.  

### **Findings:**  
- Production remained low during high oil price periods, leading to revenue losses.  
- Domestic gas supply struggled to meet demand despite high export volumes.  
- Gas flaring remains a persistent issue, affecting environmental and economic factors.  

---

## **3. Forecasting & Modeling**  
We developed forecasting models to predict future hydrocarbon production using time series and machine learning approaches.  

### **Approaches Used:**  
1. **ARIMA Model**  
   - Performed stationarity tests using ADF to determine differencing needs.  
   - Used Auto-ARIMA for optimal parameter selection.  
   - Forecasted production trends assuming a random-walk behavior.  

2. **XGBoost Model**  
   - Created lagged features to train an XGBoost regressor.  
   - Explored different lag values (3, 6, 12, 18, 24 months) to identify optimal forecasting windows.  
   - Evaluated performance using RMSE and forecast accuracy.  

3. **Hybrid ARIMA-XGBoost Model**  
   - Combined ARIMA’s linear forecasting with XGBoost’s ability to model residual errors.  
   - Improved accuracy by reducing forecast bias seen in individual models.  
   - Developed a multi-lag framework that aggregates forecasts from different time lags.  

### **Findings:**  
- The **ARIMA model alone** assumes a constant production level due to its differencing order (0,1,0).  
- The **XGBoost model alone** effectively captures patterns within the training set but struggles slightly with the test data, especially at the tail end. While it follows short-term fluctuations well, its performance declines when applied to unseen data, indicating potential overfitting or difficulty adapting to new trends.  
- The **hybrid model outperforms both ARIMA and XGBoost**, providing more balanced and realistic forecasts. It effectively captures fluctuations in the training set and maintains consistency in the test set. It successfully adapts to unseen data without significant deviations, ensuring stability in predictions. While the model corrects ARIMA’s residuals effectively, its ability to track long-term trends can still be influenced by structural breaks in the data as seen in the Non-Associated gas forecasting.
---

## **4. Technical Implementation**  
- **Data Preprocessing:** Cleaning, transforming, and structuring datasets for analysis.  
- **Visualization & Trend Analysis:** Using Pandas, Matplotlib, and Seaborn for insights.  
- **Model Training & Evaluation:** Implementing ARIMA and XGBoost with hyperparameter tuning.  
- **Multi-Lag Forecasting:** A weighted approach to balance short-term and long-term lag contributions.  

---

## **5. Next Steps**  
- **Evaluate the model with additional real-world data** as new production reports are released.  
- **Retrain and refine the models** using an updated dataset covering 6-12 months.  
- **Perform long-term forecasting** for the next year to assess industry outlook.  

---

## **Usage Instructions**  
To get started with this project, follow these steps:  

1. **Clone the repository**  
   ```bash
   git clone https://github.com/peterobarotu/Hydrocarbon_Analytics_and_Modelling.git
   ```  
2. **Navigate to the project directory**  
   ```bash
   cd Hydrocarbon_Analytics_and_Modelling

---

## **License**  
This project is licensed under the Apache License 2.0.  

---
