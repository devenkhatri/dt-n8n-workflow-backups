# Workflow Analysis for GitLab Project Backup to Google Drive

## Description
This workflow automates the daily backup of specified GitLab projects, compressing them into a .tar.gz file and uploading them to a designated folder in Google Drive.

## Input Details
The workflow is triggered daily at 00:00.

## Process Summary
The workflow starts by retrieving a list of GitLab projects based on specified IDs. For each project, it generates an archive, compresses it into a .tar.gz file, and saves it locally. Finally, it uploads the compressed backup file to a specific folder in Google Drive and then deletes the local file.

## Output Details
The workflow uploads a compressed (.tar.gz) backup of the specified GitLab projects to Google Drive.
