# Workflow Analysis for Import CSV from URL to GoogleSheet

## Description
This workflow downloads a CSV file from a provided URL, processes it by filtering for specific countries (Germany, Austria, Switzerland) and the year 2023, adds a unique identifier to each row, and then uploads the resulting data to a Google Sheet.

## Input Details
The workflow is manually triggered and uses a CSV file downloaded from a URL specified in an environment variable (WEBHOOK_URL).

## Process Summary
The workflow starts by downloading a CSV file from a URL. It then parses the CSV into structured data. A unique key is generated for each row by combining the country code and year-week fields. Next, it filters the data to include only records from Germany (DE), Austria (AT), and Switzerland (CH) in the year 2023. Finally, the filtered and enriched data is appended or updated in a specified Google Sheet, using the unique key to avoid duplicates.

## Output Details
The processed data is written to a Google Sheet named 'COVID-weekly' in a specified Google Sheets document, with rows either appended or updated based on the unique key.

## Tags
CSV import, Google Sheets, data filtering, automation, n8n, production-ready, HTTP request, data transformation
