# Workflow Analysis for Invoice Agent Workflow

## Description
This workflow automates the processing of invoices received via Telegram. It extracts key information from invoice documents, logs them into a Google Sheet database, stores the original invoice in Google Drive, and provides a summarized response back to the user on Telegram.

## Input Details
The workflow is triggered by new messages on Telegram, specifically when a document (invoice) is sent to the configured Telegram bot.

## Process Summary
Upon receiving an invoice via Telegram, the workflow first downloads the document and then uploads it to a specified Google Drive folder. Next, it sends the invoice image to an OCR service for text extraction. The extracted text is then parsed to identify key invoice details such as invoice number, date, total amount, billing address, due date, and notes. This structured data is subsequently appended as a new row to a Google Sheet designated as the invoice database. Finally, an AI agent generates a concise summary of the invoice, including a link to the database and confirms the file upload, which is then sent back to the user on Telegram.

## Output Details
The workflow outputs structured invoice data into a Google Sheet, saves the original invoice image to Google Drive, and sends a summary message back to the originating Telegram chat.
