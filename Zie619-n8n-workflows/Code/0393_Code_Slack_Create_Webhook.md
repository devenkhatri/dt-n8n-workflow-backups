# Workflow Analysis for Airtable Workflow

## Description
This workflow automatically creates and schedules recurring tasks in Airtable based on predefined templates, assigns them to team members, and updates tracking records accordingly.

## Input Details
The workflow is triggered when a record enters the 'First Task - Create Task' view in an Airtable table, monitored via an Airtable trigger node.

## Process Summary
The workflow starts by capturing a triggering Airtable record that signals a new task should be created. It then retrieves related data such as the task template, assignee, and client from other Airtable tables. A code node calculates the kickoff date, soft due date, hard due date, and next task creation date based on task timing rules. Using this data, a new task record is created via an HTTP request to Airtable's API. Finally, the original automation record is updated to reflect that the first task was created and to schedule the next task creation.

## Output Details
The workflow creates a new task record in Airtable and updates the original automation record with status and scheduling information; Slack notifications are configured but currently disabled.

## Tags
Airtable, task automation, recurring tasks, workflow automation, n8n, HTTP request, date calculation, production-ready
