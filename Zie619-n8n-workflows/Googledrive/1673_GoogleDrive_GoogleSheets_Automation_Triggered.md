# Workflow Analysis for Google Doc Summarizer to Google Sheets

## Description
This workflow automatically detects new Google Docs added to a specific Drive folder, extracts their content, generates an AI-powered summary, and saves the summary along with the document owner's name and email into a Google Sheet for easy tracking and reference.

## Input Details
The workflow is triggered when a new file is created in a specified Google Drive folder, receiving the file metadata and reference.

## Process Summary
The workflow starts by monitoring a designated Google Drive folder for newly created files. When a new document is detected, it fetches the full content of the Google Doc. This content is then sent to an AI model (GPT-4o-mini) to generate a concise summary. The workflow also captures the document’s last modifying user’s name and email from the metadata. Finally, it appends the summary and user details to a predefined Google Sheet.

## Output Details
The workflow outputs the document summary, owner name, and email to a specified Google Sheet, enabling centralized tracking and quick access to summarized content.

## Tags
Google Drive, Google Docs, Google Sheets, AI summarization, automation, n8n, production-ready, document processing, GPT
