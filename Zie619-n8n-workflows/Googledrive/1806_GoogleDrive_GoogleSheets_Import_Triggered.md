# Workflow Analysis for Fetch the Most Recent Document from Google Drive

## Description
This workflow automatically detects when a new document is added to a specific Google Drive folder, retrieves its content, generates an AI-powered summary, and stores the summary along with the document’s owner information in a Google Sheet for easy reference and organization.

## Input Details
The workflow is triggered when a new file is created in a specified Google Drive folder, receiving file metadata including the document ID and last modifying user details.

## Process Summary
The workflow starts by monitoring a Google Drive folder for newly created files. When a new document is detected, it fetches the full content of the document using the Google Docs node. It then sends this content to an AI model (GPT-4o-mini) to generate a concise summary. Finally, the workflow appends a row to a Google Sheet containing the document owner's name, email, and the AI-generated summary.

## Output Details
The workflow outputs the document owner’s name, email, and AI-generated summary to a designated Google Sheet.

## Tags
Google Drive, Google Docs, Google Sheets, AI summarization, document automation, n8n, production-ready, file monitoring, GPT-4o-mini
