# Workflow Analysis for Example - Backup n8n to Nextcloud

## Description
This workflow automatically backs up all n8n workflows to a Nextcloud instance by fetching workflow data from the n8n API and storing each workflow as a separate JSON file in a designated Nextcloud folder.

## Input Details
The workflow is triggered either manually or automatically every 6 hours via a cron scheduler, and it uses the n8n API base URL from environment variables to fetch workflow data.

## Process Summary
The workflow starts by fetching a list of all workflows from the n8n API. It then maps over each workflow to extract individual items. For each workflow, it retrieves the full workflow data via another HTTP request. The data is processed and converted into binary format. Finally, each workflow is saved as a JSON file in a specified Nextcloud directory with a filename based on the workflow name.

## Output Details
The workflow produces individual JSON files for each n8n workflow and uploads them to a Nextcloud folder path '/n8n/Backup/lacnet1/'.

## Tags
n8n, backup, nextcloud, automation, cron, json, http request, file storage
