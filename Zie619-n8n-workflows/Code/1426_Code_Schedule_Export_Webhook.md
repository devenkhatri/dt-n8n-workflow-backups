# Workflow Analysis for Backup workflows to git repository on Gitea

## Description
This workflow automatically backs up all n8n workflows to a specified Gitea Git repository. It runs on a schedule, checks whether each workflow already exists in the repository, and either creates a new file or updates the existing one only if there are changes. This ensures version control and secure backup of automation workflows.

## Input Details
The workflow is triggered on a recurring schedule (every 45 minutes) and pulls all current n8n workflows via the n8n API.

## Process Summary
The workflow starts by setting global variables like repository URL, name, and owner. It then fetches all workflows from the n8n instance. For each workflow, it checks if a corresponding file already exists in the Gitea repository. If the file doesn’t exist, it creates a new one; if it does exist, it compares the content and only updates the file if there are changes. Before committing, workflow data is converted to a formatted JSON string and encoded in base64 as required by Gitea’s API.

## Output Details
The workflow produces updated or newly created JSON files in a Gitea repository, each representing an n8n workflow, and commits them using the Gitea REST API.

## Tags
n8n, gitea, git backup, workflow backup, automation, version control, scheduled backup, production-ready
