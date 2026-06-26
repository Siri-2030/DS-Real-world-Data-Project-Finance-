Stock Market Trend Predictor 

An End-to-End Financial Data Analysis and Machine Learning Project

📖 Overview


This project demonstrates a complete data science pipeline applied to real-world financial data. It automatically fetches historical stock market data for Apple Inc. (AAPL), engineers custom financial indicators (like Moving Averages and Volatility), performs exploratory data analysis (EDA), and trains a Random Forest machine learning model to predict the stock's future directional movement (Up/Down).

✨ Key Features

Live Data Ingestion: Uses the yfinance API to pull real, up-to-date market data directly from Yahoo Finance.

Feature Engineering: Calculates 20-day and 50-day Simple Moving Averages (SMA), Daily Returns, and rolling Volatility.

Exploratory Data Analysis: Generates correlation heatmaps and overlays moving averages on price charts to visualize trends.

Predictive Modeling: Utilizes a Random Forest Classifier to predict the next day's closing direction.

Robust Evaluation: Implements time-series splitting (preventing data leakage) and evaluates the model using accuracy scores, classification reports, and a confusion matrix.

🛠️ Prerequisites & Installation

To run this project, you need Python installed on your system.

1. Clone or Download the Project

Ensure the python script (e.g., main.py or predict.py) is saved in your project directory.

2. Install Required Libraries

Open your terminal (or Command Prompt / PowerShell) and run the following command to install the necessary dependencies:

Bash

python -m pip install yfinance pandas matplotlib seaborn scikit-learn
(Note: If the command above fails on Windows, try using py -m pip install... instead).

🚀 How to Run

Navigate to the project directory in the terminal and execute the script:

What to Expect Upon Running:

Console Output: The terminal will display the shape of the dataset before and after cleaning, followed by the model's training status.

Dashboard 1 (EDA): A window will pop up showing the historical stock price with moving average overlays, alongside a feature correlation heatmap. (You must close this window for the script to continue).

Dashboard 2 (Evaluation): A second window will appear showing the Confusion Matrix of the model's predictions.

Final Report: The terminal will print out the model's overall accuracy, a detailed classification report, and key project conclusions.

🧠 Project Conclusions
Market Noise: Financial data is inherently noisy and highly volatile. Predicting exact future prices with basic models is incredibly difficult, which is why this project focuses on directional movement (binary classification: Up or Down).

Feature Importance: EDA reveals that while moving averages strongly correlate with the raw price, engineered features like Daily Returns and Volatility provide independent signals that are more useful for the machine learning algorithm.

Model Edge: In algorithmic trading, a model consistently achieving above a 52-53% accuracy on out-of-sample data is often considered sufficient to generate a statistical and profitable edge.

Domain: Financial Data Science | Language: Python