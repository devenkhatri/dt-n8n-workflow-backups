# Workflow Analysis for Stickynote Workflow

## Description
This workflow demonstrates how to receive events from a service like Linear, filter for urgent bugs, transform the data, and send a formatted alert to a Slack channel. It’s designed as a customizable template for event-driven notifications.

## Input Details
The workflow is triggered either manually for testing or by a Linear issue event (currently disabled), and it receives issue data including title, priority, labels, and URL.

## Process Summary
The workflow starts with a manual trigger for testing, which feeds mock Linear issue data into the flow. It then filters the data to only include issues labeled as 'bug' with a priority of 3 or higher. Next, it transforms the issue title to title case and prepares a clickable message with the issue URL. Finally, it sends a formatted notification to a specified Slack channel mentioning the entire channel.

## Output Details
The workflow sends a formatted message to the '#important bugs' Slack channel notifying the team of a new urgent bug, including a link to the issue.

## Tags
automation, alerting, Linear, Slack, data transformation, filtering, n8n, template, bug tracking, notifications
