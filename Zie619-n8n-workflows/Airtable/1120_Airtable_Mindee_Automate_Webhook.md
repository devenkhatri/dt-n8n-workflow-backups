# Workflow Analysis for Production Workflow

## Description
This workflow automatically processes receipt images submitted via a secure webhook, extracts key expense details using AI, stores the data in Airtable, and generates a human-readable summary of the expense.

## Input Details
The workflow is triggered by a POST request to a secure webhook that includes a receipt image as binary data.

## Process Summary
The workflow starts by receiving a receipt image via a webhook with header-based authentication. It then sends the image to Mindee's receipt parsing API to extract structured data like merchant, date, total, and category. The extracted fields are appended as a new record to a specified Airtable 'Receipt' table. Finally, a Set node formats a readable expense summary message using the stored data. An error handler is in place to catch and report any failures during execution.

## Output Details
The workflow stores the parsed receipt data in Airtable and returns a formatted expense summary message as the final output.

## Tags
receipt processing, expense tracking, OCR, airtable, webhook, mindee, automation, production-ready
