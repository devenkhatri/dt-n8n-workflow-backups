# Workflow Analysis for Send Specific PDF Attachments from Gmail to Google Drive Using OpenAI

## Description
This workflow automatically processes emails received in Gmail, scans any PDF attachments using OpenAI to determine if they match a specified document type (like 'payslip'), and uploads matching PDFs to a designated Google Drive folder.

## Input Details
The workflow is triggered when a new email with attachments is received in a Gmail inbox.

## Process Summary
The workflow starts by checking if the incoming email has attachments. It then iterates over each attachment and filters for PDF files. For each PDF, it extracts the text content and checks if the size is within OpenAI token limits. The extracted text and filename are sent to OpenAI with a prompt asking whether the document matches a configurable term (e.g., 'payslip'). If OpenAI responds with 'true', the original PDF file is uploaded to a specified Google Drive folder.

## Output Details
Matching PDF attachments are uploaded to a designated Google Drive folder based on OpenAI's classification.

## Tags
Gmail, Google Drive, OpenAI, PDF processing, document classification, automation, n8n
