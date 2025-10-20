# Workflow Analysis for Automate Google Calendar Events for New ActiveCampaign Deals

## Description
This workflow automates the creation of Google Calendar events whenever a new deal is added or updated in ActiveCampaign. It ensures that meetings and appointments related to sales opportunities are automatically scheduled and accessible.

## Input Details
The workflow is triggered by a webhook from ActiveCampaign when a new deal is added or updated.

## Process Summary
First, the workflow receives deal data from ActiveCampaign via a webhook. Then, it creates a new event in Google Calendar using pertinent deal information such as title, start and end dates, and description. Next, it updates the ActiveCampaign deal with a custom field indicating that a calendar event has been created. Finally, it sends a Slack notification to a specified channel, confirming the successful creation of the calendar event.

## Output Details
The workflow creates a Google Calendar event, updates an ActiveCampaign deal, and sends a Slack notification.
