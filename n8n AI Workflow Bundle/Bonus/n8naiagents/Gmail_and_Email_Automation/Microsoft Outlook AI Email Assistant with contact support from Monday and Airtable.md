# Workflow Analysis for Microsoft Outlook AI Email Assistant

## Description
This workflow automates the categorization and prioritization of incoming Microsoft Outlook emails using an AI model. It integrates with Monday.com for contact management and Airtable for custom categorization rules, contacts, and deletion rules, ensuring efficient email processing and organization.

## Input Details
The workflow is triggered either manually or on a 15-minute schedule to fetch new, unflagged, and uncategorized emails from Microsoft Outlook, and it also has a separate scheduled trigger to update contact information from Monday.com into Airtable.

## Process Summary
The workflow fetches new emails from Microsoft Outlook that are not flagged and do not have existing categories. It converts the email body from HTML to Markdown and then sanitizes it by removing unwanted characters and formatting. Concurrently, it retrieves contact information from Monday.com and stores it in Airtable, along with custom categorization rules and categories from Airtable. An AI agent (OpenAI Chat Model) analyzes each sanitized email, along with the retrieved contacts and rules, to determine its appropriate category and sub-category. Finally, it updates the original email in Microsoft Outlook with the assigned category and, if the sub-category is "Action", sets its importance to "High".

## Output Details
The workflow categorizes and potentially prioritizes emails within Microsoft Outlook, and it maintains an updated list of contacts in Airtable.
