# Workflow Analysis for Check To Do on Notion and send message on Slack

## Description
Automated workflow: Check To Do on Notion and send message on Slack. This workflow processes data and performs automated tasks.

## Input Details
The workflow is triggered daily at 8 AM by a Cron schedule.

## Process Summary
The workflow is scheduled to run every day at 8 AM. It connects to Notion to retrieve all existing to-do items from a specified block. For each retrieved to-do, it checks if the task is assigned to "Harshil" and if it has not been marked as complete. If an uncompleted task is assigned to "Harshil", the workflow initiates a direct message conversation with a specific user on Slack. Finally, it sends the details of that incomplete to-do item as a direct message to the Slack user.

## Output Details
The workflow sends a direct message on Slack to a specific user containing the details of an unchecked to-do item from Notion.

## Tags
automation, n8n, production-ready, excellent, optimized
