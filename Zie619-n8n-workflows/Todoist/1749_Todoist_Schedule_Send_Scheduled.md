# Workflow Analysis for Email Mailbox as Todoist Tasks

## Description
This workflow automates the process of converting emails into Todoist tasks, using AI to summarize email content and propose actions or responses. It helps manage your inbox by ensuring important emails are tracked as actionable tasks.

## Input Details
The workflow is primarily triggered manually, but can also be configured to run on a schedule or by new emails received via IMAP. It processes unread and starred emails from a Gmail inbox.

## Process Summary
1. The workflow scans a Gmail inbox for unread and starred messages and retrieves all open tasks from a specified Todoist project. 2. It identifies emails that do not yet have a corresponding task in Todoist. 3. For each new email, an AI model summarizes its content, suggests actions, and proposes a reply. 4. A new task is then created in Todoist using the AI-generated summary, description, actions, and proposed answer. 5. Additionally, the workflow monitors starred emails and closes existing Todoist tasks if their corresponding email in Gmail is no longer starred.

## Output Details
The workflow creates new tasks in Todoist with AI-generated summaries and actions, closes existing Todoist tasks based on email unstarring, and marks processed emails as read and starred in Gmail.

## Tags
automation, n8n, Gmail, Todoist, AI, Email Management, Task Automation, Inbox Zero
