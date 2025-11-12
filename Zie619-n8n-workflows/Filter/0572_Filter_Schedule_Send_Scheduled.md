# Workflow Analysis for Weekly Notion Task Summary Email

## Description
This workflow fetches tasks from a Notion database, filters and sorts them by deadline, groups them into overdue and upcoming tasks, and sends a weekly summary email with a formatted HTML report. It also sends a Pushover notification to remind the user to check their email.

## Input Details
The workflow is triggered either manually or automatically every Monday at 9 AM via a schedule trigger, and it uses configuration variables such as email address, Notion database URL, and logo path set in the 'Set Workflow vars' node.

## Process Summary
The workflow starts by fetching all pages from a specified Notion database. It filters out tasks without a deadline and sorts the remaining tasks by their deadline. Each task is then converted into an HTML snippet. Tasks are split into two groups: overdue and upcoming, based on whether the deadline has passed. These groups are combined into a single HTML email template that includes styling and links, and the final email is sent to the configured address while a Pushover notification is also dispatched.

## Output Details
The workflow sends a styled HTML email with a summary of overdue and upcoming Notion tasks to the user's email address and triggers a Pushover mobile notification.

## Tags
Notion, email, automation, task management, weekly report, Pushover, HTML template, schedule trigger, productivity
