# AlgoBulls_Task

Install:

pip install alpha_vantage
pip install pandas

Usage:

To get the API data simply use :

ts = TimeSeries(key='TZC4MVZ8NEY5J1WJ')
self.data, meta_data = ts.get_intraday(self.symbol)
