# Workflow Analysis for Gmail Workflow

## Description
This workflow retrieves emails with a specific label from Gmail, extracts attachments, uploads them to a designated Google Drive folder, and captures the shareable link of the uploaded file.

## Input Details
The workflow is triggered manually and does not receive external input data.

## Process Summary
The workflow starts with a manual trigger. It then fetches all Gmail messages labeled with a specific custom label. For each message with an attachment, it uploads the attachment to a predefined Google Drive folder. After uploading, it extracts and stores the web view link of the uploaded file. The workflow includes error handling to manage any failures during execution.

## Output Details
The workflow produces a shareable Google Drive link for each uploaded email attachment and makes it available as output data.

## Tags
Gmail, Google Drive, attachment handling, file upload, email automation, manual trigger, n8n, production-ready
