# Workflow Analysis for Notion Workflow

## Description
This workflow automatically syncs GitHub issue events (like opening, editing, closing, or deleting issues) with a Notion database, keeping project tracking up to date without manual intervention.

## Input Details
The workflow is triggered by GitHub issue events (e.g., opened, edited, closed, reopened, deleted) from the 'DemoRepo' repository belonging to 'John-n8n'.

## Process Summary
When a GitHub issue event occurs, the workflow first checks if the action is 'opened'; if so, it creates a new page in a Notion database with the issue title and ID. For other actions (edited, deleted, closed, reopened), it constructs a Notion filter to find the corresponding database page using the issue ID, then routes the event through a Switch node to perform the appropriate update: editing the title, archiving (deleting), marking as closed via a checkbox, or reopening the issue in Notion.

## Output Details
The workflow creates or updates pages in a specified Notion database to reflect the current state of GitHub issues, ensuring synchronization between the two platforms.

## Tags
GitHub, Notion, issue tracking, automation, webhook, database sync, n8n
