Yes Bank Stock Price Prediction using Machine Learning
Project Overview
The Indian banking sector plays a vital role in the country's economy, and stock price movements often reflect investor confidence and market sentiment. This project focuses on predicting the monthly closing stock price of Yes Bank using historical market data. The study is particularly significant because the bank experienced major volatility following the fraud case involving its former CEO, Rana Kapoor, which led to a sharp decline in investor confidence and stock value.
Objective
The primary objective of this project is to analyze historical stock price trends and develop a machine learning model capable of accurately predicting the monthly closing price of Yes Bank shares.
Dataset
The dataset contains monthly stock price data from Yes Bank's inception and includes:
Date
Opening Price
Highest Price
Lowest Price
Closing Price
These variables provide comprehensive information about the stock's market performance over time.
Methodology
1. Data Preprocessing
Converted the Date column into datetime format.
Sorted data chronologically to preserve the time-series structure.
Checked for missing values and data inconsistencies.
2. Exploratory Data Analysis (EDA)
Analyzed long-term stock price trends.
Visualized price movements and volatility patterns.
Performed correlation analysis between stock price variables.
Identified the impact of major financial events on stock performance.
3. Model Development
Used Opening, High, and Low prices as input features.
Selected Closing Price as the target variable.
Split data into training and testing sets without random shuffling to maintain temporal order.
Implemented a Linear Regression model as the baseline prediction algorithm.
4. Model Evaluation
The model was evaluated using:
Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
R² Score
Results
The Linear Regression model achieved strong predictive performance with:
High R² score indicating strong explanatory power.
Low prediction error across test observations.
Good alignment between actual and predicted closing prices.
Visual comparisons confirmed the model's ability to capture overall market trends, including periods of significant volatility.
Conclusion
This project demonstrates the effectiveness of machine learning techniques in forecasting stock prices using historical market data. Despite the impact of major financial disruptions, the Linear Regression model successfully captured underlying price patterns and delivered reliable predictions.
