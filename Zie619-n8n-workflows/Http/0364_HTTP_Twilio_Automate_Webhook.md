# Workflow Analysis for BillBot

## Description
This workflow automatically processes receipts sent via Telegram, extracts key billing information like amount, merchant, date, and category, saves the data to a Google Sheet, and sends confirmation messages via Telegram and SMS.

## Input Details
The workflow is triggered when a user sends a receipt image or file to a Telegram bot.

## Process Summary
The workflow starts by receiving a receipt via a Telegram bot. It then sends the receipt to an external receipt parsing service via HTTP request to extract structured data. Relevant details like amount, merchant, date, time, category, and submitter are extracted and formatted. The formatted data is appended to a Google Sheet for expense tracking. Finally, a confirmation message is sent back to the user via Telegram, and an SMS notification is sent to a configured phone number with submission details and a link to the Google Sheet.

## Output Details
The workflow adds the parsed receipt data to a Google Sheet and sends confirmation messages via Telegram to the user and via SMS to a predefined number.

## Tags
receipt processing, expense tracking, Telegram bot, Google Sheets, SMS notification, automation, production-ready
