# Workflow Analysis for Email to Notion Save

## Description
This workflow captures incoming emails, extracts their content and attachments, and then saves this information into a specified Notion database.

## Input Details
The workflow is triggered by an incoming email received via a custom webhook address.

## Process Summary
The workflow starts by receiving an email via a webhook. It then extracts the email content and any attachments. Next, it determines if custom properties (like "Project" and "Tags") are set in the email subject. Finally, it creates a new page in a specified Notion database, populating it with the email subject, sender, body, a link to view the original email, and any extracted attachments. It automatically categorizes the Notion page based on detected properties.

## Output Details
The workflow creates a new page in a specified Notion database containing email details and attachments.
