# Workflow Analysis for Extract expenses from emails and add to Google Sheet

## Description
This workflow automatically scans incoming emails for expense-related subjects, extracts receipt data from email attachments using AI, and logs the expense details into a Google Sheet for record-keeping and analysis.

## Input Details
The workflow is manually triggered and fetches unread emails from a configured IMAP email inbox (e.g., Gmail).

## Process Summary
First, the workflow checks the inbox for new emails. It then filters emails by subject using a regular expression to match keywords like 'expenses' or 'reciept'. For matching emails, it uses Mindee AI to parse receipt data from the first attachment. The extracted data—such as date, category, currency, and total amount—is formatted along with a description derived from the email subject. Finally, this structured expense data is appended to a designated Google Sheet.

## Output Details
The workflow appends parsed expense details (date, description, category, currency, and amount) to a Google Sheet.

## Tags
expense tracking, email automation, Google Sheets, receipt parsing, Mindee, IMAP, finance automation, n8n
