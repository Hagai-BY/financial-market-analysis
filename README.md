# Financial Market Analysis

This project combines trading strategies using the UT-BOT indicator, financial data analysis, and sentiment analysis on market news and Reddit posts.

---

## 📌 **Project Overview**
This project is divided into three main parts:
1. **Data Cleaning & Processing** – Handling missing data and outliers in financial datasets.  
2. **Trading Strategy (UT-BOT)** – Developing and backtesting a trading strategy using the UT-BOT indicator and ATR-based trailing stop loss.  
3. **Sentiment Analysis** – Analyzing sentiment of financial news and Reddit posts using NLP (Natural Language Processing) with `distilroberta-financial-sentiment` model.  

---

## 🚀 **Highlights**
✅ **Financial Data Retrieval** – Data pulled directly using `yfinance`, `Reddit API` (`PRAW`) and financial news with `Trafilatura`  
✅ **Advanced Data Cleaning** – Handling missing values, outliers, and data normalization  
✅ **UT-BOT Trading Strategy** – ATR-based trailing stop loss and dynamic entry/exit signals  
✅ **Sentiment Analysis with NLP** – Using `distilroberta-financial-sentiment` to assess market sentiment  
✅ **Full NLP Pipeline** – Structured process for data collection → cleaning → sentiment scoring → result aggregation  
✅ **Virality Metric** – Calculating a weighted virality score based on likes and comments  
✅ **Backtest Results** – Performance evaluation and optimization using dynamic stop loss  


---

## 🏆 **Technical Details**
### 📥 **1. Data Retrieval**
- Fetched Tesla stock data using `yfinance`  
- Pulled Reddit posts using `PRAW` (Python Reddit API Wrapper)  
- Collected financial news using `Trafilatura` for web scraping  

### 🔎 **2. Data Cleaning & Processing**
- Detected outliers using IQR (Interquartile Range)  
- Handled missing values using a 20-day moving average  
- Adjusted stock prices based on dividends and splits  

### 📊 **3. Trading Strategy (UT-BOT)**
- Built UT-BOT strategy using ATR-based trailing stop loss  
- Used `STC` (Schaff Trend Cycle) for trend confirmation  
- Dynamic stop loss calculation based on key value and ATR  

### 🧠 **4. Sentiment Analysis**
- Employed `distilroberta-financial-sentiment` for sentiment scoring  
- Combined sentiment from post title + content  
- Created a weighted sentiment score  
- Designed a virality metric using:  
    - **Likes × 1** + **Comments × 0.3**  
    - Normalized using log transformation  
- **Reddit API** – Collected Reddit posts using `PRAW`  
- **Financial News API** – Collected financial news articles using `Trafilatura` for web scraping  
- **Full NLP Pipeline** – Built a structured pipeline for:  
    - **Data collection** → **Cleaning** → **Sentiment scoring** → **Result aggregation**  
    - Applied pre-processing for tokenization, stopword removal, and text normalization  
- Weighted sentiment and virality scores combined to generate a final market sentiment index  


---


