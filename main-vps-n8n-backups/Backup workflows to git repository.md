# Workflow Analysis for Backup N8N Workflows to Git Repository

## Description
This workflow automates the process of backing up all your n8n workflows to a specified Git repository, ensuring your workflow definitions are version-controlled and easily recoverable.

## Input Details
This workflow is manually triggered to initiate the backup process.

## Process Summary
The workflow starts by retrieving all active n8n workflows. It then iterates through each workflow, converts its data to a JSON string, and saves it as a .json file within a structured folder. Finally, it commits these changes to a Git repository, creating a new commit with the updated workflow files.

## Output Details
The workflow outputs updated JSON files representing each n8n workflow to a specified Git repository.
