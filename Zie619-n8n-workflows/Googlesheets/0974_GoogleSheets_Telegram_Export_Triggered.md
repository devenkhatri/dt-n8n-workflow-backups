# Workflow Analysis for Save Telegram reply to journal spreadsheet

## Description
This workflow automatically saves journal entries from Telegram replies into a Google Spreadsheet. It ensures that only replies from a specific user to a designated bot are captured and logged with the corresponding date.

## Input Details
The workflow is triggered by a new message in Telegram that is a reply to a bot message, and it receives the message content and metadata from Telegram.

## Process Summary
The workflow starts when a Telegram message is received. It checks if the message is a reply to the bot and from the authorized user. If valid, it extracts the journal entry text and the associated date from the original bot message. The parsed data (entry and date) is then appended to a specified Google Sheet. If any error occurs during execution, it is handled by an error handler node.

## Output Details
The workflow appends the validated journal entry and date to a Google Spreadsheet.

## Tags
Telegram, Google Sheets, journaling, automation, n8n, production-ready
