# Workflow Analysis for Microsoft Outlook AI Email Assistant

## Description
Automated workflow: Microsoft Outlook AI Email Assistant. This workflow integrates 15 different services: microsoftOutlook, stickyNote, markdown, airtable, scheduleTrigger. It contains 29 nodes and follows best practices for error handling and security.

## Input Details
The workflow is triggered either manually or on a schedule (every 15 minutes) to fetch unflagged and uncategorized emails from a Microsoft Outlook inbox, and it also periodically updates a contact list from Monday.com into Airtable.

## Process Summary
The workflow is initiated either manually or via a scheduled trigger (every 15 minutes) to process incoming emails. It first updates a contact list from Monday.com into Airtable for better AI context. Then, it fetches unflagged and uncategorized emails from a specified Microsoft Outlook folder, converts their bodies to Markdown, and sanitizes them. For each email, an AI model analyzes its content, sender, and subject, using predefined rules, categories, and contact information from Airtable, to assign a primary category and an optional sub-category. Finally, the workflow updates the email in Outlook by setting its assigned category, and if the AI identifies an "Action" sub-category, it also sets the email's importance to "High."

## Output Details
The workflow categorizes and prioritizes emails within Microsoft Outlook, updating their category and importance based on AI analysis, and maintains an updated contact list in Airtable.

## Tags
automation, n8n, production-ready, excellent, optimized
