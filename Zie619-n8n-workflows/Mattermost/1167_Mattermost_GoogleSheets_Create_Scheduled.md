# Workflow Analysis for Mattermost Workflow

## Description
This workflow automatically checks a Google Sheet for new data entries every 45 minutes and sends a notification to Mattermost if new information is found.

## Input Details
The workflow is triggered either manually or automatically every 45 minutes, and then reads data from a specified Google Sheet.

## Process Summary
The workflow initiates either by a manual trigger or on a scheduled interval of every 45 minutes. It then reads all rows from a designated Google Sheet. A custom function compares the fetched data with previously processed data, identifying only the new entries based on their unique IDs. For each new entry detected, the workflow prepares a message. Finally, it sends these messages containing the new data (ID, Name, Email) to a Mattermost channel.

## Output Details
The workflow sends a formatted message to a Mattermost channel, alerting users about new data entries found in the Google Sheet, including the ID, Name, and Email.

## Tags
automation, google sheets, mattermost, data monitoring, notifications, scheduled
