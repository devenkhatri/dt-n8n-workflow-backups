# Workflow Analysis for n8n Workflow Backup to Google Drive

## Description
This workflow automatically backs up all n8n workflows to Google Drive on a nightly schedule. It ensures organized storage by moving previous backups to an 'n8n_old' folder and optionally purges backups older than 30 days to manage space.

## Input Details
The workflow is triggered by a scheduled timer (nightly) and optionally a second schedule every 30 days for purging old backups; it also fetches current n8n workflow data via the n8n API and existing Google Drive folder structure.

## Process Summary
First, the workflow checks if required Google Drive folders ('n8n_backups' and 'n8n_old') exist and creates them if missing. It then retrieves all current workflow files from the 'n8n_backups' folder and moves them to the 'n8n_old' folder with updated names. Next, it fetches all active workflows from n8n via API, converts them to JSON files, and uploads them to the 'n8n_backups' folder. Separately, every 30 days, it scans the 'n8n_old' folder and deletes backup files older than 30 days.

## Output Details
The workflow produces up-to-date JSON backups of n8n workflows stored in Google Drive under 'n8n_backups', with aged backups archived or deleted in 'n8n_old'.

## Tags
n8n, backup, google drive, automation, workflow management, scheduled task, data retention
