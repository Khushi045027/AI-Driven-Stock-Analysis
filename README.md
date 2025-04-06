# AI-Driven-Stock-Analysis

*Introduction*

This project leverages LlamaIndex and Mistral AI to build an AI-powered stock analysis dashboard. The goal is to empower users—especially non-finance professionals—with a simple interface that offers:

1. Retrieval of real-time financial data via YFinance.
2. Calculation of key financial ratios such as ROIC, ROA, EBIT Margin, etc.
3. AI-generated investment recommendations based on financial health, using Mistral LLM.
4. The system combines traditional finance metrics with cutting-edge language models to provide interpretable insights for stock market decision-making.

*Tools and Technologies Used*

This project integrates a variety of open-source tools and APIs to perform financial analysis and provide intelligent recommendations:

1. Streamlit: Used to build the interactive user interface for entering stock tickers and displaying analysis.
2. YFinance: A Python wrapper for Yahoo Finance API that fetches real-time financial data such as income statements and balance sheets.
3. LlamaIndex: Acts as the orchestration layer, helping structure prompts for the language model.
4. Mistral via Ollama: An open-source local language model that analyzes financial ratios and provides investment suggestions.
5. Pandas and Numpy: Core libraries used for data manipulation and computation of financial ratios.

   
*Model Overview*

The model fetches financial statements such as income statements, balance sheets, and cash flow statements using the YFinance API. It then computes several key financial ratios:

1. Return on Invested Capital (ROIC)
2. Return on Assets (ROA)
3. Debt-to-Equity Ratio
4. Current Ratio
5. EBIT Margin
6. Operating Cash Flow to Debt Ratio

These ratios are then passed to the Mistral AI model (running locally via Ollama) through a structured prompt using the LlamaIndex framework. The model evaluates the company’s financial health and provides a recommendation to Buy, Hold, or Sell along with justification.

*How to Run the Model*

1 Prerequisites

i. Ubuntu or any Linux-based OS
ii. Python 3.8 or higher
iii. Jupyter Notebook (optional)
iv. Ollama installed for Mistral model

2. Installation Steps

i. Install Ollama:
curl -fsSL https://ollama.com/install.sh | sh
ollama run mistral

ii. Install Python dependencies:
pip install -r requirements.txt
pip install streamlit

iii. Run the Streamlit App:
streamlit run stream.py

This will open the application in your browser at: http://localhost:8501

*Output Example*

Upon entering a stock ticker (e.g., AAPL), the app will:

i. Fetch and display the financial ratios.
ii. Provide an AI-generated recommendation based on the analysis.

*Future Learning and Scope*

The project has vast potential for scaling and enhancement:

1. Multi-Stock Comparison: Support batch analysis and portfolio benchmarking.
2. Data Visualization: Integrate interactive graphs and historical trends.
3. ESG Integration: Add environmental, social, and governance metrics.
4. Advanced LLMs: Upgrade to GPT-4 or Claude for deeper contextual analysis.
5. Deployment: Host on cloud platforms such as Streamlit Cloud, Heroku, or AWS EC2.
6. Personalization: Enable user profiles and track portfolio performance.
