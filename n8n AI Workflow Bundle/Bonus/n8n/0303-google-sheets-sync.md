# Workflow Analysis for Google Sheets Sync and Email Notification

## Description
This workflow synchronizes data between two Google Sheets and sends an email notification detailing the synchronization results.

## Input Details
The workflow is manually triggered.

## Process Summary
The workflow first reads data from a source Google Sheet. Then, it clears all existing data in a destination Google Sheet. Next, it appends the data from the source sheet to the newly cleared destination sheet. Finally, it constructs an HTML email body containing the names of the source and destination sheets and the number of rows copied, and sends this email.

## Output Details
The workflow updates a Google Sheet and sends an email notification.
