# Workflow Analysis for Euro Exchange Rate Processor

## Description
This workflow fetches Euro exchange rates from a specified API, processes the exchange rate data, and stores it in a Google Sheet and a local file.

## Input Details
This workflow is manually triggered.

## Process Summary
The workflow starts by fetching exchange rate data for EUR from the 'Frankfurter' API. It then converts the API response from XML to JSON format to make processing easier. Next, it extracts the relevant exchange rate information for each currency into separate items. Finally, it formats the exchange rate data in a table structure suitable for a Google Sheet and stores the raw data in a local HTML file.

## Output Details
The workflow outputs processed exchange rate data to a Google Sheet and saves the raw data to a local HTML file.
