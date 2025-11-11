# Workflow Analysis for n8n Workflow Backup to GitHub

## Description
This workflow automatically backs up all n8n workflows to a specified GitHub repository, comparing the current version with the one in GitHub and either creating a new file or updating an existing one if changes are detected.

## Input Details
The workflow is triggered either manually via a 'Manual Trigger' node or automatically every 2 hours via a 'Schedule Trigger', and it receives no external input data beyond the configured global settings.

## Process Summary
The workflow starts by fetching all workflows from the n8n instance using the n8n API. It then loops through each workflow and checks if a corresponding JSON file already exists in the specified GitHub repository by attempting to retrieve it. If the file exists, it compares the decoded content with the current workflow data; if they differ, it updates the file in GitHub. If the file doesn't exist, it creates a new one. The comparison is done after sorting JSON keys to ensure consistent ordering.

## Output Details
The workflow produces updated or newly created workflow JSON files in a GitHub repository, with commit messages indicating the workflow name and whether it was new or modified.

## Tags
n8n, github, backup, automation, workflow-sync, json, version-control, scheduled-task
