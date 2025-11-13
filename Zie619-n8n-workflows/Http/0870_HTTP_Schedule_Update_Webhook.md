# Workflow Analysis for Daily Crypto Market Summary Bot

## Description
This workflow automatically fetches the latest 24-hour price data for Bitcoin (BTC), Ethereum (ETH), and Solana (SOL) from Binance, analyzes key market metrics like volatility, trading volume, and price momentum, and sends a richly formatted market summary to a Telegram chat every hour.

## Input Details
The workflow is triggered on a schedule (every hour at minute 5) and pulls public cryptocurrency price data from the Binance API.

## Process Summary
The workflow starts with a scheduled trigger that runs hourly. It then fetches 24-hour price change data for all USDC trading pairs from Binance. A custom function filters the data to only include BTC, ETH, and SOL, calculates analytics like volatility, momentum, and market comparison, and formats the results into a human-readable HTML message. The message is split into chunks to comply with Telegram's 4096-character limit. Finally, each message chunk is sent to a specified Telegram chat.

## Output Details
The workflow sends one or more formatted HTML messages summarizing crypto market activity to a Telegram chat.

## Tags
crypto, binance, telegram, market-data, automation, hourly-report, btc, eth, sol
