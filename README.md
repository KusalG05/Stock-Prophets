# Stock-Prophets
CS337 AI/ML Project 

## Team Members
|Roll No. | Team Member                  |
|-----|------------------------------|
| 210050043   | Desai Sai Pranav |
| 210050051   | Gangisetty Krishna Sai Kusal |
| 210050120 | PVR Sai Kumar |
| 210050153 | Sudarshanam Harshith |

Our project aims to predict the closing price of the stock using LSTM and GRU

StockMarketv1.ipynb has a code that tries to predict closing prices using only closing prices. Models used are LSTM and GRU 

StockMarketv2.ipynb has a code that tries to predict closing prices using closing prices and dividends. Models used are LSTM and GRU

StockMarketv3.ipynb has a code that tries to predict closing prices using only closing prices and dividends. The models used are LSTM and GRU. We also predicted future prices for 10 days using the last 100 days.

### General CodeWalkthrough

After importing the required libraries, we preprocessed the data
1. yf.Ticker imports data from yfinance library
2. Using TimeSeriesGenerator we can get sequential data as required. We have implemented it in generate_series.
3. Using MinMaxScaler from sklearn, we have scaled the closing indices between 0 to 1.
4. Then models were initiated with layers as mentioned in the report.
5. Then we trained the dataset using the validation set for hyperparameter tuning.
6. Then we predicted values for the test set.
7. For future values presentation in v3, we used one instance of the test set and predicted for the next few(10) days.
8. We have plotted everything
9. GRU part is implemented in a similar fashion

### How to run

You can open our files in Google Colab and run all. 
