# Workflow Analysis for Manualtrigger Workflow

## Description
This workflow compares n8n workflows with their saved versions in a GitLab repository to determine if they are new, unchanged, or have differences. Based on this comparison, it either creates a new file, updates an existing one, or logs the status, ensuring workflow versions are synchronized with the repository.

## Input Details
The workflow is triggered manually and receives no external input data; it internally fetches all n8n workflows and compares them against corresponding files in a predefined GitLab repository.

## Process Summary
The workflow starts with a manual trigger and sets global GitLab repository details. It retrieves all n8n workflows and loops through each one. For each workflow, it attempts to fetch a corresponding JSON file from GitLab. If the file doesn't exist, it's marked as 'new'; if it exists, the workflow compares the current n8n version with the GitLab version (ignoring fields like 'updatedAt' and 'global'). Based on the comparison result ('new', 'same', 'diff', or 'error'), it either creates a new file, updates the existing one, or logs an error, and outputs the status for each workflow.

## Output Details
The workflow outputs a status for each n8n workflow (e.g., 'new', 'same', 'diff', or 'error') and may create or update corresponding JSON files in the specified GitLab repository.

## Tags
n8n, GitLab, workflow versioning, file synchronization, manual trigger, automation, production-ready
