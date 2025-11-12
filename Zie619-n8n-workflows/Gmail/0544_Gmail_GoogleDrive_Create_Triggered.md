# Workflow Analysis for Gmailtrigger Workflow

## Description
This workflow automatically detects new emails with attachments in Gmail, extracts each attachment, and uploads it to Google Drive with a renamed file that includes the sender's email address.

## Input Details
The workflow is triggered by new Gmail messages that contain attachments, polling every minute for matching emails.

## Process Summary
The workflow starts by monitoring Gmail for new emails with attachments. When such an email arrives, it downloads the attachments. A function node then processes each attachment, creating individual items with binary data and original file names. Each file is then uploaded to the root folder of Google Drive, renamed to include the sender's email address for traceability. Errors during execution are captured and handled by a dedicated error handler node.

## Output Details
The workflow uploads renamed email attachments to the root folder of Google Drive, preserving sender information in the file name.

## Tags
gmail, google drive, file upload, email automation, attachment processing, n8n, production-ready
