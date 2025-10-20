# Workflow Analysis for Gmail Expense Receipt Processing with Mindee

## Description
This workflow automates the extraction of expense information from receipts attached to emails in Gmail using Mindee OCR and then logs the extracted data into a Google Sheet.

## Input Details
The workflow is triggered manually by clicking "Execute Workflow".

## Process Summary
The workflow first retrieves a specific email from Gmail. It then extracts the first attachment (assumed to be a receipt) from that email. This attachment is then sent to Mindee for OCR processing to extract expense details. Finally, the extracted expense data is formatted and appended as a new row to a specified Google Sheet.

## Output Details
The workflow logs extracted expense data (date, merchant, total, and currency) into a Google Sheet.
