🏏 IPL Score Prediction Using Machine Learning

Predicting First Innings Total in IPL T20 Matches

📌 Project Overview

This project builds a Machine Learning model that predicts the final first-innings score in an IPL T20 match based on the current match situation.

The model analyzes factors such as overs completed, runs scored, wickets fallen, and performance in the last 5 overs to forecast the expected final score. Multiple regression models were tested, and Linear Regression provided the best performance.

🎯 Problem Statement

Given the match context — batting team, bowling team, overs completed, current runs, wickets, and last-5-overs performance — predict the final first-innings score in an IPL match.

📂 Dataset Description

The dataset contains ball-by-ball IPL match details. After preprocessing, the following key features are used:

Input Features
Feature	Description
bat_team	Current batting team
bowl_team	Current bowling team
overs	Overs completed (e.g., 10.3)
runs	Runs scored till now
wickets	Wickets fallen till now
runs_last_5	Runs scored in last 5 overs
wickets_last_5	Wickets lost in last 5 overs
Target Variable
Feature	Description
total	Final first-innings total score
Columns Removed During Cleaning

mid, venue, batsman, bowler, striker, non-striker

Teams Considered

Only 8 consistent IPL teams were kept for modeling:

Chennai Super Kings

Mumbai Indians

Royal Challengers Bangalore

Kolkata Knight Riders

Sunrisers Hyderabad

Delhi Daredevils

Kings XI Punjab

Rajasthan Royals

🧹 Data Preprocessing

✔ Removed inconsistent teams
✔ Removed first 5 overs (too unstable for score prediction)
✔ Converted date column into datetime
✔ Applied One-Hot Encoding for teams
✔ Time-based Train/Test split (Train ≤ 2016, Test ≥ 2017)

🤖 Models Implemented

The following regression models were trained and compared:

Model	Description
Linear Regression	Best performing model
Decision Tree Regression	High variance, less accurate
Random Forest Regression	Overfitting observed
AdaBoost Regression	Did not improve performance

Linear Regression achieved the lowest MAE and RMSE on the test set.

📈 Model Evaluation Metrics

Each model was evaluated using:

MAE (Mean Absolute Error)

MSE (Mean Squared Error)

RMSE (Root Mean Squared Error)

Linear Regression provided the most stable and interpretable predictions.

🧮 Final Prediction Function

A custom Python function predict_score() takes real-time match inputs:

final_score = predict_score(
    batting_team='Chennai Super Kings',
    bowling_team='Mumbai Indians',
    overs=10.2,
    runs=85,
    wickets=2,
    runs_in_prev_5=45,
    wickets_in_prev_5=1
)
print("Projected Score:", final_score)


Outputs a predicted score such as 165–180 runs.

📊 Correlation Heatmap

A heatmap was generated to study relationships between numerical features:

Strong correlation found between current runs, last 5 overs performance, and final total.

🛠 Tech Stack

Python

Scikit-Learn

Pandas, NumPy

Matplotlib, Seaborn

📘 Project Structure
├── ipl.csv                     # Dataset
├── IPL Score Prediction.ipynb  # Full notebook
├── README.md                   # Project documentation
└── images/                     # (Optional) banners and visuals

🚀 How to Run the Project
1️⃣ Clone the repository
git clone https://github.com/your-username/ipl-score-prediction.git
cd ipl-score-prediction

2️⃣ Install dependencies
pip install -r requirements.txt

3️⃣ Run the notebook
jupyter notebook "IPL Score Prediction.ipynb"

📝 Future Improvements

🔹 Add deep learning models (LSTM for sequence data)
🔹 Include venue, toss, pitch conditions
🔹 Build a live interactive web app using Streamlit
