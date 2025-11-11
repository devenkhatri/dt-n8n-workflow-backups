# Workflow Analysis for Extract spend details (template)

## Description
This workflow automatically processes financial emails (invoices and payment notifications) from Gmail, extracts transaction details like date, amount, merchant, and category using AI, and logs them into a Google Sheet for expense tracking.

## Input Details
The workflow is triggered by new emails arriving in specific Gmail labels for invoices and payment notifications, with optional PDF attachments.

## Process Summary
The workflow monitors two Gmail labels for financial emails, processes any PDF attachments, and routes emails based on sender type (Cathay Bank statements, other card notifications, or invoices). It extracts structured spend data using AI models (Google Gemini or Groq) with a predefined schema, then appends the parsed transaction details to a Google Sheet.

## Output Details
Parsed expense records containing date, amount, service, category, currency, and other details are appended to a designated Google Sheet named 'raw data 2'.

## Tags
Finance, Expense Tracking, Gmail, Google Sheets, AI Parsing, PDF Extraction, Automation
