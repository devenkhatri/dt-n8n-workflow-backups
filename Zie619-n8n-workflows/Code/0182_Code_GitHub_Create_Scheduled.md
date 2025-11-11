# Workflow Analysis for Workflow Backup to GitHub

## Description
This workflow automatically backs up all n8n workflows to a GitHub repository on a daily schedule or manual trigger. It compares each workflow with its existing backup file (if any) and either creates a new file or updates the existing one if changes are detected, organizing backups in year/month folders.

## Input Details
The workflow is triggered either manually via the 'On clicking execute' node or automatically via a scheduled trigger (daily at 1:33 AM UTC). It receives no external input data but fetches all workflows from the current n8n instance.

## Process Summary
The workflow starts by fetching all workflows from the n8n instance and looping through them in batches. For each workflow, it tries to retrieve the corresponding backup file from GitHub using a path based on the workflow's creation date (YYYY/MM/). It then compares the current workflow JSON with the existing backup (if any), normalizing key order for accurate comparison. Based on whether the file is new, unchanged ('same'), or modified ('different'), it either creates a new file, updates the existing one, or skips the file. Notifications are sent to Slack at the start, completion, and for any failures.

## Output Details
The workflow outputs backup files to a GitHub repository in a structured folder format (YYYY/MM/ID.json) and sends status notifications to a Slack channel.

## Tags
backup, github, n8n, automation, slack, workflow-management, scheduled-task, json
