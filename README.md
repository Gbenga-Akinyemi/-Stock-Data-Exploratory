# Stock Performance(AFRM, APP and RIOT) :  Exploring the Descriptives 
## Introduction
This project is focused on analyzing the stock performance of three(3) high-performing stocks, using a 1(one)  year-long daily  stock market performance. The data set includes date, variables for opening stock price, highest stock sales price per day, lowest stock sales price per day, and closing sales price for the day. The data set  includes AFRM, APP and RIOT data set.  AFRM is a  tech stock. It is a high-performing  business  globally known as Affirm Holdings, Inc. Riot Platforms, Inc. is a Blockchain Tech company, Riot Blockchain incorporated, with  proven years of record success. At the same time, AppLovin Corporation (APP) is a mobile technology company. It specializes in mobile app development, marketing, and monetization. 
## Objective: Analysis Objective 
The project focuses on providing an analytical exploration of 1-year daily stock market data set with  the aim of providing key summaries that highlight performance insight, especially the peak and trough points. 
## Methods 
Data was collected through Yahoo Finance using dedicated Python libraries for fetching finance data(yfinance ). Pandas libraries were also imported and used to set up the data frame  and data analysis. 

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


*Data Cleaning*:

   The beauty of using the Yahoo Finance library in  Pythion is that it offers the advantage of fetching pre-cleaned or pre-arranged data sets, according to the preset specification. 

*Data Analysis and Data Visualization* : 

*### Descriptive Statistics* 
Descriptive statistics offers key summary statistics for the businesses' stock market performance under the period of review, 1-year of daily stock market data.

The objective of the analysis is to provide summaries and visualization snapshots that could highlight performance insights among the firms  

*### Stock Return Analysis* 
This step analyzes performance return per firm and produces visualization to emphasize peaks and trough periods. Peaks are the steep or high points in the visualization which represent points of high returns. While troughs are the low points in the visualization which emphasizes the points of stock sales performance or returns  in the review period.

![AFRM_return_analysis](https://github.com/Gbenga-Akinyemi/-Stock-Data-Exploratory/assets/102978818/800e5f15-5d8c-44a8-a2a8-5fa6a01ba457)

![APP_return_analysis](https://github.com/Gbenga-Akinyemi/-Stock-Data-Exploratory/assets/102978818/067d5212-907f-4142-b708-10856e8dae33)


![RIOT_return_analysis](https://github.com/Gbenga-Akinyemi/-Stock-Data-Exploratory/assets/102978818/d9cc0cdf-6e6f-427b-b776-71dfc64cad35)


*Further analysis and visual representation of data using box plots*

![closing_prices_box_plot_afrm](https://github.com/Gbenga-Akinyemi/-Stock-Data-Exploratory/assets/102978818/6bac8459-bb5c-402e-b1a9-3956a294a4c2)


    
![closing_prices_box_plot_app](https://github.com/Gbenga-Akinyemi/-Stock-Data-Exploratory/assets/102978818/2ea01a18-bd8c-484c-a32e-b66d18e5fe43) 


![closing_prices_box_plot_riot](https://github.com/Gbenga-Akinyemi/-Stock-Data-Exploratory/assets/102978818/2f912b36-d9fa-46c3-9fe0-2644189bca9f) 


*Further analysis and visual representation of data using distribution plots* 


![closing_prices_distribution_afrm](https://github.com/Gbenga-Akinyemi/-Stock-Data-Exploratory/assets/102978818/7032601d-c718-442a-9717-7fd62089c1d5)



![closing_prices_distribution_app](https://github.com/Gbenga-Akinyemi/-Stock-Data-Exploratory/assets/102978818/a24a026e-75d4-4cc0-b3ab-7f2fbf14c33d) 


![closing_prices_distribution_riot](https://github.com/Gbenga-Akinyemi/-Stock-Data-Exploratory/assets/102978818/c4cd49be-b844-4aba-ad10-4fca41095cec)

## Reference 
1. Python
2. Python libraries: Yahoo Finance (finance)
3. Python libraries: Pandas 
4. Bloomberg 


