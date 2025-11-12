# Workflow Analysis for 📦 New Email ➔ Create Google Task

## Description
This workflow automatically creates a new task in Google Tasks whenever a new email arrives in Gmail with the label 'To-Do'. It helps users turn important emails into actionable to-do items without manual effort.

## Input Details
The workflow is triggered by new Gmail messages labeled 'To-Do', which are polled every minute.

## Process Summary
The workflow starts by polling Gmail every minute for new emails with the label 'To-Do'. When such an email is found, it extracts the subject and snippet. It then creates a new Google Task using the email subject as the task title and the snippet as task notes. The due date for the task is set to the next day. Error handling is included to manage failures during execution.

## Output Details
The workflow creates a new task in Google Tasks with the email subject as the title, snippet as notes, and a due date of the following day.

## Tags
automation, n8n, production-ready, excellent, optimized, gmail, google tasks, email to task, to-do list
