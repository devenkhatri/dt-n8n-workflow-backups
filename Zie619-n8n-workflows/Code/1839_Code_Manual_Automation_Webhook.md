# Workflow Analysis for OCR receipts from Google Drive

## Description
This workflow automatically extracts text and structured data from receipts or invoices stored in a Google Drive folder using OCR technology, and saves the parsed information into a Google Sheet for easy tracking and analysis.

## Input Details
The workflow is triggered either manually via the 'Test workflow' button or automatically when a new file is added to a specified Google Drive folder.

## Process Summary
The workflow first retrieves a list of already processed files from Google Sheets and all files from a designated Google Drive folder. It then filters out files that have already been processed by comparing file IDs. For each unprocessed file, it downloads the file from Google Drive, sends it to an OCR API (via HTTP request) to extract structured invoice data, parses the JSON response, and finally appends or updates the extracted data in a Google Sheet with fields like vendor name, amount, currency, and line items.

## Output Details
The extracted and structured receipt/invoice data is saved into a Google Sheet, including details like file ID, filename, sender information, total amount, and line item descriptions.

## Tags
OCR, Google Drive, Google Sheets, automation, invoice processing, receipt extraction, n8n, production-ready
