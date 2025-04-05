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

   
