# Workflow Analysis for Automated n8n Workflow Backup to GitHub

## Description
This workflow automates the process of backing up all your n8n workflows to a specified GitHub repository, ensuring your workflow definitions are version-controlled and recoverable.

## Input Details
The workflow is triggered manually and does not receive any external input data.

## Process Summary
First, the workflow retrieves a list of all active n8n workflows. For each workflow, it then fetches its detailed JSON definition. The workflow then iterates through each workflow definition and dynamically creates a file path in a GitHub repository. Finally, it commits each workflow definition as a separate JSON file to the specified GitHub repository.

## Output Details
The workflow saves n8n workflow definitions as individual JSON files to a designated GitHub repository.
