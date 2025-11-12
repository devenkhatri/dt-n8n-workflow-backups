# Workflow Analysis for Todoist Task Snooze and Unsnooze Automation

## Description
This workflow automatically manages task visibility in Todoist by moving tasks with due dates from the Inbox to a 'snoozed' project, then returning them to the Inbox a few days before they're due.

## Input Details
The workflow is triggered on a schedule—once every 5 minutes and once daily at 5am—and fetches tasks from specified Todoist projects.

## Process Summary
The workflow first retrieves tasks from the Inbox and snoozed projects. It filters out subtasks and tasks without due dates. For valid tasks, it calculates an 'unsnooze date' (3 days before the due date). If the current date is past the unsnooze date, it prepares to move the task back to the Inbox; otherwise, it ensures the task remains in the snoozed project. Finally, it batches and executes the necessary task moves via the Todoist API.

## Output Details
The workflow moves tasks between Todoist projects (Inbox and snoozed) based on their due dates and unsnooze logic, using batch API requests.

## Tags
Todoist, task management, automation, snooze, scheduling, productivity, n8n
