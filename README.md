# Stock-Market-Forecasting

Stock Market Forecasting for AAPl(Apple Inc) using Stacked LSTMs.

For Data Collection - Pandas Datareader - https://pandas-datareader.readthedocs.io/en/latest/

Remote Data Access - https://pandas-datareader.readthedocs.io/en/latest/remote_data.html

For Stock Data - Tiingo - https://pandas-datareader.readthedocs.io/en/latest/remote_data.html#remote-data-tiingo

Data is collected and stored in AAPL.csv

Data available from [2015-05-27 00:00:00+00:00] to [2020-05-22 00:00:00+00:00] time.

Prediction of closing rate is done.

As LSTMs are quite sensitive to the scale of data, so the data has been scaled using MinMaxScaler

The data is then splitted in 65:35 ratio. As the data is Time series, [len(data)*0.65] is taken as training size and remaining for test.

The dataset is created using create_dataset function in Main.ipynb. 

MSE is used as the performance metrics.

The model can be further improved by changing time step and observing and also by using Bi-directional LSTMs.

Article for help - https://machinelearningmastery.com/time-series-prediction-with-deep-learning-in-python-with-keras/


