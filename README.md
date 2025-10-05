# Stock Price Prediction for Tesla stock data

This project uses historical stock data for Tesla to perform a time-series analysis and develop a predictive model to forecast future stock prices using the Prophet library.

## 📈 Project Goal

The goal of this project is to analyze historical Tesla stock data to identify long-term trends and seasonality. Based on this analysis, a time-series model is built to forecast the closing stock price for the next 365 days.

---

## 🛠️ Technologies Used

* **Python:** The core programming language used.
* **Pandas:** For data manipulation and analysis.
* **Matplotlib:** For creating static visualizations.
* **Prophet:** The forecasting library used to build the predictive model.
* **Statsmodels:** Used for time-series decomposition analysis.
* **Jupyter Notebook:** As the development environment.

---

## 📊 Analysis Workflow

The project follows a sequential workflow to analyze the data and build the forecast.

### 1. Data Exploration and Analysis
The `Tesla.csv` dataset was loaded and checked for data quality. Initial exploratory analysis was performed by plotting the closing price and trading volume over time to visualize the historical performance.

### 2. Time-Series Decomposition
To better understand the underlying patterns, a seasonal decomposition was performed on the closing price. This separated the data into three components:
* **Trend:** The long-term direction of the stock price.
* **Seasonality:** Recurring patterns within a specific time frame (e.g., monthly).
* **Residuals:** The random noise left over after accounting for trend and seasonality.

### 3. Forecasting with Prophet
The Prophet library was used to build the forecasting model. The model was fit on the *entire* historical dataset and then used to generate a forecast for the next 365 days.

---

## 🎯 Key Findings

Based on the analysis and model output from the original notebook:

* **Strong Upward Trend:** The analysis consistently shows a strong, long-term upward trend in Tesla's stock price over the years.
* **Yearly and Weekly Seasonality:** The Prophet model identified clear yearly and weekly patterns. The yearly seasonality suggests that the stock price tends to be higher in the first half of the year, while the weekly seasonality shows minor fluctuations during the week.
* **Forecasted Growth:** The model's forecast predicts a continuation of the upward trend for the next year, following the established historical pattern.

---

## 🚀 How to Use

1.  Clone this repository.
2.  Install the required libraries:
    -pandas
    -matplotlib
    -prophet
    -statsmodels
    -numpy
4.  Run the file `Stock_Price_Prediction.ipynb` to see the full analysis.
