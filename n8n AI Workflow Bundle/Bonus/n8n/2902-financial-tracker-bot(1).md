# Workflow Analysis for Telegram Financial Tracker Bot

## Description
This workflow automates the process of tracking financial transactions by receiving commands and data via Telegram, recording them in a Google Sheet, and providing summaries.

## Input Details
The workflow is triggered by an HTTP webhook that receives messages from a Telegram bot.

## Process Summary
The workflow starts by extracting the Telegram message text and user ID. It then uses an IF node to check if the message is a "Start" command or a financial transaction. If it's a transaction, it extracts the type (income/expense), category, and amount using regular expressions and a Switch node. Finally, it records the transaction details in a Google Sheet, including the user, date, transaction type, category, and amount.

## Output Details
The workflow records financial transaction data into a Google Sheet for tracking and analysis.
