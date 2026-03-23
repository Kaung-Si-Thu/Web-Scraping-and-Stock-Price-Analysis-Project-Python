# Stock Revenue & Price Analysis Dashboard

## 📌 Project Overview
This project analyzes and visualizes stock data and revenue trends for **Tesla, Inc. (TSLA)** and **GameStop Corp. (GME)** using Python. It demonstrates how to extract financial data from online sources, perform web scraping to collect revenue data, and create interactive graphs to visualize stock performance and revenue trends.

The project highlights key Python techniques, including:
- Stock data extraction with **yfinance**
- Web scraping for company revenue data using **BeautifulSoup**
- Data visualization with **Plotly** and **Matplotlib**
- Function-driven modular code for reusable plotting

---

## ⚙️ Technologies Used
- Python 3.x
- yfinance
- Pandas
- Plotly
- BeautifulSoup
- Matplotlib
- Jupyter Notebook / Google Colab

---

## 📂 Project Workflow

### 1. Extract Stock Data
- Use `yfinance` to retrieve historical stock price data for TSLA and GME:
```python
import yfinance as yf

tesla_data = yf.download("TSLA", start="2010-01-01", end="2022-12-31")
gme_data = yf.download("GME", start="2010-01-01", end="2022-12-31")
```
### 2. Extract Revenue Data via Web Scraping
Scrape Tesla and GameStop quarterly revenue data from financial pages using BeautifulSoup:
from bs4 import BeautifulSoup
import requests

url = "https://example.com/tesla-revenue"
html_data = requests.get(url).text
soup = BeautifulSoup(html_data, "html.parser")
# Parse the revenue table

### 3. Define a Reusable Graph Function
Create a function to plot stock prices and revenue together:
def make_graph(stock_data, revenue_data, company):
    # Plot stock prices and revenue
    pass

### 4. Visualize Data
Tesla Stock & Revenue Graph
GameStop Stock & Revenue Graph

The graphs provide insights into trends, correlations, and key financial metrics.

## 📊 Sample Insights
Tesla’s stock price growth compared with quarterly revenue trends.
GameStop’s stock demonstrates higher volatility with corresponding revenue fluctuations.
Interactive graphs allow users to zoom and explore trends over time.

## 🚀 How to Run
Clone the repository:
git clone https://github.com/yourusername/Stock-Revenue-Analysis.git
Install required libraries:
pip install yfinance pandas plotly beautifulsoup4 matplotlib
Open the Jupyter Notebook or Google Colab file and run all cells step-by-step.

##👤 Author

[Kaung Si Thu]

📄 License

This project is for educational and research purposes.
