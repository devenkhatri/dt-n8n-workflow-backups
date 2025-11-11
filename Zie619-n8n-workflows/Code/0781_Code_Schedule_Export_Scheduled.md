# Workflow Analysis for Set Workflow

## Description
This workflow automatically backs up all n8n workflows to Google Drive in JSON format on a daily schedule, ensuring data security and easy recovery.

## Input Details
The workflow is triggered on a daily schedule at 1:30 AM UTC and does not require external input data.

## Process Summary
The workflow starts with a scheduled trigger that runs daily at 1:30 AM. It then retrieves all n8n workflows using the n8n API. A Code node converts each workflow's JSON data into a base64-encoded binary file named 'data.json'. The Parameters node sets directory and parent drive information using environment variables. Finally, the workflow uploads the JSON file to a specified Google Drive folder, naming it based on the workflow's name.

## Output Details
The workflow produces a JSON backup file for each n8n workflow and saves it to a designated folder in Google Drive.

## Tags
automation, n8n, Google Drive, backup, scheduled workflow, data security, production-ready
