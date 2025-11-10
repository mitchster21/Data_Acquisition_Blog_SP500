# Data_Acquisition_Blog_SP500
This repository contains the code and data used in the blog post "Data Acquisition: Scraping and Analyzing S&P 500 Stock Performance". The blog post demonstrates how to scrape data from Wikipedia and Yahoo Finance, merge the datasets, and perform basic exploratory data analysis (EDA) on the combined data.

## Project Overview
This project explores the question:  
**"How have S&P 500 companies performed over the past year?"**

Data was collected from:
- **Wikipedia** — for the list of all S&P 500 companies and metadata (sector, symbol, industry, etc.)
- **Yahoo Finance** — for stock price history and performance metrics

After scraping and merging both datasets, a basic **Exploratory Data Analysis** was performed to investigate:
- 1-year percentage change by company  
- Distribution of returns across sectors  
- Top/bottom performing stocks 

## Data Description
`Ticker` - Company ticker symbol 
`Company` - Full company name 
`Sector` - Industry sector classification 
`SubIndustry` - More specific industry classification
`1Y_Change(%)` - Percent change in stock price over the past year
`Volatility(%)` - Annualized volatility of daily returns
`AvgAnnualReturn(%)` - Average annualized return percentage
`MaxDrawdown(%)` - Maximum decline from peak to trough over the year

## Files
- `scrape.ipynb` — Jupyter notebook for scraping and analysis  
- `sp500_merged.csv` — Final merged dataset used in the analysis  
- `README.md` — Project documentation 

## Tools & Libraries
- **Python 3.12**
- `requests`, `BeautifulSoup4` — Web scraping  
- `pandas`, `numpy` — Data cleaning and transformation  
- `matplotlib`, `seaborn` — Data visualization 

## Summary
This project showcases data acquisition techniques and basic EDA on financial data. The findings provide insights into the performance of S&P 500 companies over the past year, highlighting trends and outliers in stock returns.