# **Sales Data Analysis and Forecasting**

## **Project Overview**
This project analyzes Walmart sales data (2010–2012) to uncover seasonal trends, the impact of holidays and temperature on sales, and forecast future demand. The goal is to optimize inventory management by minimizing overstock and stockout scenarios during high-impact periods.

## **Key Objectives**
1. Analyze seasonal sales trends across Winter, Spring, Summer, and Fall.
2. Quantify the impact of high-impact holiday weeks on sales performance.
3. Segment sales based on temperature brackets (Cold, Moderate, Hot) to identify weather-driven trends.
4. Perform time series forecasting to predict weekly sales using ARIMA models.

## **Dataset**
The dataset is sourced from Kaggle: **([Walmart Sales Data](Walmart.xlsx)
)**.  
It includes:
- **Store**: Store number.
- **Date**: Week of sales.
- **Weekly_Sales**: Sales for the given store during the week.
- **Holiday_Flag**: Indicates whether the week is a holiday (1) or not (0).
- **Temperature**: Temperature on the sale day.
- **Fuel_Price**: Fuel price in the region.
- **CPI**: Consumer price index.
- **Unemployment**: Unemployment rate in the region.

---

## **Project Workflow**

### **1. Data Collection and Preparation**
- Imported the dataset into a database and extracted insights using SQL.
- Key SQL queries:
  - Seasonal grouping of sales.
  - Analysis of sales by holiday weeks.
  - Temperature-based segmentation of sales.
  - Rolling averages to smooth sales trends.  

### **2. Exploratory Data Analysis (EDA)**
- Created pivot tables and visualizations in Excel to identify sales trends by store, region, and time period.
- Analyzed top-performing stores and the contribution of holiday weeks to overall sales.

### **3. Time Series Analysis**
- Converted weekly sales data into a time series object using R.
- Decomposed time series into trend, seasonality, and residual components using STL.
- Built ARIMA models to forecast weekly sales for 52 weeks.
- Evaluated model accuracy using:
  - **Mean Absolute Error (MAE)**
  - **Root Mean Square Error (RMSE)**

### **4. Dashboard Creation**
- Designed an interactive Tableau dashboard to visualize:
  - Seasonal sales trends.
  - Holiday vs. non-holiday sales impact.
  - Forecasted sales for inventory planning.
- [View Tableau Dashboard](<https://public.tableau.com/app/profile/ritya.singh7647/viz/WalmartSalesDashboard_17326920509980/Dashboard1>)

---

## **Key Insights**
- Seasonal analysis revealed Summer as the peak season for average sales.
- Sales were highest in cool temperature ranges (<40°F).
- Forecasted weekly sales trends to guide inventory planning.
---

## **Tools and Technologies**
- **SQL**: Data extraction and segmentation.
- **Excel**: Data cleaning and preliminary visualization.
- **R**: Time series analysis and forecasting (ARIMA).
- **Tableau**: Interactive dashboard creation.

---
