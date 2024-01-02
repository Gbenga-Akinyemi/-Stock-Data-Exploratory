# Stock Performance(AFRM, APP and RIOT) :  Exploring the Descriptives 
## Introduction
This project is focused on analyzing the stock performance of three(3) high-performing stocks, using a 1(one)  year-long daily  stock market performance. The data set includes date, variables for opening stock price, highest stock sales price per day, lowest stock sales price per day, and closing sales price for the day. The data aset  includes AFRM, APP and RIOT data set.  AFRM is a  tech stocks. It is a high-perfroming  business  globally known as Affirm Holdings, Inc. Riot Platforms, Inc. is a Blockchain Tech company, Riot Blockchain incorporated, with  proven years of record success. While AppLovin Corporation (APP) is a mobile technology company. It specializes in mobile app development, marketing, and monetization. 
## Objective : Analysis Objective 
The project focuses on providing an analytical exploration of 1 year daily stock markert data set witht  the aim of providing key summaries that highlighting performance insight, especially the peak and trough pooints. 
## Methods 
Data was collected through Yahoo Finance using dedicated Python libraries for fetching finance data(yfinance ). Pandas libries were also imported and used to set up the data frame  and data analysis. 

 - Python Codes: 
   
    [Uploadingimport yfinance as yf
import pandas as pd

### Define the stock symbols for the companies of interest
symbols = ['AFRM', 'APP', 'RIOT']

### Specify the date range for the past month
end_date = pd.to_datetime('today')
start_date = end_date - pd.DateOffset(months=1)

### Create dictionaries to store data for each stock
stock_data = {}
key_stats = {}

### Fetch historical stock data and key financial ratios
for symbol in symbols:
    # Fetch historical stock data
    stock_data[symbol] = yf.download(symbol, start=start_date, end=end_date)

    # Fetch key financial ratios
    key_stats[symbol] = yf.Ticker(symbol).info

### Print or analyze the data as needed
for symbol in symbols:
    print(f"\nStock: {symbol}")
    print("\nHistorical Stock Data:")
    print(stock_data[symbol].head()) 
    
   Python.codes.for.fetching.data…]() 


    * Data Cleaning *


    

