# Workflow Analysis for Notion and Linear.app Issue Synchronisation

## Description
This workflow synchronises issues between Notion and Linear.app, enabling seamless project management across both platforms.

## Input Details
This workflow is triggered manually to start the synchronization process.

## Process Summary
The workflow starts by retrieving all issues from a specified Notion database. It then iterates through each Notion issue, checking if a corresponding issue exists in Linear.app using the Notion page ID. If a Linear.app issue is found, it updates the issue with information from Notion; otherwise, it creates a new issue in Linear.app based on the Notion data. Conversely, the workflow also fetches issues from Linear.app and updates or creates corresponding entries in Notion based on whether a Notion page ID already exists for the Linear.app issue.

## Output Details
The workflow updates existing issues or creates new issues in both Notion and Linear.app to maintain synchronization.
