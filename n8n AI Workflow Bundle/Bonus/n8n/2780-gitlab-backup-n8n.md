# Workflow Analysis for Automated GitLab Project Backup to Google Drive

## Description
This workflow automates the daily backup of specified GitLab projects to a designated folder in Google Drive, ensuring that your code repositories are securely stored off-site.

## Input Details
The workflow is triggered daily at 2:00 AM by a CRON schedule.

## Process Summary
First, the workflow identifies all active GitLab projects. Then, for each project, it generates a backup archive. The workflow then uploads each generated project backup file to a specific folder within Google Drive. Additionally, it removes older backup files from Google Drive to maintain storage efficiency.

## Output Details
The workflow uploads GitLab project backup archives to a Google Drive folder and manages their retention.
