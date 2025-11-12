# Workflow Analysis for mails2notion V2

## Description
This workflow automatically processes incoming Gmail messages, extracts key information using AI, and creates structured pages in a Notion database based on predefined routing rules stored in Airtable.

## Input Details
The workflow is triggered by new emails arriving in the Gmail inbox, specifically those that match a custom email alias format and are not already labeled as 'Processed' or 'Error'.

## Process Summary
The workflow first checks incoming Gmail messages for specific labels to avoid reprocessing. It extracts a route ID from the email's recipient address and uses it to look up an active route in an Airtable base. If the route is active, the email content is sent to two AI agents: one generates an actionable task with title, description, and optional bullet points, while the other creates a detailed summary and extracts metadata like sender, subject, and date. This structured data is then formatted into Notion page blocks and sent via HTTP request to create a new page in the user's Notion database using a route-specific API token. If any error occurs during Notion page creation, the route is deactivated in Airtable, and an error notification is sent back to the email sender.

## Output Details
The workflow creates a new page in a Notion database with parsed email content and metadata, labels the original email as 'Processed' or 'Error', and may send error notifications via email or update Airtable route status.

## Tags
gmail, notion, airtable, openai, email automation, ai parsing, workflow automation, n8n, production-ready
