# Predictive Football Betting Model for West Ham United (2023 Season)

## Overview
This project develops a data analytics pipeline to predict West Ham United’s match outcomes in the 2023 Premier League season, designed for sports betting applications. Using the [football-data.org](https://www.football-data.org) API, I collected match data, engineered features like "points scored vs. opponent defense strength," and trained a random forest model with scikit-learn. The model achieved a hypothetical 89% accuracy, yielding a simulated £200 profit on £240 invested at even odds. Visualizations (confusion matrix, cumulative wins/losses, profit trends) enhance storytelling, and the model is deployed via Flask for real-time predictions.

## Features
- **Data Collection**: Fetches West Ham United’s 2023 season data using a free football API.
- **Feature Engineering**: Computes rolling averages and relative scoring metrics.
- **Modeling**: Random forest classifier predicts match wins.
- **Evaluation**: Backtests performance with accuracy and profit metrics.
- **Visualizations**: Includes confusion matrix, win/loss trends, and profit plots.
- **Deployment**: Flask app delivers live win probabilities.

## Technologies
- **Python**: pandas, numpy, scikit-learn, requests, Flask, matplotlib, seaborn
- **Machine Learning**: Random Forest Classifier
- **APIs**: football-data.org RESTful API

## Setup Instructions
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/ibryam/west-ham-united-betting-model.git
   cd west-ham-united-betting-model

2. Install Dependencies:
   pip install -r requirements.txt

3. Get an API Key:
   Register at football-data.org for a free API key.
   Replace "YOUR_API_KEY_HERE" in the scripts with your key.

4. Run the Pipeline:
   Execute step1_data_gathering.py to fetch data.
   Run step2_preprocessing.py to preprocess.
   Train the model with step3_modeling.py.
   Evaluate and visualize with step4_evaluation.py.
   Deploy with step5_deployment.py (e.g., python step5_deployment.py).



Usage
   Backtesting: Run step4_evaluation.py to see accuracy, profit, and generate plots:
   Accuracy: 0.89
   Games: 37, Bets Placed: 12, Wins: 11, Losses: 1
   Total Profit: £200.00

Live Predictions: Start the Flask app and query http://localhost:5000/predict for real-time win probabilities.
Visualizations: Check confusion_matrix.png, wins_losses_trend.png, and profit_trend.png.

Visualizations

Confusion Matrix


![image](https://github.com/user-attachments/assets/d39fefb5-3cf4-46f6-ad46-3c86f934abb1)

Cumulative Wins and Losses


![image](https://github.com/user-attachments/assets/66c53441-5b31-42ca-9d8e-62605c4e0f7c)


Cumulative Profit


![image](https://github.com/user-attachments/assets/00d71224-4e1a-436a-9b8b-13b5c9e5fef5)




Project Structure

├── step1_data_gathering.py       # Fetches match data

├── step2_preprocessing.py        # Cleans and engineers features

├── step3_modeling.py             # Trains the random forest

├── step4_evaluation.py           # Backtests and visualizes

├── step5_deployment.py           # Flask app for live predictions

├── requirements.txt              # Dependencies

├── west_ham_2023_raw.csv         # Raw data

├── west_ham_2023_features.csv    # Features

├── west_ham_2023_target.csv      # Targets

├── west_ham_rf_model.pkl         # Trained model

├── confusion_matrix.png          # Visualization 1

├── wins_losses_trend.png         # Visualization 2

├── profit_trend.png              # Visualization 3

└── README.md                     # This file

Results

Accuracy: 89% (based on simulated data)

Profit: $200 on £240 invested (assuming £20 bets at even odds)

Key Insight: Model performs above random guessing (50%), suggesting betting potential.


Contact

GitHub: ibryam

Email: ibryamfibryam@gmail.com

