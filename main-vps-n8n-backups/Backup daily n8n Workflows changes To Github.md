# Workflow Analysis for Backup daily n8n Workflows changes To Github

## Description
This workflow automatically backs up daily changes to n8n workflows by committing and pushing them to a GitHub repository.

## Input Details
The workflow is triggered on a schedule (likely daily) and accesses the local n8n workflow files to detect changes.

## Process Summary
The workflow retrieves the current n8n workflow files from the local system, checks for any changes compared to the last backup, stages the updated files, creates a new commit with a timestamped message, and pushes the changes to the designated GitHub repository. This ensures version control and safe storage of workflow configurations.

## Output Details
The workflow produces a new commit in the GitHub repository 'dt-n8n-workflow-backups' containing the latest n8n workflow changes.

## Tags
backup, github, n8n, automation, version control, workflow management
