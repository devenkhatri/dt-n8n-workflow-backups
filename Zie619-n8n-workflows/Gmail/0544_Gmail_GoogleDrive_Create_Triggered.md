# Workflow Analysis for Gmailtrigger Workflow

## Description
This workflow automatically monitors a Gmail inbox for new emails with attachments, extracts those attachments, and uploads them to Google Drive with a renamed format that includes the sender's email address.

## Input Details
The workflow is triggered by new emails in a Gmail inbox that contain attachments, polled every minute.

## Process Summary
The workflow starts by polling Gmail for new emails with attachments. When such an email is found, it downloads the attachments as binary data. A function node then processes each attachment, preserving its filename and binary content. The workflow then uploads each file to the root folder of Google Drive, renaming it to include the sender's email address. Error handling is included to manage any failures during execution.

## Output Details
The workflow uploads renamed email attachments to the root folder of Google Drive, with filenames that include the sender's email address.

## Tags
gmail, google drive, file upload, email automation, attachment processing, n8n
