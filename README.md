# Trading Bot

## Overview

This trading bot uses financial sentiment analysis to make trading decisions based on financial news.
The bot will place a buy order if there is positive sentiment, and vice versa.

## Future improvements

Future improvements can include another model that predicts whether the stock price will go up or down based on historical stock market prices,
and the bot will place a buy order if there is positive sentiment AND model predicts stock price goes up, and vice versa.

## Tools used

**FinBERT**, a pre-trained NLP model, is used to analyse financial text and give softmax outputs for three labels: positive, neutral, and negative.

It uses **Alpaca’s API** for trading operations and Yahoo Finance for historical data during backtesting.

**Pytorch** and **Transformers** are used to load and run the FinBERT model for sentiment analysis.

**Lumibot** is used to create and test trading strategies.
