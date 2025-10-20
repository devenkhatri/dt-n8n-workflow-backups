# Workflow Analysis for Invoice Data Extraction with LlamaParse

## Description
This workflow automates the extraction of key data from invoice documents using LlamaParse and stores the extracted information in a Google Sheet. It also includes steps for language detection and translation if needed.

## Input Details
The workflow is triggered manually and receives invoice document data as input.

## Process Summary
First, the workflow checks if a document is present for processing. Then, LlamaParse is used to extract structured data from the invoice document. After extraction, it prepares the data into a format suitable for Google Sheets, mapping the extracted fields to specific columns. Finally, the extracted and formatted invoice data is appended as a new row to a designated Google Sheet.

## Output Details
The workflow outputs extracted invoice data as a new row in a Google Sheet.
