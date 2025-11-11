# Workflow Analysis for Asana to Notion Task Sync

## Description
This workflow automatically syncs Asana task updates to a Notion database, either creating new Notion pages for unseen Asana tasks or updating existing ones based on task changes like due dates.

## Input Details
The workflow is triggered by an Asana webhook that sends task update events from a specific Asana project or workspace.

## Process Summary
When an Asana task is updated, the workflow captures the task's unique ID (gid) and fetches full task details. It then checks a Notion database for existing pages with the same Asana GID. If a match is found, it prepares an 'Update' action; otherwise, it prepares a 'Create' action. Based on this decision, it either creates a new Notion page or updates an existing one with the task name and due date. A final check ensures the due date exists before updating the deadline in Notion.

## Output Details
The workflow creates or updates pages in a specified Notion database with Asana task information such as name, GID, and due date.

## Tags
Asana, Notion, task sync, automation, webhook, database sync, project management
