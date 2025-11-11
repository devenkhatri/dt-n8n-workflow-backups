# Workflow Analysis for Backup all n8n Workflows To Github

## Description
This workflow automatically backs up all n8n workflows to a specified GitHub repository, organizing them by creation date and updating or creating files as needed.

## Input Details
The workflow is triggered either manually via a button click or automatically on a schedule (daily at 1:33 AM).

## Process Summary
The workflow fetches all n8n workflows and processes them in batches. For each workflow, it checks whether a corresponding file already exists in the GitHub repository. It compares the current workflow content with the existing file (if any) after normalizing JSON key order. Based on the comparison, it either creates a new file, updates an existing one with changes, or skips if unchanged. Files are stored in a folder structure organized by year and month of creation (YYYY/MM/).

## Output Details
The workflow commits updated or new workflow files to a GitHub repository and sends start and completion notifications to a Slack channel.

## Tags
Github, n8n, backup, automation, file-sync, Slack
