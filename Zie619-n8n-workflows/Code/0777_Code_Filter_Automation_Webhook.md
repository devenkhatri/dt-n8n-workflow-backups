# Workflow Analysis for mails2notion V2

## Description
This workflow automatically processes incoming Gmail messages by extracting actionable tasks and email metadata using AI, then creates a structured page in a Notion database linked to the sender's email alias. It also manages error handling by labeling problematic emails, notifying senders, and deactivating faulty routing configurations in Airtable.

## Input Details
The workflow is triggered by new emails arriving in the Gmail inbox, specifically those addressed to a unique alias containing a route ID in the format +routeID@example.com.

## Process Summary
The workflow first filters unprocessed emails and extracts a route ID from the recipient address. It then retrieves the corresponding route configuration from Airtable and skips processing if the route is inactive. Using OpenAI, it generates an actionable task and a detailed email summary with metadata. This content is formatted into Notion page blocks and sent via an HTTP request to the Notion API using a token from the route. If successful, the email is labeled 'Processed'; if it fails, the route is deactivated, the email is labeled 'Error', and a notification is sent to the sender.

## Output Details
The workflow creates a new page in a Notion database with structured content and metadata, labels the original email as 'Processed' or 'Error' in Gmail, deactivates faulty routes in Airtable, and sends email notifications to the sender in case of errors.

## Tags
automation, n8n, production-ready, excellent, optimized, gmail, notion, airtable, openai, email-processing, ai-summarization, error-handling
