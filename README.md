# 🛢️ Black Gold Horizon: Projecting America's Oil Future

This repository is dedicated to the project **"Black Gold Horizon: Projecting America's Oil Future"**, a comprehensive analysis and forecast of crude oil production in the United States, both at the national level and for specific regions. The project utilizes advanced time-series analysis and forecasting models in **R** to provide predictions of future production levels. The goal of the project is to aid policymakers, industry professionals, and researchers in making data-driven decisions in the energy sector.

---

## 🌟 Project Overview

**Black Gold Horizon** focuses on analyzing the historical production of crude oil in the United States and projecting future production levels for individual states and regions categorized according to the **Petroleum Administration for Defense Districts (PADD)**. By identifying trends, seasonal patterns, and other characteristics within the data, the project aims to construct robust and accurate forecasts for the next 5 to 10 years.

The insights from this project are crucial for understanding the future of America’s oil production, helping inform decisions regarding energy policy, investments, and sustainability efforts.

---

## 📊 Key Objectives

- **Trend Analysis**: Explore historical production data to identify long-term trends in crude oil production.
- **Seasonality Detection**: Investigate seasonal patterns in production that could affect supply and demand cycles.
- **Forecasting**: Build reliable models to predict future crude oil production for the entire US and specific regions (PADD).
- **Regional Focus**: Analyze production trends for each of the **PADD regions**:
  - PADD 1: East Coast
  - PADD 2: Midwest
  - PADD 3: Gulf Coast
  - PADD 4: Rocky Mountain
  - PADD 5: West Coast

---

## 📂 Data Collection

The primary dataset for this project includes historical monthly field production of crude oil in the US, ranging from **January 1981 to November 2016**. The data includes:
- **Total US field production of crude oil**.
- **Field production of crude oil by PADD regions**.
- **Field production of crude oil by selected states within each PADD region**.

### Data Sources:
- The data was sourced from the **U.S. Energy Information Administration (EIA)**, which provides official statistics on energy.
- Recent and updated data will be retrieved from the EIA's API and monthly reports.

**Dataset Link**: [US EIA Crude Oil Production Data](https://www.eia.gov/dnav/pet/hist/LeafHandler.ashx?n=PET&s=MCRFPUS1&f=M)

---

## 🧠 Data Analysis & Forecasting

The project employs the following techniques for data analysis and forecasting in **R**:

### 1. **Data Cleaning & Preprocessing**
   - Handle missing data, outliers, and anomalies in the historical data.
   - Normalize the data to facilitate smooth time-series analysis using **dplyr** and **tidyr** packages.

### 2. **Exploratory Data Analysis (EDA)**
   - Visualize trends, seasonality, and cyclic behaviors in crude oil production data using **ggplot2**.
   - Analyze the impact of external factors (e.g., market conditions, technological changes) on production levels.

### 3. **Time-Series Forecasting Models**
   - **Seasonal Decomposition**: Break down production data into trend, seasonal, and residual components using **stats::decompose** and **STL** methods.
   - **ARIMA (Auto-Regressive Integrated Moving Average)**: Model and forecast time-series data to capture production trends and short-term fluctuations using the **forecast** package.
   - **SARIMA (Seasonal ARIMA)**: Incorporate seasonality in the ARIMA model to better handle repetitive patterns in the data.

### 4. **Performance Evaluation**
   - **Root Mean Square Error (RMSE)** and **Mean Absolute Error (MAE)** will be used to evaluate model performance and ensure high accuracy in the forecasts.

---

## 🛠️ Tools & Technologies

| Tool/Technology  | Description  |
| ---------------- | ------------ |
| ![R](https://img.shields.io/badge/-R-276DC3?logo=r&logoColor=white) | The main programming language for data analysis and modeling. |
| **dplyr** | For data manipulation, cleaning, and transformation. |
| **tidyr** | For reshaping and cleaning the dataset. |
| **ggplot2** | For visualizing trends and patterns in crude oil production data. |
| **forecast** | Used for implementing time series models like ARIMA and SARIMA. |
| **TTR** | For technical analysis and trend detection in time-series data. |
| **zoo** | For working with regular and irregular time-series data. |
| **xts** | For time-series data management and forecasting. |

---

## 🔮 Deliverables

The project will deliver forecasts for crude oil production for the major US oil-producing states and regions. Key deliverables include:
- **10-15 individual forecasts** covering major oil-producing states and PADD regions.
- **Forecast horizon** of 5 to 10 years into the future, with regular updates based on new data.
- **Visualizations** of trends and seasonal patterns, highlighting key insights for policymakers and industry stakeholders.

---

## 🔧 Forecasting Models

The following models were explored and implemented to provide accurate predictions:
1. **Seasonal Decomposition**: Decomposing the data into seasonal, trend, and residual components to better understand cyclical patterns in production using the `decompose()` and `stl()` functions.
2. **ARIMA Model**: A statistical model used for analyzing and forecasting time-series data that shows auto-correlation using the **forecast** package.
3. **SARIMA Model**: Extends ARIMA by supporting seasonal differencing, making it suitable for data with seasonal variations (e.g., oil production that varies seasonally).

---

## 📈 Performance Metrics

The following metrics will be used to evaluate the performance and accuracy of the forecasting models:
- **Root Mean Square Error (RMSE)**: Measures the average magnitude of the error in the forecasts.
- **Mean Absolute Error (MAE)**: Measures the absolute differences between predicted and actual values, providing a clearer view of the model’s performance.
- **R-squared**: To assess how well the model explains the variability in the data.

---

## 🎯 Goals and Conclusion

This project aims to provide actionable insights for stakeholders in the energy sector, including:
- **Policymakers**: Supporting energy policy decisions based on future oil production trends.
- **Industry Professionals**: Helping businesses optimize production and investment strategies.
- **Researchers**: Offering a comprehensive dataset and model framework for further study.

By accurately forecasting future crude oil production, **Black Gold Horizon** contributes to a better understanding of the evolving energy landscape in the United States and offers valuable guidance for planning and decision-making in the oil industry.


## 🔗 Related Resources

- **EIA U.S. Crude Oil Data**: [U.S. Energy Information Administration](https://www.eia.gov/dnav/pet/hist/LeafHandler.ashx?n=PET&s=MCRFPUS1&f=M)
- **Time Series Forecasting in R**: [Forecasting with R](https://otexts.com/fpp3/)

