# Workflow Analysis for Send specific PDF attachments from Gmail to Google Drive using OpenAI

## Description
This workflow reads PDF textual content and sends the text to OpenAI. Attachments of interest will then be uploaded to a specified Google Drive folder. For example, you may wish to send invoices received from an email to an inbox folder in Google Drive for later processing. This workflow has been designed to easily change the search term to match your needs.

## Input Details
The workflow is triggered by new emails received in Gmail and processes their attachments.

## Process Summary
The workflow is triggered upon receiving a new email, downloading any attached files. It checks for attachments and iterates through them, verifying if each is a PDF. If it is a PDF, its textual content is extracted and sent to OpenAI to determine if it matches a pre-configured search term. If OpenAI confirms a match, the original PDF attachment is then uploaded to a specified Google Drive folder.

## Output Details
The workflow uploads matching PDF attachments to a designated Google Drive folder.
