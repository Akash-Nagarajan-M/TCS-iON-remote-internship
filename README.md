# Sales Forecasting with Time Series Analysis

## Overview

This project aims to forecast product sales using time series analysis and two different models: SARIMAX and Prophet. The analysis is performed on a historical sales dataset containing information about sales across various stores and items. The goal is to build accurate sales forecasting models and gain insights into sales patterns over time.

## Dataset

The dataset used for this analysis is available in `data.csv`. It contains the following columns:

- `date`: The date of the sales record.
- `store`: The store ID where the sales occurred.
- `item`: The item ID being sold.
- `sales`: The number of units sold on that particular date.

## Files

- `data.csv`: The original dataset containing historical sales data.
- `test.csv`: A separate test dataset for evaluating model performance on unseen data.
- `sales_forecasting.ipynb`: Jupyter Notebook containing the complete analysis and code implementation.
- `README.md`: This file providing an overview of the analysis and instructions.

## Data Preprocessing

The data preprocessing steps include:

- Importing the dataset and necessary libraries.
- Converting the `date` column to the appropriate date format.
- Handling any missing values if present.
- Exploring the data to identify any trends, seasonality, or outliers.

## SARIMAX Model

The SARIMAX model is implemented using the `statsmodels` library. The following steps are performed:

- Exploratory Data Analysis (EDA) to understand the time series characteristics.
- Splitting the dataset into training and testing sets.
- Hyperparameter tuning to find the best combination of SARIMA orders and seasonal orders using AIC.
- Training the SARIMAX model on the training set.
- Evaluating the model's performance on the test set.

## Prophet Model

The Prophet model is implemented using the `Prophet` library. The following steps are performed:

- Data preprocessing to prepare the data in the required format for Prophet.
- Splitting the dataset into training and testing sets.
- Training the Prophet model on the training set.
- Making predictions on the test set and visualizing the forecasts.

## Results and Forecasting

The results of both the SARIMAX and Prophet models are presented with visualizations and performance metrics. The sales forecasting is also performed on future dates using both models.

## Conclusion

The time series analysis and sales forecasting provide valuable insights into the sales patterns and future trends for different items and stores. The performance of both the SARIMAX and Prophet models is compared, and the best model for forecasting sales is identified based on various evaluation metrics.

For more details and code implementation, please refer to the Jupyter Notebook `sales_forecasting.ipynb`.

## Dependencies

The following Python libraries are required to run the code:

- pandas
- numpy
- matplotlib
- statsmodels
- prophet

## How to Run the Code

1. Ensure you have installed all the required libraries as mentioned in the Dependencies section.
2. Clone this repository to your local machine or download the files.
3. Open the Jupyter Notebook `sales_forecasting.ipynb` using Jupyter or any compatible notebook environment.
4. Follow the step-by-step instructions in the notebook to perform the analysis and run the code cells.

Feel free to customize this README further based on your specific analysis, insights, and any additional information you want to include. You can also add a section on how to interpret the results, potential use cases, or limitations of the analysis if applicable. Happy forecasting!
