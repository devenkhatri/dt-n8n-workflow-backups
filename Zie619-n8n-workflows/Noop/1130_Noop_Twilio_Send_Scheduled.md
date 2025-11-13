# Workflow Analysis for Get the price of BTC in EUR and send an SMS when the price is larger than EUR 9000

## Description
This workflow automatically monitors the price of Bitcoin in Euro and sends a notification if it exceeds a certain threshold.

## Input Details
This workflow is triggered every minute by a scheduled cron job.

## Process Summary
The workflow starts by fetching the current price of Bitcoin in EUR from CoinGecko. It then checks if the obtained price is greater than or equal to 9000 EUR. If the condition is met, an SMS message is sent via Twilio with the current price. If the price is below 9000 EUR, the workflow does nothing further.

## Output Details
The workflow sends an SMS notification via Twilio if the Bitcoin price in EUR is 9000 or more.

## Tags
automation,n8n,production-ready,excellent,optimized
