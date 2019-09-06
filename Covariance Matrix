import pandas as pd
import matplotlib.pyplot as plt
import pandas_datareader as web
from numpy import array
from numpy import mean
from numpy import var
import numpy as np
tickers = ['MSFT', 'RACE']
start = '2015-11-01'
end = '2019-05-09'
data_source = 'yahoo'

Google = ['GOOG']
Ferrari = ['RACE']

f = web.DataReader(Ferrari, data_source, start, end)
ferrari_result = f['Close']

g = web.DataReader(Google, data_source, start, end)
google_result = g['Close']

google_result.head()

all_data = web.DataReader(tickers, data_source, start, end)
all_frame = all_data['Close']


corr = all_frame.corr()

def corr(a, b, c, d, e):
  all_data = web.DataReader([a, b, c, d, e], data_source, start, end)
  all_frame = all_data['Close']
  return  all_frame.corr()
  
def cov(a, b):
  all_data = web.DataReader([a, b], data_source, start, end)
  all_frame = all_data['Close']
  return all_frame.cov()
  
  corr('msft', 'tsla', 'abx.to', 'gold', '^GSPC')
