# Workflow Analysis for Save_your_workflows_into_a_GitHub_repository

## Description
This workflow automatically backs up all your n8n workflows to a specified GitHub repository, checking for changes and either creating new files or updating existing ones as needed.

## Input Details
The workflow is triggered either manually or on a schedule, and it fetches all workflows from the n8n instance via the n8n API.

## Process Summary
The workflow first retrieves all n8n workflows and filters those updated in the last 7 days. It then loops through each workflow, checking if a corresponding file already exists in the specified GitHub repository. If the file exists, it compares the content; if different, it updates the file, otherwise skips it. If the file doesn’t exist, it creates a new one. All files are saved as JSON with ordered keys for consistent diffs. The workflow also handles large files by downloading them via HTTP if needed.

## Output Details
The workflow saves or updates JSON files in a GitHub repository and optionally sends Slack notifications when the backup process starts and completes.

## Tags
github, backup, workflow, automation, n8n, slack, json, version-control
