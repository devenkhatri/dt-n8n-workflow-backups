# Workflow Analysis for Manualtrigger Workflow

## Description
This workflow automatically backs up all n8n workflows to a GitHub repository, organizing them by their first tag into subfolders. It compares the current workflow version with the one stored on GitHub and either creates a new file or updates an existing one if there are differences.

## Input Details
The workflow is triggered either manually via a 'manual trigger' node or automatically on a daily schedule at 7 AM UTC.

## Process Summary
The workflow starts by fetching all workflows from the n8n instance. It then loops through each workflow, checks if it has a tag, and sets the GitHub folder path accordingly. For each workflow, it attempts to retrieve the corresponding file from GitHub. If the file exists, it compares the content with the current workflow; if it doesn't exist, it marks the workflow as new. Based on whether the workflow is new, unchanged, or modified, it either creates a new file, updates the existing one, or does nothing. The whole process uses a self-referencing subworkflow to manage memory efficiently.

## Output Details
The workflow saves or updates JSON files in a specified GitHub repository, with each file named after the workflow ID and placed in a tag-based subfolder, and returns a confirmation that the backup process is complete.

## Tags
github, backup, workflow automation, n8n, subworkflow, file sync, json, version control
