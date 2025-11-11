# Workflow Analysis for Invoice Workflow SBS

## Description
This workflow automatically processes new invoice PDFs added to a specific Google Drive folder by extracting key invoice details, logging them into a Google Sheet, and sending a notification email to the billing team.

## Input Details
The workflow is triggered when a new file is created in a specified Google Drive folder.

## Process Summary
When a new file appears in the designated Google Drive folder, the workflow downloads it, extracts text from the PDF, and uses an AI model to parse essential invoice details such as invoice number, client information, dates, and total amount. These extracted details are then appended to a Google Sheet for record-keeping. Finally, the workflow generates a notification email with the invoice summary and sends it to the internal billing team.

## Output Details
The workflow updates a Google Sheet with the extracted invoice data and sends a notification email to billing@example.com.

## Tags
invoice processing, Google Drive, Google Sheets, PDF extraction, email notification, AI extraction, automation
