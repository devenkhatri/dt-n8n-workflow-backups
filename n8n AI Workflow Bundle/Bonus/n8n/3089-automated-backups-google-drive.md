# Workflow Analysis for Automated n8n Workflow Backups to Google Drive

## Description
This workflow automates the backup of n8n workflows by exporting them as JSON files and uploading them to a designated folder in Google Drive.

## Input Details
This workflow is triggered every day at 1:00 AM by a Cron job.

## Process Summary
First, the workflow retrieves all active n8n workflows. Then, it iterates through each workflow and exports it as a JSON file. These JSON files are then combined into a single file and uploaded to a specified folder in Google Drive. If the folder does not exist, it creates a new one.

## Output Details
The workflow creates JSON files of n8n workflows and uploads them to a specified folder in Google Drive.
