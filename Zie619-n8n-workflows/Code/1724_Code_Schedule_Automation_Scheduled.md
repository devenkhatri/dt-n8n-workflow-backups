# Workflow Analysis for Todoist Weekly Review Template

## Description
This workflow automatically compiles a weekly summary of completed Todoist tasks and emails it every Friday afternoon, helping users reflect on their productivity over the past week.

## Input Details
The workflow is triggered automatically every Friday at 3 PM UTC and optionally via manual testing; it fetches completed tasks from the Todoist API for the last 7 days.

## Process Summary
The workflow starts by fetching completed tasks from the Todoist API for the past 7 days. It then optionally filters out tasks from specified projects using a hardcoded list of project IDs. Next, it groups the remaining tasks by completion date and formats them into an HTML email body with headings for each day and a bulleted list of tasks. Finally, it sends the formatted summary via email with the subject 'Todoist Weekly Review'.

## Output Details
The workflow sends a formatted HTML email containing a day-wise list of completed Todoist tasks from the past week to a configured email address.

## Tags
todoist, weekly review, email automation, productivity, task tracking, n8n, automation, production-ready
