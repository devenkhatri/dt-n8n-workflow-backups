# Workflow Analysis for n8n workflow deployer

## Description
This workflow automates the deployment of n8n workflows by importing JSON files from a Google Drive 'ToDeploy' folder into an n8n instance, assigning a predefined tag, and moving the file to a 'Deployed' folder upon success.

## Input Details
The workflow is triggered when a new JSON file is added to a specified Google Drive 'ToDeploy' folder.

## Process Summary
The workflow starts by monitoring a Google Drive folder for new JSON files. When a file is detected, it downloads the file, extracts and cleans the workflow JSON to include only valid fields, then sends it to the n8n API to create a new workflow. After successful creation, it assigns a predefined tag to the workflow and moves the JSON file to a 'Deployed' folder in Google Drive. If workflow creation fails, it captures the workflow name and error message for debugging.

## Output Details
The workflow creates a new n8n workflow, tags it, and moves the processed JSON file to a 'Deployed' folder in Google Drive.

## Tags
n8n, automation, workflow deployment, Google Drive, API integration, production-ready
