# Workflow Analysis for n8n Workflow Backup to GitLab

## Description
This workflow automatically backs up selected n8n workflows to a GitLab repository. It can be triggered manually or on a schedule, and only saves workflows that have changed since the last backup.

## Input Details
The workflow is triggered either manually via a Manual Trigger node or automatically via a Schedule Trigger set to run weekly at 9:30 PM on Saturdays.

## Process Summary
The workflow begins by setting global configuration values such as GitLab owner, project, and tags to identify which n8n workflows should be backed up. It fetches all n8n workflows tagged with 'gitlab_backup_enabled' and derives a safe filename from each workflow's name. It then checks if a file with that name already exists in the GitLab repository. If the file exists and its content differs from the current workflow, it updates the file; if it doesn’t exist, it creates a new file. Unchanged workflows are skipped to avoid unnecessary commits.

## Output Details
The workflow outputs updated or newly created JSON files in a specified GitLab repository, with each file representing a backed-up n8n workflow, and commits are annotated with execution type (manual or scheduled) and timestamp.

## Tags
n8n, gitlab, backup, automation, workflow-management, scheduled-task, manual-trigger, version-control
