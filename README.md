# time-series-forecasting of cryptocurrency prices
 Time Series Forecasting of Bitcoin (BTC) Price
 
With this project, I tested three different models on crypto-currency prices to check their
forecasting ability. In the first place, I  extracted and analyzed the data used in the analysis. 
Then, I compared the ARIMA model, the Prophet procedure, and the LSTM model.
# results and conclusion
We can easily conclude that the ARIMA model is, by far, the best model. It’s probably due 
to the rolling basis logic, to calculate the forecasted upcoming value, which is similar to the 
"recency" heuristic method. Prophet did not produce good results out of the box for highly 
volatile Bitcoin prices. LSTM produced more convincing results and it could predict the trend 
much better than prophet. Predictions via prophet were stagnant and it could not recognize the 
trend in the prices. Prophet will perform better with trends that have some sort of seasonality, 
for example in cases where we have to predict website hits on an e-commerce website.
LSTM produced an MAE of upwards of 13000 in just 25 epochs, it can improve with more 
layers in the model and more epochs. Prophet produced an MAE of almost 17000 and since 
there is not much seasonality when we consider a highly volatile value of interest like the price 
of Bitcoin, there’s not a lot of parameters that can be tuned for the model. However, certain 
spike events can be added to slightly improve the model, but that is not a practical approach.
