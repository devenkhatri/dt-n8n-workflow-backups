# Workflow Analysis for Send Specific PDF Attachments from Gmail to Google Drive Using OpenAI

## Description
This workflow automatically processes incoming Gmail messages, extracts PDF attachments, and uses OpenAI to determine if each PDF matches a specified document type (like 'payslip' or 'invoice'). Matching PDFs are then uploaded to a designated Google Drive folder for further use.

## Input Details
The workflow is triggered when a new email with attachments is received in a Gmail inbox.

## Process Summary
1. The workflow starts when a new email arrives and checks if it has attachments. 2. It iterates over each attachment and filters only PDF files. 3. Each PDF is converted to text, and a check ensures the text length is within OpenAI token limits. 4. OpenAI analyzes the PDF content and filename to determine if it matches a user-defined term (e.g., 'payslip'), responding with 'true' or 'false'. 5. If OpenAI returns 'true', the original PDF is uploaded to a specified Google Drive folder.

## Output Details
PDF attachments identified as matching the specified document type are uploaded to a designated Google Drive folder.

## Tags
Gmail, Google Drive, OpenAI, PDF processing, document classification, automation, n8n, email automation, AI filtering, file upload
