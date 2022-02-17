# AlgoBulls_Task

In this task I have fetch the stock data using Alpha Vantage. Alpha Vantage delivers a free API for real time financial data and most used finance indicators in a simple json or pandas format. This module implements a python interface to the free API provided by Alpha Vantage. It requires a free API key, that can be requested from http://www.alphavantage.co/support/#api-key.

**Requirement:**

Python 3.8.8
Jupyter Notebook v2022.1.1201831736
3rd party Python modules: alpha_vantage,Pandas 1.3.3

**Usage**

Task 1:
-> To get the stock intraday data.
-> Converted the fetched data into Pandas Dataframe.
code snippet:
1. To get the data:
        ts = TimeSeries(key='TZC4MVZ8NEY5J1WJ')
        self.data, meta_data = ts.get_intraday(self.symbol)


Task 2:

-> Defined a function called indicator1 which returns the dataframe which contains two column one timestamp and other indicator(it is the running average of closing value).

code snippet:
    out_df = pd.DataFrame(columns=["Timestamp" , "Indicator"])
    out_df["Timestamp"] = inp_df["Timestamp"]
    out_df["Indicator"] = inp_df["Close"].rolling(timeperiod).mean()
    
Task 3:
-> here, made a statergy to BUY and SELL.
