# Workflow Analysis for Automated Spend and Invoice Data Extraction to Google Sheets

## Description
This workflow automates the extraction of spend and invoice details from incoming Gmail emails and organizes them into a Google Sheet for financial tracking. It processes different types of financial notifications, including multi-item credit card statements, single transaction alerts, and invoices, using AI-powered text extraction.

## Input Details
The workflow is triggered by new emails arriving in specified Gmail labels, polling every minute for new messages with attachments. It listens for emails categorized as invoices or payments.

## Process Summary
First, the workflow retrieves new emails from designated Gmail labels and extracts text from any attached PDFs. It then categorizes these emails based on the sender into types like "Multiple payment info", "One payment info", or "Invoices". Depending on the category, it either extracts structured spend details directly from the email body (for multiple payments) or prepares the email content for AI processing. AI models (Google Gemini or Groq) then extract detailed transaction information like date, service, amount, category, and currency based on predefined schemas. Finally, these extracted details are formatted and appended as new rows to a Google Sheet.

## Output Details
The workflow produces structured financial transaction records which are then appended as new rows to a Google Sheet named "raw data 2".
