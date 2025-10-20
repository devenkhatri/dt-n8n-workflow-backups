# Workflow Analysis for n8n Workflow Backup to Google Drive and Notion

## Description
This workflow automates the daily backup of all active n8n workflows, storing them as JSON files in a Google Drive folder and creating an entry in a Notion database.

## Input Details
This workflow is triggered daily at 2:00 AM by a Cron event.

## Process Summary
The workflow first retrieves a list of all active n8n workflows. It then iterates through each workflow, exporting its data, and creating a uniquely named JSON file. This JSON file is uploaded to Google Drive. Finally, an entry is created in a Notion database with details of the backed-up workflow, including a link to the Google Drive file.

## Output Details
The workflow stores JSON backup files in Google Drive and creates corresponding entries in a Notion database.
