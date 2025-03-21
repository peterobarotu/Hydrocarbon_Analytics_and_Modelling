Here's your **updated README.md**, incorporating **regression analysis on hydrocarbon (HC) production and associated gas (AG)** while comparing both since **AG is a byproduct of crude extraction**. Also, I have **removed the example code and updated the license to Apache**.  

---

# **Hydrocarbon Analytics and Modeling**  

## **Overview**  
This project provides a **comprehensive analysis and forecasting model** for **Nigeria's crude oil and natural gas production**, integrating **exploratory data analysis (EDA), regression modeling, and time series forecasting**.  

We examined **historical production trends, OPEC quotas, price fluctuations, offshore vs. onshore production, and different contract types (JV, PSC, SR)**. Additionally, we analyzed the relationship between **hydrocarbon (HC) production and associated gas (AG), given that AG is a byproduct of crude oil extraction**. The analysis highlights **economic opportunities and constraints**, identifying key policy implications.  

---

## **Key Findings**  

1. **Production vs. OPEC Quota Compliance**  
   - Nigeria has consistently **underperformed relative to its OPEC quota**, revealing operational inefficiencies.  

2. **Revenue Loss in 2022**  
   - Despite a surge in global oil prices, **production remained low**, leading to **missed economic gains**.  

3. **Yearly, Monthly & Year-over-Year (YoY) Analysis**  
   - Conducted **detailed trend analysis** of oil & gas production at **monthly and yearly intervals**.  
   - Identified **seasonal variations** and **production declines** over time.  

4. **Offshore vs. Onshore Production Analysis**  
   - Compared **offshore vs. onshore crude oil & gas production**.  
   - Analyzed efficiency and trends between both production environments.  

5. **Contract Type Analysis (JV, PSC, SR)**  
   - Assessed production trends under **Joint Ventures (JV), Production Sharing Contracts (PSC), and Sole Risk (SR)**.  
   - Identified differences in performance across contract types.  

6. **Regression Analysis of Hydrocarbon (HC) Production vs. Associated Gas (AG)**  
   - **Performed regression analysis to quantify the relationship between crude oil (HC) and associated gas (AG) production**.  
   - Compared HC and AG production trends to assess **efficiency in gas utilization** and **flaring reduction strategies**.  

7. **Forecasting with Hybrid Models**  
   - Developed a **Hybrid ARIMA-XGBoost model**, leveraging **multiple lag-based predictions** to refine forecasts.  
   - Aggregated **multi-lag XGBoost outputs** to improve predictive accuracy.  

---

## **Work Completed**  

### **1️⃣ Oil & Gas Production Analysis**  
- **Performed yearly, monthly, and YoY trend analysis** for both **crude oil and gas production**.  
- Compared **actual production vs. OPEC quotas** over time.  
- **Analyzed offshore vs. onshore production performance**.  
- **Evaluated contract-based production trends** (JV, PSC, SR).  
- **Performed regression analysis of HC vs. AG production**.  
- Visualized data using **Matplotlib & Seaborn** for **dual-axis plots and trend graphs**.  

### **2️⃣ Regression Analysis: HC vs. AG Production**  
- Investigated the relationship between **crude oil production (HC) and associated gas (AG)**.  
- **Built a regression model** to quantify the correlation and trends.  
- **Examined how production fluctuations impact gas utilization**.  

### **3️⃣ Time Series Forecasting (ARIMA-XGBoost Hybrid)**  
- Implemented an **ARIMA model** to capture long-term production trends.  
- Designed an **XGBoost-based residual correction** to enhance forecasts.  
- Developed a **multi-lag XGBoost ensemble approach**, combining forecasts from `3, 6, and 12` lag periods.  
- Generated hybrid forecasts for:  
  ✅ **Crude Oil (MMbbls/day, bbls)**  
  ✅ **Natural Gas (BCF/day, MMSCF)**  

---

## **Installation & Setup**  

Clone the repository:  

```bash
git clone https://github.com/your-username/Hydrocarbon_Analytics_and_Modelling.git
cd Hydrocarbon_Analytics_and_Modelling
```

## **Contributing**  
Contributions are welcome! Feel free to **open an issue or submit a pull request**.  

---

## **License**  
This project is licensed under the **Apache License 2.0**.  

---

This version includes **regression analysis on HC vs. AG production**, removes example code, and updates the license. Let me know if anything else needs to be refined! 🚀
