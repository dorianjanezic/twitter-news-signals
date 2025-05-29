# twitter-news-signals

## Project Overview

This project aims to analyze tweets from influential Twitter accounts to identify trading signals for cryptocurrencies. The core idea is to collect tweets and align them with market price data, enabling the backtesting and comparison of various trading strategies based on social sentiment and real-time information.

## Key Components

### Data Collection
Gather tweets from selected influential accounts and store them in a structured database. For each tweet, record the price of relevant cryptocurrencies at the time of the tweet and at intervals after (such as 5, 10, and 30 minutes later).

### Signal Extraction
Use different models to analyze tweets. These include fast NLP models (like RoBERTa/Bertha) for sentiment and ticker extraction, as well as advanced AI models (such as Claude) with custom prompts to interpret tweet content.

### Backtesting
Simulate trading strategies using the extracted signals and the aligned price data. Evaluate strategies based on metrics like returns, risk-adjusted performance, and signal accuracy.

### Strategy Comparison
Compare the effectiveness of different models and prompt structures. Assess how execution speed (the time between tweet publication and signal processing) impacts strategy performance, especially in volatile markets.

### Performance Evaluation
Use quantitative metrics such as Sharpe ratio, win rate, and slippage to determine the best-performing strategies. Test strategies under different market conditions and latency scenarios to understand their robustness and sensitivity to execution delays.

## Project Goals

- Build a robust pipeline for collecting and aligning tweet and price data
- Enable rapid experimentation with multiple strategy types and models
- Quantitatively evaluate the importance of execution speed for different trading approaches
- Provide clear, actionable insights into which strategies perform best and under what conditions
