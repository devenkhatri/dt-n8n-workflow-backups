# Workflow Analysis for Backup all n8n Workflows To Github

## Description
This workflow backs up all n8n instance workflows to a specified GitHub repository daily or on manual trigger. Workflow files are organized into YYYY/MM/ folders and named by their ID. The repository owner, name, and main folder are configurable. The workflow efficiently processes each workflow, comparing it to the existing version in GitHub and either creating a new file, updating an existing one, or doing nothing if no changes are detected. After all workflows are processed, a completion notification is sent to Slack.

## Input Details
This workflow is triggered either manually or on a daily schedule, and it retrieves all existing n8n workflows from the instance.

## Process Summary
The workflow begins by fetching all n8n workflows and then processes them one by one. For each workflow, it sets up GitHub repository configuration and calculates a sub-path based on the workflow's creation date. It attempts to get the existing workflow file from GitHub, handling cases where the file might be large or non-existent. A custom code block compares the current n8n workflow with its GitHub counterpart, determining if it is "same," "different," or "new." Based on this status, the workflow either skips, updates an existing file, or creates a new file in the GitHub repository. Finally, a completion message is sent to Slack.

## Output Details
The workflow saves or updates n8n workflow JSON files in a designated GitHub repository and sends a completion notification to a Slack channel.
