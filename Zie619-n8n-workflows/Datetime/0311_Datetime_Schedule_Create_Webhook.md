# Workflow Analysis for Gmail to Notion Task Sync

## Description
This workflow automatically syncs Gmail emails labeled with a specific tag to a Notion database as tasks. When a task is marked complete in Notion, the corresponding Gmail label is removed.

## Input Details
The workflow is triggered on a schedule (every minute) and also listens for updates to pages in a Notion database.

## Process Summary
The workflow first runs every minute to find Gmail messages with a specific label. For each email, it checks if a corresponding page already exists in a Notion database by matching the email thread ID. If no matching page is found, it creates a new Notion page with the email subject as the title, a snippet of the body, and a link to the email. Separately, if a Notion database page is updated and marked as complete, the workflow removes the Gmail label from the associated email thread.

## Output Details
New pages are created in a Notion database for unlabeled Gmail messages, and the Gmail label is removed when tasks are completed in Notion.

## Tags
Gmail, Notion, automation, email-to-task, scheduled workflow, two-way sync
