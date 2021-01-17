# Stock Market prediction with numerical + sentiment analysis 

A hybrid model is created for stock price/performance prediction
using numerical analysis of historical stock prices, and sentimental analysis of
news headlines.

# Overview
Preprocessing of news and stocks data is done followed by merging the 2 datasets such that all headlines are given due importance in predicting stock closing price. 
TextBlob and VADER sentiment analysis model from the NLTK library have been used for sentiment analysis to generate new features. This precedes the conversion of the time series data into a supervised learning problem where closing price of next day is predicted.
New features are computed which are then scaled to train a stacked LSTM (4 layer).
Test data is taken and preprocessed separtely and then the trained model predicts and visualizes the prediction vs real world data.


Datasets used: 
1. Historical stocks of BSE from 2001 till 2020: https://finance.yahoo.com/
2. Textual headline data of Times Of India from 2001 to 2020: https://bit.ly/36fFPI6


# References
1. https://www.sciencedirect.com/science/article/pii/S1877050920307924
2. https://github.com/monica110394/Stock-Market-Prediction
