# Workflow Analysis for Add new incoming emails to a Google Sheets spreadsheet as a new row.

## Description
This workflow automatically captures new incoming emails and logs key details—such as sender email, subject, and message snippet—into a Google Sheets spreadsheet for record-keeping, analysis, or follow-up.

## Input Details
The workflow is triggered by new emails arriving in a Gmail inbox, polled every minute.

## Process Summary
The workflow starts by monitoring the Gmail inbox for new emails using a Gmail trigger. When a new email arrives, it extracts the sender’s email address, the subject line, and a snippet of the email body. These details are then formatted and appended as a new row in a specified Google Sheets document. The workflow includes error handling to manage potential failures during execution.

## Output Details
The extracted email data is added as a new row in a designated Google Sheets spreadsheet.

## Tags
email automation, Google Sheets, Gmail integration, data logging, n8n workflow, production-ready
