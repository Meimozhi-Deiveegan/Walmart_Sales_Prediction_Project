# Capstone Project: Walmart Sales Forecasting - Project Report

## 1. Introduction

This report details the exploratory data analysis (EDA) and initial forecasting attempts conducted on the Walmart sales dataset. The primary objective of this project is to understand the factors influencing weekly sales and develop a predictive model to forecast future sales. This report focuses on addressing the initial set of business questions provided.

## 2. Objectives

The project aims to:

* Perform comprehensive EDA to gain insights into the dataset.
* Analyze the impact of various factors (unemployment rate, seasonality, temperature, CPI) on weekly sales.
* Identify top and worst-performing stores.
* Develop a forecasting solution for Walmart sales.

## 3. Methodology

The project followed these steps:

1.  **Data Loading and Initial Inspection:**
    * Imported necessary libraries (Pandas, NumPy, Matplotlib, Seaborn).
    * Loaded the "Walmart.csv" dataset into a Pandas DataFrame.
    * Performed initial data inspection using `info()` and `head()`.
2.  **Data Preprocessing:**
    * Set the 'Date' column as the index.
    * Created a copy of the dataframe for analysis.
3.  **Exploratory Data Analysis (EDA):**
    * Analyzed the correlation between 'Unemployment' and 'Weekly_Sales' for each store.
    * Visualized weekly sales trends over time to identify seasonality.
    * Further analysis of Temperature and CPI relationship to weekly sales.
4.  **Addressing Business Questions:**
    * Analyzed store-wise correlation to determine the impact of unemployment.
    * Identified seasonal trends through time-series plots.
    * Analyzed the effect of Temperature and CPI on weekly sales.
    * Determined the top and worst-performing stores based on historical data.

## 4. Dataset Description

The dataset "Walmart.csv" contains the following columns:

* **Store:** Store number.
* **Date:** Week of sales.
* **Weekly_Sales:** Sales for the given store in that week.
* **Holiday_Flag:** If it is a holiday week.
* **Temperature:** Temperature on the day of the sale.
* **Fuel_Price:** Cost of the fuel in the region.
* **CPI:** Consumer Price Index.
* **Unemployment:** Unemployment Rate.

## 5. Results and Observations

### 5.1. Impact of Unemployment Rate

* The correlation between 'Unemployment' and 'Weekly_Sales' varies significantly across stores.
* Stores 38 and 44 show a strong negative correlation, indicating that increased unemployment leads to decreased sales.
* Store 36 showed a strong positive correlation.
* Most stores showed little to no correlation.

### 5.2. Seasonal Trends

* Time-series plots of 'Weekly_Sales' reveal seasonal trends.
* Sales tend to peak around holiday periods, particularly towards the end of the year.

### 5.3. Impact of Temperature and CPI

* The provided code does not show a clear analysis of the Temperature or CPI relationship to weekly sales. Further code should be added to analyze these relationships.

### 5.4. Top and Worst-Performing Stores

* The code does not contain the logic to identify top and worst-performing stores. This will need to be added.

## 6. Conclusion

The EDA provided valuable insights into the factors influencing Walmart's weekly sales. Unemployment rates appear to have a store-specific impact, with some stores being more sensitive than others. Seasonal trends are evident, with holiday periods driving sales peaks. Further analysis is required to determine the impact of Temperature and CPI.

## 7. Future Work

* Complete the analysis of Temperature and CPI impact on weekly sales.
* Implement logic to identify and rank top and worst-performing stores.
* Develop and evaluate forecasting models for predicting weekly sales.
* Implement time series models.
* Add more detailed visualizations.
* Add more detailed business conclusions.
* Consider holiday effect in the model creation.


# Walmart-Sales-Prediction-Best-ML-Algorithms
# Machine Learning Project - Retail Sales Forecasting - Walmart

## 1. Introduction

This report details a machine learning project aimed at forecasting weekly sales for a retail store with multiple outlets across the country. The project utilizes the "Walmart DataSet.csv" dataset, which contains weekly sales data along with various influencing factors such as unemployment rate, temperature, fuel price, and consumer price index. The primary goal is to provide insights into sales patterns and develop a predictive model for future sales forecasting.

## 2. Objectives

The primary objectives of this project were:

* To perform exploratory data analysis (EDA) to understand the relationships between various factors and weekly sales.
* To identify and handle outliers and missing values in the dataset.
* To develop and evaluate predictive models for forecasting weekly sales for the next 12 weeks.
* To answer specific business questions related to the impact of unemployment rate, seasonality, temperature, and consumer price index on weekly sales.

## 3. Methodology

The project followed a structured approach:

1.  **Data Exploration:**
    * Imported necessary Python libraries (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Statsmodels).
    * Loaded the "Walmart DataSet.csv" dataset into a Pandas DataFrame.
    * Performed initial data inspection, including checking data types and unique values.
    * Converted the Date column to datetime format, and extracted weekday, month and year values.
2.  **Exploratory Data Analysis (EDA):**
    * Analyzed the distribution of the target variable (Weekly_Sales).
    * Visualized the distribution of numerical features and identified outliers.
    * Examined the relationships between features using pair plots.
3.  **Data Preprocessing:**
    * Removed duplicate rows.
    * Checked for and handled missing values (none found).
    * Converted categorical features to numerical using one-hot and dummy encoding.
    * Removed outliers using the interquartile range (IQR) method.
4.  **Feature Engineering and Selection:**
    * Extracted time based features.
5.  **Predictive Modeling:**
    * Implementation of various regression models to predict weekly sales.
    * Future steps, not completed in provided code, would include model evaluation and selection.
6.  **Business Insights:**
    * Analysis of the impact of unemployment rate, seasonality, temperature, and consumer price index on weekly sales.
    * Identification of top and worst performing stores.
    * Forecasting sales for the next 12 weeks.

## 4. Dataset Description

The "Walmart DataSet.csv" dataset contains the following columns:

* **Store:** Store number.
* **Date:** Week of sales.
* **Weekly_Sales:** Sales for the given store in that week.
* **Holiday_Flag:** If it is a holiday week.
* **Temperature:** Temperature on the day of the sale.
* **Fuel_Price:** Cost of the fuel in the region.
* **CPI:** Consumer Price Index.
* **Unemployment:** Unemployment Rate.

## 5. Results and Observations

* The target variable (Weekly_Sales) was found to be normally distributed.
* Outliers were identified and removed from numerical features.
* The dataset was cleaned and prepared for modeling.
* Time based features were created to help with the seasonality of the data.
* The code provided shows the data preparation and EDA stages, but does not contain the predictive modeling or forecasting section.

## 6. Conclusion

This project successfully loaded, cleaned, and explored the Walmart sales dataset. The EDA provided valuable insights into the relationships between various factors and weekly sales. The data preprocessing steps ensured that the dataset was ready for predictive modeling.

## 7. Future Work

Future steps for this project include:

* Developing and evaluating predictive models for forecasting weekly sales.
* Using time series models to forecast sales.
* Performing feature selection to improve model performance.
* Providing detailed answers to the business questions related to the impact of various factors on sales.
* Forecasting sales for the next 12 weeks and providing actionable insights to the retail store.
* Evaluating the models using time series evaluation metrics.
* Testing different models, and comparing the results.
* Refining the outlier detection method.
