# LSTM-GAN-architecture-for-stock-price-prediction

This work combines time-series data and twitter sentiment analysis model to predict the price of a stock for a given day. A CGAN with stacked bi-directional LSTM as generator and GRU as discriminator along with conditional parameter of sentiment scores provides best results according to the chosen performance metrics (RMSE). 

## Motivation
Stock market prediction is a challenging and popular problem in the field of finance.
Deep learning models can be used to derive patters in historical data and natural language processing can be used to understand market sentiment.
Using extensive feature engineering techniques and exploring novel architectures to do so can greatly improve the accuracy of the prediction of price movements.
Such models can be used by investors and economists to beat the market and understand the dynamics of the system.


## Modules
1. Data (collection, pre-processing and feature engineering)
   _ Stock price time-series data is collected from Python library yfinance. The historical data contains Open, Low, High, Close, Adjusted Close and Volume attributes. 
   _ Amazon.com Inc. stock is used and data from 01-01-2021 to 01-01-2024 is collected.
   _ Technical indicators like SMA, MACD, RSI, ATR, Bollinger Bands and RSV, and Fourier transform values of closing price of stock are added as additional parameters to the dataset.
   _ XGBoost is performed for feature analysis.
   _ Variational encoders are used to extract latent space features. 



2. Implementing Deep learning models (LSTM, GRU, GAN) and designing and developing CGAN model
   _ Designing and developing the deep learning models namely, LSTM, GRU and GAN which will later be used to compare prediction results with proposed CGAN architecture.
   _ A time step of 10 is used to predict next 1 day stock price.


4. Web Scraping and Sentiment Analysis
   _ The financial news is collected from SeekingAlpha, a leading finance news outlet.
   _ Amazon.com Inc. stock is used and news from 01-01-2021 to 01-01-2024 is collected.
   _ Web scraping is done using Selenium and Beautiful Soup.
   _ FinBERT is used to get sentiment scores.

## Results
![image](https://github.com/user-attachments/assets/024f303b-b98b-4d55-91a8-0f51a96ce8cf)









