# Workflow Analysis for Binance Telegram Price Alert

## Description
This workflow monitors the price of a specified cryptocurrency on Binance and sends a Telegram message if the price crosses a predefined threshold.

## Input Details
This workflow is triggered every 5 minutes by a Cron job.

## Process Summary
The workflow starts by defining the cryptocurrency symbol, target price, and price type (e.g., above or below). It then retrieves the current price of the cryptocurrency from Binance. The current price is compared to the target price based on the specified price type. If the condition is met, a Telegram message is constructed with the current price and sent to a specified chat.

## Output Details
The workflow sends a Telegram message with the cryptocurrency price alert.
