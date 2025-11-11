# Workflow Analysis for Backup n8n Credentials to GitHub

## Description
This workflow automatically exports all decrypted n8n credentials and backs them up to a specified GitHub repository. It compares existing files in GitHub to avoid unnecessary updates, only creating or updating files when credentials are new or have changed.

## Input Details
The workflow is triggered either manually or on a schedule (every 2 hours) and receives no external input data—it fetches credentials directly from the n8n instance.

## Process Summary
The workflow starts by exporting all decrypted credentials from the n8n instance using a CLI command. It parses and formats the JSON output, then processes each credential individually via a subworkflow. For each credential, it checks if a corresponding file already exists in the configured GitHub repository. If the file exists, it compares the content; if different, it updates the file, and if the file doesn't exist, it creates a new one. If the content is identical, no action is taken.

## Output Details
The workflow creates or updates JSON files in a GitHub repository, where each file represents a credential from the n8n instance, named by its ID.

## Tags
n8n, credentials, backup, github, automation, security, workflow, json, scheduled
