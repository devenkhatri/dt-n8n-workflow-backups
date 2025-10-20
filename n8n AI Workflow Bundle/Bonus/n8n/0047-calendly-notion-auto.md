# Workflow Analysis for Automate Calendly to Notion Integration

## Description
This workflow automates the process of adding new Calendly event invitees to a Notion database, ensuring your meeting schedule and attendee information are always organized and up-to-date in your Notion workspace.

## Input Details
This workflow is triggered by new Calendly invitee events via a webhook.

## Process Summary
First, the workflow receives data from a new Calendly invitee event. Then, it extracts the invitee's name and email, along with the event name and date. Next, it creates a new item in a specified Notion database using the extracted information. Finally, it formats the event date for consistency within Notion.

## Output Details
The workflow creates a new item in a Notion database with the invitee's name, email, event name, and event date.
