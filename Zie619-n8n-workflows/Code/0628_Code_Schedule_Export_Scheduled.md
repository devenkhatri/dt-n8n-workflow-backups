# Workflow Analysis for Backup workflows to git repository

## Description
This workflow automatically backs up all n8n workflows to a GitHub repository by checking if each workflow file already exists. If it doesn't exist, it creates a new file; if it does exist, it updates the file only if there are changes. The process runs on a scheduled interval to ensure continuous backup.

## Input Details
The workflow is triggered on a schedule (every minute) and fetches all existing n8n workflows via the n8n API.

## Process Summary
The workflow starts by setting global repository details like owner, repo name, and path. It then fetches all n8n workflows using the n8n API and processes them one by one using a loop. For each workflow, it checks if a corresponding file already exists in the GitHub repository. If the file doesn’t exist, it creates a new file with the workflow content. If the file exists, it decodes the existing file content, compares it with the current workflow, and updates the file only if there are differences.

## Output Details
The workflow either creates new JSON files or updates existing ones in the specified GitHub repository with the latest workflow definitions, along with descriptive commit messages.

## Tags
automation, n8n, github, backup, workflow-management, git, production-ready, scheduled-task
