<p align="center">
  <img src="https://github.com/ashish78566/ML_Projects/blob/main/Wine%20Quality/wine%20images.jpeg" alt="Wine Image" width="250">
</p>
# 🍷 Wine Quality Prediction – Machine Learning Project

This project focuses on building a machine learning model to **predict the quality of wine** based on its chemical properties. The notebook includes data preprocessing, EDA, feature engineering, model training, and evaluation using multiple ML algorithms.

---

## 📌 Problem Statement  
Develop a machine learning model that can accurately **classify wine quality** using physicochemical inputs provided in the dataset.

---

## 📊 Dataset Insights  
Each wine record includes several chemical features:

- Fixed acidity  
- Volatile acidity  
- Citric acid  
- Residual sugar  
- Chlorides  
- Free sulfur dioxide  
- Total sulfur dioxide  
- Density  
- pH  
- Sulphates  
- Alcohol  
- Quality *(target)*  

These features help determine the final quality score of wine.

---

## 🔧 Project Workflow

### 1️⃣ **Data Preprocessing**
- Handling missing values  
- Treating outliers  
- Scaling numerical variables  
- Encoding quality labels (if categorical)  

### 2️⃣ **Exploratory Data Analysis**
- Distribution plots  
- Correlation matrix  
- Pairwise relationships  
- Importance of chemical features  

### 3️⃣ **Feature Engineering**
- Normalization / Standardization  
- Creating quality groups (Low, Medium, High)  
- Removing redundant or highly correlated predictors  

### 4️⃣ **Model Training**
Models used:
- Logistic Regression  
- Random Forest Classifier  
- XGBoost Classifier  
- Support Vector Machine  
- KNN  

Evaluation metrics:
- Accuracy  
- Precision / Recall  
- F1 Score  
- Confusion Matrix  

### 5️⃣ **Model Evaluation**
Final model selected based on:
- Highest F1 score  
- Balanced performance on all quality classes  
- Lowest misclassification rate  

---

## 📈 Output (Model Predictions)
Example prediction:Predicted Wine Quality: 7 (Good)


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
├── Wine Quality Prediction.ipynb # Main ML notebook
├── winequality.csv # Dataset file
├── README.md # Project documentation



