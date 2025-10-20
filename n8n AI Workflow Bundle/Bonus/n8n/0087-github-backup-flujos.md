# Workflow Analysis for Monitor Active n8n Workflows and Backup to GitHub

## Description
This workflow automates the process of monitoring active n8n workflows, retrieving their data, and backing them up to a specified GitHub repository.

## Input Details
The workflow is manually triggered or initiated by a cron job set to run at a specific interval.

## Process Summary
First, the workflow fetches all active workflows from n8n. Then it iterates through each active workflow. For every workflow, it constructs a filename using the workflow ID and name and retrieves the workflow definition. Finally, it uploads the workflow definition as a JSON file to a specified GitHub repository, creating or updating the file as needed.

## Output Details
The workflow creates or updates JSON files in a GitHub repository, each containing the definition of an active n8n workflow.
