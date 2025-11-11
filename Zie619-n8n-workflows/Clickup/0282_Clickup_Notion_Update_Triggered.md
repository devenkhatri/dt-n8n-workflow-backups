# Workflow Analysis for Notiontrigger Workflow

## Description
This workflow synchronizes task updates between Notion and ClickUp in both directions. When a Notion database page is updated, it updates the corresponding ClickUp task. Conversely, when a ClickUp task status changes, it updates the matching Notion database page.

## Input Details
The workflow is triggered either by updates to a specific Notion database page (polled every minute) or by a webhook when a ClickUp task’s status is updated.

## Process Summary
The workflow has two main branches. First, when a Notion page is updated, it extracts the ClickUp task ID, task name, status, and deadline, then updates the corresponding ClickUp task. Second, when a ClickUp task status changes, it queries the Notion database for a page matching the ClickUp task ID and updates that page’s status field to reflect the new ClickUp status. Error handling is included to manage failures during execution.

## Output Details
The workflow updates tasks in ClickUp and database pages in Notion to keep both systems synchronized based on changes in either platform.

## Tags
Notion, ClickUp, two-way sync, task management, automation, workflow synchronization, production-ready
