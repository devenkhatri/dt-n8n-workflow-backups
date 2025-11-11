# Workflow Analysis for Create ClickUp Tasks from Slack Commands

## Description
This workflow allows users to create new tasks in ClickUp directly from Slack by using a custom slash command. When a user types a command like '/newTask Update CRM contacts', the workflow captures the message, extracts relevant details, and automatically creates a corresponding task in ClickUp with the provided text as both the title and description.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint from a Slack slash command, receiving data such as channel name, command, user name, and task text.

## Process Summary
The workflow starts by receiving a Slack slash command via a webhook. It then uses a Set node to extract and structure key fields like user name, channel, command, and task description. Next, it creates a new task in ClickUp using the provided text as both the task name and content. Finally, it sends a confirmation response back to Slack indicating the task was created successfully.

## Output Details
The workflow creates a new task in ClickUp and sends a plain-text confirmation message back to Slack via the webhook response.

## Tags
Slack, ClickUp, task automation, webhook, slash command, productivity, n8n
