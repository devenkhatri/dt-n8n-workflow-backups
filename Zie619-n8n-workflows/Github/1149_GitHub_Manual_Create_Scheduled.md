# Workflow Analysis for Production Workflow

## Description
This workflow automatically backs up n8n workflows to a GitHub repository by comparing the current workflow definitions with existing files in GitHub and either updating or creating new files as needed.

## Input Details
The workflow is triggered either manually or on a daily schedule at 20:11 UTC, and it receives no external input data beyond the configured environment variables and hardcoded repository details.

## Process Summary
The workflow starts by fetching a list of workflows from an n8n instance via an HTTP request. It then processes this list into individual items and retrieves detailed data for each workflow. For each workflow, it checks if a corresponding JSON file already exists in a specified GitHub repository. It compares the current workflow definition with the existing file content (if any) and determines whether the workflow is 'same', 'different', or 'new'. Based on this status, it either skips the workflow, updates the existing file, or creates a new file in GitHub with the workflow definition.

## Output Details
The workflow outputs updated or newly created JSON files in a GitHub repository, with commit messages indicating the status of each workflow (same, different, or new).

## Tags
automation, n8n, github, backup, workflow-sync, production-ready
