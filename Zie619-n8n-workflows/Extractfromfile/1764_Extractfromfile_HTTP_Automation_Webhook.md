# Workflow Analysis for Attachments Gmail to Drive and Google Sheets

## Description
This workflow automatically processes unread Gmail messages with PDF attachments (like invoices), saves the attachments to Google Drive with a standardized name, extracts key invoice details using AI, and logs the information in a Google Sheet for reconciliation.

## Input Details
The workflow is triggered by unread Gmail emails that contain PDF attachments, polling every minute for new messages.

## Process Summary
1. The workflow checks for unread Gmail messages with attachments. 2. It uploads the PDF attachment to Google Drive and renames it using the email subject and current date. 3. The file is moved to a specific folder in Google Drive. 4. The PDF is downloaded and its text content is extracted. 5. An AI model (GPT-4o) parses the text to extract structured invoice data (date, description, total price, and a link to the file), which is then appended to a Google Sheet.

## Output Details
The workflow saves the PDF to Google Drive, marks the Gmail message as read, and appends the extracted invoice data to a Google Sheet with a hyperlink to the stored document.

## Tags
Gmail, Google Drive, Google Sheets, PDF processing, AI data extraction, automation, invoice processing, n8n
