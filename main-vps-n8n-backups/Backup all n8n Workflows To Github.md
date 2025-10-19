# Workflow Analysis for Automated n8n Workflow Backup to GitHub

## Description
This workflow automates the daily backup of all n8n workflows to a specified GitHub repository, ensuring that all workflow definitions are securely stored and version-controlled.

## Input Details
The workflow is triggered manually and does not receive any external data.

## Process Summary
First, the workflow retrieves all existing n8n workflows. Then, it iterates through each active workflow, converts its JSON data into a string, and formats it as a .json file. For each workflow file, it creates a new file in a designated GitHub repository with the workflow's name and content, and if the file already exists, it updates the file. Finally, it combines the output of all file operations.

## Output Details
The workflow creates or updates JSON files representing n8n workflows in a specified GitHub repository.
