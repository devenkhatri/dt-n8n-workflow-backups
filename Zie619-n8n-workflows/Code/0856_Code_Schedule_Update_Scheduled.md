# Workflow Analysis for Daily Currency Exchange Rate Updater

## Description
This workflow automatically fetches the latest USD exchange rates every day at 8:00 AM, formats the data, and updates both a main rate sheet and an archive log in Google Sheets.

## Input Details
The workflow is triggered by a daily schedule at 8:00 AM and fetches exchange rate data from an external API using a provided API key.

## Process Summary
The workflow starts with a scheduled trigger that initiates an HTTP request to retrieve the latest USD-to-all-currencies exchange rates. The response is processed by a code node to extract the conversion rates. A Set node formats key fields like the base currency and the last update time in a human-readable format. A Merge node combines this formatted metadata with the full exchange rate data. Finally, the workflow writes the updated rates to two Google Sheets: one that updates the current rate sheet and another that appends a new row to an archive log.

## Output Details
The workflow updates a Google Sheet with the latest USD exchange rates and appends a historical record to an archive sheet within the same document.

## Tags
currency exchange, Google Sheets, automation, scheduled workflow, financial data, API integration, data logging
