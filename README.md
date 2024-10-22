# Demand_Forecasting_System
Demand Forecasting System for Optimizing Inventory and Supply Chain Efficiency Using Historical Sales Data

This project focuses on building a system that forecasts the demand for the company's top 10 best-selling products over the next 15 weeks. By analyzing historical sales data, the aim is to help the company maintain optimal stock levels and enhance supply chain efficiency.

1. Problem Statement

The company has been collecting sales data from December 2021 to December 2023 and needs a reliable way to predict demand for its most popular products.

The goal is to forecast demand for the next 15 weeks, ensuring inventory levels are well-managed to avoid both overstocking and stockouts.

2. Data Used

We utilized several datasets to inform the forecasting model:

Transactional_data_retail01.csv & Transactional_data_retail_02.csv: These contain transaction records, such as stock codes, transaction dates, and quantities sold.

CustomerDemographics.csv: Provides information on customer types, which might help identify buying trends.

ProductInfo.csv: Includes details about products, like categories and stock codes.

3. Data Preprocessing
   
Before building the model, several preprocessing steps were applied:

The data was cleaned to address any missing or inconsistent entries.

Sales quantities were aggregated by week for each product.

Dates were formatted correctly, and any additional features necessary for forecasting were derived.

4. Demand Forecasting Model
   
We tested multiple models to accurately predict future demand:

ARIMA and Prophet were used for traditional time series forecasting.

LSTM, a deep learning model, was applied to capture more complex patterns in the sales data.

The model focuses on predicting weekly demand for the top 10 products over the next 15 weeks.

5. Model Validation

To ensure the model's predictions are accurate:

The data was split into training (December 2021 to September 2023) and validation sets (October 2023 to December 2023).

This allowed us to validate the model’s ability to generalize and not just memorize the training data.

6. Assumptions Made

Some assumptions were made to simplify the modeling process:


The model assumes that demand trends and seasonality seen in the historical data will continue into the future.

External factors such as holidays, promotions, or market disruptions are not explicitly modeled but may influence the demand.

7. Technologies Used

The following tools and technologies were used in the project:

Python for all data processing and modeling tasks.

Pandas for data cleaning, aggregation, and manipulation.

Scikit-learn, TensorFlow/Keras, and Prophet for building machine learning and time series models.
