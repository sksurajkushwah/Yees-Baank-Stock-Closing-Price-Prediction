Yes Bank Stock Price Prediction using Machine Learning
Project Overview

The banking sector plays a crucial role in the Indian economy, and stock price movements often reflect investor confidence, market sentiment, and organizational performance. This project focuses on predicting the monthly closing stock price of Yes Bank using historical stock market data and machine learning techniques.

The study is particularly important because Yes Bank experienced significant volatility following the financial crisis and fraud allegations involving its former CEO, Rana Kapoor. These events resulted in a sharp decline in investor confidence and substantial fluctuations in the bank's stock price.

The project aims to analyze historical stock market trends, identify key factors affecting stock prices, and build predictive machine learning models capable of forecasting future closing prices.

Objective

The primary objectives of this project are:

Analyze historical stock price trends of Yes Bank.
Understand the impact of market volatility and major financial events.
Perform statistical hypothesis testing on stock market behavior.
Engineer meaningful features from historical stock data.
Build and compare multiple machine learning models.
Select the best-performing model for stock price prediction.
Evaluate model performance using appropriate regression metrics.
Dataset

The dataset contains monthly stock price data of Yes Bank and includes the following features:

Feature	Description
Date	Trading Month and Year
Open	Opening Stock Price
High	Highest Stock Price
Low	Lowest Stock Price
Close	Closing Stock Price (Target Variable)

These variables provide comprehensive information about the stock's market performance over time.

Project Workflow
1. Data Preprocessing
Converted Date column into datetime format.
Sorted observations chronologically to preserve time-series structure.
Checked for missing values and inconsistencies.
Prepared the dataset for machine learning analysis.
2. Exploratory Data Analysis (EDA)
Analyzed long-term stock price trends.
Examined closing price distributions.
Identified outliers using box plots.
Visualized moving averages and trend patterns.
Performed correlation analysis among stock price variables.
Investigated volatility and market fluctuations over time.
3. Hypothesis Testing

The following statistical hypotheses were tested:

Did the 2018 crisis significantly impact Yes Bank's stock price?
Is there a strong linear relationship between Open and Close prices?
Did stock price volatility increase after 2018?
Is there a significant difference between High and Low prices?

Statistical tests used:

Independent T-Test
Pearson Correlation Test
Levene's Test
Paired T-Test
4. Feature Engineering

Several new features were created to improve predictive performance:

Lag Features
Rolling Mean Features
Rolling Standard Deviation (Volatility)
Monthly Returns
Log Returns
Price Range
Range Percentage
5. Feature Selection
Correlation Analysis
Multicollinearity Assessment
Correlation Heatmap
Selection of highly relevant predictors
6. Data Transformation & Scaling
Applied StandardScaler to normalize feature values.
Reduced the effect of differing feature scales.
Improved model convergence and stability.
7. Dimensionality Reduction
Applied Principal Component Analysis (PCA).
Reduced feature dimensionality while retaining approximately 95% of total variance.
Minimized multicollinearity among engineered features.
8. Data Splitting & Validation
Used an 80:20 chronological train-test split.
Implemented TimeSeriesSplit (5-fold) cross-validation.
Prevented data leakage and ensured realistic forecasting evaluation.
Machine Learning Models

The following machine learning models were implemented:

Model 1: Linear Regression

Used as the baseline prediction model.

Model 2: Ridge Regression

Applied regularization and hyperparameter tuning using GridSearchCV.

Model 3: Random Forest Regressor

Captured non-linear relationships and feature interactions.

Model 4: XGBoost Regressor

Implemented gradient boosting for enhanced predictive performance.

Hyperparameter Tuning

Hyperparameter optimization was performed using:

GridSearchCV
TimeSeriesSplit Cross Validation

Models tuned:

Ridge Regression
Random Forest Regressor
XGBoost Regressor
Model Evaluation Metrics

The models were evaluated using:

Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
R² Score
Model Comparison
Model	MAE	RMSE	R² Score
Linear Regression	29.26	38.07	0.9090
Ridge Regression	31.35	40.93	0.8949
XGBoost Regressor	35.41	44.17	0.8776
Random Forest Regressor	51.01	64.00	0.7429
Final Model Selection

Linear Regression was selected as the final prediction model because it achieved:

Highest R² Score
Lowest MAE
Lowest RMSE

Final Performance:

R² Score = 0.9090
MAE = 29.26
RMSE = 38.07
Key Insights
The 2018 financial crisis significantly impacted Yes Bank's stock prices.
Open and Close prices exhibited a strong positive correlation.
Stock price volatility increased significantly after 2018.
Lag features and rolling statistics improved predictive performance.
Time-series cross-validation provided a more realistic model evaluation framework.
Conclusion

This project demonstrates the effectiveness of machine learning techniques in forecasting stock prices using historical financial data. Through comprehensive data preprocessing, feature engineering, statistical analysis, and model comparison, multiple predictive models were evaluated for forecasting Yes Bank's closing stock price.

Among all the models tested, Linear Regression achieved the best overall performance with an R² Score of 0.9090 and the lowest prediction error. The results highlight the importance of feature engineering, time-series validation, and proper model evaluation in building reliable stock price forecasting systems.

This project showcases how machine learning can support data-driven investment analysis and financial decision-making in real-world business environments.
