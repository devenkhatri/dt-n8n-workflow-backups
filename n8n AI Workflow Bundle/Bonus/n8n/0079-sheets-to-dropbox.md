# Workflow Analysis for Google Sheets to Dropbox Backup

## Description
This workflow automates the process of backing up data from a Google Sheet to a CSV file in Dropbox. It runs on a schedule, ensuring your data is regularly saved and accessible.

## Input Details
This workflow is triggered by a CRON job that runs daily at 6 AM.

## Process Summary
First, the workflow fetches all rows from a specified Google Sheet. Next, it converts the retrieved Google Sheet data into CSV format. Finally, the generated CSV file is uploaded to a designated folder in Dropbox with a dynamic filename that includes the current date.

## Output Details
The workflow creates a new CSV file containing the Google Sheet data in a specified Dropbox folder.
