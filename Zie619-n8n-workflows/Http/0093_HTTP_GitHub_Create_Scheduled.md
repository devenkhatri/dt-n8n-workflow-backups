# Workflow Analysis for Production Workflow

## Description
This workflow automatically backs up n8n workflows to a GitHub repository daily at 23:59. It fetches the list of workflows, retrieves each workflow's detailed data, and either creates a new file or updates an existing one in the repository with the latest workflow definition in JSON format.

## Input Details
The workflow is triggered daily at 23:59 by a cron scheduler and receives no external input data.

## Process Summary
The workflow starts by fetching a list of all n8n workflows via an HTTP request. It then processes this list to iterate over each workflow and fetch its detailed data. Separately, it retrieves existing workflow files from a GitHub repository. Using merge nodes, it compares existing and new workflow data to determine whether to create a new file or update an existing one in GitHub. All operations use authenticated requests and include proper error handling.

## Output Details
The workflow saves or updates JSON files representing each n8n workflow in a specified GitHub repository, with a daily commit message including the workflow name and date.

## Tags
n8n, github, backup, automation, cron, workflow management, production, json, version control
