# Workflow Analysis for Automated n8n Workflow Backup and Cleanup

## Description
This workflow automatically backs up all current n8n workflows to Dropbox, moves existing backups into an 'old' folder with a timestamp, and deletes any backup files older than 30 days to keep storage organized and efficient.

## Input Details
The workflow is triggered on a schedule (e.g., daily) and does not rely on external input data.

## Process Summary
First, the workflow sets a destination folder path for backups. It retrieves all current n8n workflows via the n8n API and converts each into a JSON file. These files are uploaded to a Dropbox folder. Before uploading, any existing backups in the main folder are moved to an 'old' subfolder with a timestamped filename. The workflow then lists all files in the 'old' folder, checks their modification dates, and deletes any older than 30 days.

## Output Details
The workflow produces organized, timestamped JSON backups in Dropbox and automatically purges outdated backups, ensuring only recent versions are retained.

## Tags
backup, automation, n8n, dropbox, cleanup, scheduled, workflow management, file management, data retention
