# Workflow Analysis for Automated Work Attendance with Location Triggers

## Description
This workflow automatically logs employee check-in or check-out times in a Google Sheet based on location-triggered webhooks from a mobile device.

## Input Details
The workflow is triggered by a webhook call from an iPhone Shortcut that includes a 'direction' header indicating 'Check-In' or 'Check-Out'.

## Process Summary
The workflow first checks if a Google Sheet named 'WorkTimeTracking' already exists by searching Google Drive. If it doesn't exist, a new spreadsheet with a 'Worklog' worksheet is created. It then prepares a log entry with the current date, time, and direction (from the webhook header). Finally, it appends this log entry to the 'Worklog' sheet in the identified or newly created spreadsheet.

## Output Details
The workflow records each attendance event (check-in or check-out) as a new row in a Google Sheet, including date, time, and direction.

## Tags
attendance tracking, time tracking, location-based automation, Google Sheets, Google Drive, webhook, mobile automation, n8n
