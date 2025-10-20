# Workflow Analysis for Telegram Financial Tracker Bot

## Description
This workflow automates tracking financial transactions reported via a Telegram bot, categorizing them, and storing them in a Google Sheet.

## Input Details
The workflow is triggered by an income or expense message received from a user via a Telegram bot.

## Process Summary
The workflow receives a message from a Telegram bot, extracts the transaction type (income/expense), amount, and category using a regular expression. It then formats the date and time, and appends this information along with the transaction details to a specified Google Sheet. Subsequently, it constructs a confirmation message and sends it back to the user via the Telegram bot.

## Output Details
The workflow updates a Google Sheet with financial transaction details and sends a confirmation message to the Telegram user.
