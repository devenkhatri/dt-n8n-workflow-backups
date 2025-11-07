# Workflow Analysis for Extract Spend Details from Emails

## Description
This workflow monitors a Gmail account for incoming invoices and payment notifications, extracts transaction details using AI models, and then records these expenses into a Google Sheet for automated financial tracking.

## Input Details
The workflow is triggered by new emails arriving in a Gmail account, specifically those labeled as "invoice" or "payment", and also processes attached PDF files.

## Process Summary
The workflow first retrieves new emails with designated labels from Gmail, downloading any attachments. It then extracts text from PDF attachments and combines it with the email's body, subject, and date. A 'Switch' node categorizes these emails based on the sender to handle different formats for multi-item credit card statements, single-item credit card notifications, or general invoices. Following this, an AI model (Google Gemini or Groq) is used in conjunction with a structured output parser to accurately extract specific transaction information like date, service, amount, category, currency, and payment card from the email content.

## Output Details
The extracted and structured financial transaction data is then appended as a new row to a designated Google Sheet, specifically "raw data 2".
