<p align="center">
  <img src="https://github.com/ashish78566/ML_Projects/blob/main/IPL%20Score/ipl-logo.png" alt="IPL Logo" width="180">
</p>

# 🏏 IPL Score Prediction – Machine Learning Project

This project focuses on building a machine learning model to **predict the final innings score** of an IPL team based on overs, wickets, run rate, player performance factors, and match situation. The notebook includes full data preprocessing, EDA, feature engineering, model training, and evaluation.

---

## 📌 Problem Statement  
Build a machine learning model that can accurately **predict the final total score** of a batting team in the Indian Premier League based on real-time match inputs.

---

## 📊 Dataset Insights  
The dataset contains ball-by-ball or over-by-over match details such as:

- `batting_team`
- `bowling_team`
- `overs`
- `runs`
- `wickets`
- `runs_last_5`
- `wickets_last_5`
- `striker`
- `non-striker`
- `bowler`

These columns help understand match context and scoring patterns.

---

## 🔧 Project Workflow

### 1️⃣ **Data Preprocessing**
- Handling null values  
- Encoding categorical variables  
- Removing irrelevant features  
- Feature transformation (if required)

### 2️⃣ **Exploratory Data Analysis**
- Run distribution  
- Wickets vs runs correlation  
- Overs vs scoring rate  
- Outlier detection  
- Team-wise scoring patterns  

### 3️⃣ **Feature Engineering**
- Adding scoring momentum features  
- Recent over performance  
- Run rate calculation  
- Pressure indicators  

### 4️⃣ **Model Training**
Models used:
- Linear Regression  
- Random Forest Regressor  
- XGBoost Regressor  
- AdaBoost Regressor  

Performance metrics:
- R² Score  
- MAE  
- RMSE  

### 5️⃣ **Model Evaluation**
Final model is selected based on:
- Highest R²  
- Lowest error  
- Stability across test data  

---

## 📈 Output (Model Predictions)
The model predicts the **final IPL score** given current match state variables.  
Example output:Predicted Final Score: 178 runs


---

## 🧪 Technologies Used
- Python  
- Pandas / NumPy  
- Scikit-learn  
- Matplotlib / Seaborn  
- XGBoost  
- Jupyter Notebook  

---

## 📁 Project Structure
├── IPL Score Prediction.ipynb # Main ML Notebook
├── dataset.csv # Input data file (if included)
├── ipl-logo.png # IPL Logo
├── README.md # Project documentation

