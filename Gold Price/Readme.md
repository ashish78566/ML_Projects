<p align="center">
  <img src="https://github.com/ashish78566/ML_Projects/blob/main/Gold%20Price/gold%20image.jpg" alt="Gold Image" width="230">
</p>

# Gold Price Prediction – Machine Learning Project

This project focuses on building a machine learning model to predict **future gold prices** using historical financial market data. The notebook includes preprocessing, feature scaling, time-series analysis, model training, and evaluation.

---

## Problem Statement
Gold is a widely traded commodity and its price is influenced by multiple economic factors.  
The goal of this project is to create a predictive ML model that can estimate future gold prices based on previous market data.

---

## Dataset Information
The dataset typically contains:

- Date  
- Gold price (target)  
- Opening, High, Low values  
- Crude oil price  
- USD price index  
- Interest rate  

These indicators help identify trends and patterns affecting gold price movement.

---

## Project Workflow

### 1. Data Preprocessing
- Load dataset  
- Handle missing values  
- Convert date column & set time index  
- Create lag features for prediction  
- Train–test split  

### 2. Exploratory Data Analysis
- Time-series plots for trend  
- Correlation heatmap  
- Seasonal trend visualization  
- Detecting volatility  

### 3. Feature Engineering
- Lag/shift features  
- Rolling averages  
- Min–Max scaling  

### 4. Model Training
Models used in this notebook include:

- Linear Regression  
- Random Forest Regressor  
- XGBoost Regressor  
- LSTM *(if applied)*  

Evaluation metrics:

- R² Score  
- Mean Absolute Error (MAE)  
- RMSE  

### 5. Model Evaluation
Final model is selected based on:

- Highest R² value  
- Lowest prediction error  
- Generalization on unseen test data  

---

## Output Example
Example model output:Predicted Gold Price: $1,955.42
