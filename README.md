# 📈 Customer Sales Forecasting with Machine Learning

This project focuses on time series forecasting of monthly customer sales using machine learning and deep learning models. It leverages data preprocessing, feature engineering, and modeling techniques to predict future sales based on historical transaction records.

## 🧠 Models Used

- Linear Regression
- (Optional to extend) Random Forest, XGBoost, LSTM

## 📁 Dataset

The project uses a sample dataset: `sales_data_sample.csv`.

Key fields include:
- `ORDERDATE`: The date of the transaction
- `SALES`: Sales value for each order
- Other customer and product-related metadata

## 📊 Workflow Summary

1. **Load and Explore Dataset**
   - Parse the dataset
   - Check for null values and data types

2. **Preprocessing**
   - Convert `ORDERDATE` to datetime
   - Group by month and sum sales
   - Calculate monthly sales difference for stationarity

3. **Feature Engineering**
   - Create lag features for 12 months
   - Normalize features using MinMaxScaler

4. **Train/Test Split**
   - Split the last 12 months as test data
   - Prepare input features and target variable

5. **Modeling**
   - Train a Linear Regression model
   - Predict sales difference, convert to actual sales
   - Evaluate performance using MSE, MAE, and R²

6. **Visualization**
   - Plot actual vs. predicted sales

## 📈 Output Example

The project visualizes:
- Raw monthly sales trends
- Transformed sales difference
- Predicted vs actual sales using a linear regression model

## 🚀 Getting Started

### Prerequisites

Install required packages:
```bash
pip install pandas numpy matplotlib scikit-learn xgboost tensorflow
