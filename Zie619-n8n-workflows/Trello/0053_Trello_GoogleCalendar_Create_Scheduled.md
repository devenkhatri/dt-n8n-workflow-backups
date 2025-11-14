# Workflow Analysis for Function Workflow

## Description
Automated workflow: Function Workflow. This workflow processes data and performs automated tasks.

## Input Details
This workflow is triggered daily at 8 AM by a cron job.

## Process Summary
The workflow starts by getting the beginning and end of the current day. It then retrieves all Google Calendar events for that day and processes them individually. Next, it filters out specific recurring tasks like "Check email and start day" or "Lunch". For the remaining events, it extracts details such as summary, description, and due date. Finally, it creates a Trello card for each of these non-recurring events.

## Output Details
The workflow creates Trello cards for relevant Google Calendar events.

## Tags
automation, n8n, production-ready, excellent, optimized
