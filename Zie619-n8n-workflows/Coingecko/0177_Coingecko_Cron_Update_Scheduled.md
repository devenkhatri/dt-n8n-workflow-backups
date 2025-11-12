# Workflow Analysis for Update Crypto Values

## Description
This workflow automatically updates cryptocurrency prices in an Airtable portfolio and calculates the total portfolio value hourly.

## Input Details
The workflow is triggered automatically every hour by a cron scheduler and fetches cryptocurrency symbols from an Airtable 'Portfolio' table.

## Process Summary
The workflow starts by triggering every hour, then retrieves cryptocurrency symbols from the Airtable 'Portfolio' table. For each symbol, it fetches the current USD price from CoinGecko. It then updates the 'Present Price' field for each crypto asset in Airtable. After updating prices, it fetches all 'Present Value' entries from the portfolio, sums them using a custom function, and appends the total portfolio value to a separate 'Portfolio Value' table.

## Output Details
The workflow updates individual crypto prices in the 'Portfolio' Airtable and appends the calculated total portfolio value to the 'Portfolio Value' table.

## Tags
cryptocurrency, Airtable, CoinGecko, portfolio tracking, cron, automation, price update, financial data
