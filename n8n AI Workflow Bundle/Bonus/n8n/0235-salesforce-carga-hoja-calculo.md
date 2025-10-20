# Workflow Analysis for Salesforce Data Loader for Spreadsheet

## Description
This workflow automates the process of extracting data from a Google Sheet, transforming it, and loading it into Salesforce as new records or updating existing ones.

## Input Details
The workflow is manually triggered and receives spreadsheet data from Google Sheets.

## Process Summary
First, the workflow retrieves data from a specified Google Sheet. Next, it iterates through each row of the spreadsheet data. For each row, it constructs a JSON object that maps the spreadsheet column headers to Salesforce field names. Finally, it attempts to create a new record in Salesforce; if a record with the same unique identifier already exists, it updates the existing record instead.

## Output Details
The workflow outputs either new records created in Salesforce or updates to existing Salesforce records.
