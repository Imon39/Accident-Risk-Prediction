🚗 Pick the Safer Road – Accident Risk Prediction Game

An interactive Streamlit web app that challenges users to predict which road is safer based on real-world traffic and environmental features.
Built using an Ensemble Machine Learning Model (LightGBM + XGBoost) that predicts the accident risk level for two randomly generated roads.

🎮 Key Features

🧠 ML-Powered Predictions – Uses a weighted ensemble of LightGBM and XGBoost models.

🔀 Random Scenario Generation – Each round creates new road conditions (weather, speed, curvature, etc.).

🎯 User Challenge Mode – Guess which road is safer before seeing the model’s prediction.

📊 Risk Visualization – Displays accident risk scores using interactive bar charts.

🧩 Feature Engineering Pipeline – Automatically processes numeric, boolean, and derived features (e.g., rush_hour, lanes_speed, sq_curv).

🛠️ Tech Stack

Python

Streamlit

LightGBM

XGBoost

Pandas / NumPy

Joblib

📦 Installation
git clone https://github.com/yourusername/accident-risk-game.git
cd accident-risk-game
pip install -r requirements.txt
streamlit run app.py

🧩 Model

The model combines two trained pipelines (LightGBM and XGBoost) into an ensemble:

final_model = 0.65 * lightgbm_model + 0.35 * xgboost_model

🧠 How It Works

Two roads are generated with random environmental conditions.

The user guesses which one is safer.

The ML model predicts accident risk for both roads.

The app visualizes results and updates the user’s score.

🪪 Author

Imon Hossain
📘 Department of CSE
🏅 Kaggle: imonhossain
