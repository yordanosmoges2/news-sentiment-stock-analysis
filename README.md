📌 News Sentiment & Stock Price Analysis

This project analyzes financial news headlines, computes sentiment, and measures how that sentiment correlates with daily stock price movements.
It includes data exploration, technical indicators, sentiment scoring, and correlation analysis.

📁 Project Structure
project/
├── .vscode/                    # VSCode workspace settings
├── .github/workflows/         # GitHub Actions CI
├── requirements.txt           # Python dependencies
├── README.md                  # Main project documentation
├── src/                       # Python package folder
├── notebooks/                 # Jupyter notebooks for analysis
├── tests/                     # Unit tests (placeholder)
└── scripts/                   # Script utilities

🚀 Features
✔ Task 1 – News Data Exploration

Clean raw headline data

Normalize timestamps

Validate structure

✔ Task 2 – Stock Indicators

Download historical prices (AAPL, AMZN, GOOG, META, MSFT, NVDA)

Compute Moving Averages, RSI, MACD

Plot indicators

✔ Task 3 – Sentiment & Returns Correlation

Compute sentiment with TextBlob

Aggregate sentiment by date

Merge with stock daily returns

Calculate correlation

🧠 Method Summary
Sentiment Analysis
TextBlob(x).sentiment.polarity

Daily Returns
df_price['return'] = df_price['Close_AAPL'].pct_change()

Correlation
corr = merged['sentiment'].corr(merged['return'])

📦 Installation
git clone https://github.com/yourusername/news-sentiment-stock-analysis.git
cd news-sentiment-stock-analysis
python -m venv venv
venv\Scripts\activate          # Windows
pip install -r requirements.txt

▶️ Usage
Run Jupyter Notebook
jupyter notebook

Run tests (if added later)
pytest

🔄 Git Workflow
git checkout -b task-1
git commit -m "Task 1 completed"

git checkout -b task-2
git commit -m "Task 2 completed"

git checkout -b task-3
git commit -m "Task 3 completed"

📈 Results Summary

Sentiment shows weak correlation with daily stock returns.

Technical indicators help visualize market trends.

Dataset contains noise and sentiment is not strongly predictive.

🛠 Technologies

Python

Jupyter Notebook

pandas

yfinance

TextBlob

Git & GitHub

GitHub Actions

📜 License

MIT License