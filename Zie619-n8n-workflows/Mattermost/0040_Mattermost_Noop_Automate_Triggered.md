# Workflow Analysis for Notion Page Added to Database

## Description
This workflow automates the process of notifying the marketing team in Mattermost whenever a new meeting note page is added to a specific Notion database.

## Input Details
The workflow is triggered hourly when a new page is added to a specified Notion database, receiving the page's properties such as Team, Agenda, Date, and ID.

## Process Summary
First, the workflow activates every hour to monitor a Notion database for new page additions. If a new page is detected, it evaluates whether the 'Team' property of this page is set to 'Marketing'. If the team is 'Marketing', a notification containing the meeting agenda, date, and a direct link to the Notion page is sent to a designated Mattermost channel. If the team is not 'Marketing', the workflow proceeds without taking any further action. In case of any execution error, the workflow stops and reports a generic error.

## Output Details
The workflow sends a formatted message with meeting details to a Mattermost channel if the new Notion page belongs to the Marketing team.

## Tags
automation,n8n,notion,mattermost,marketing,notification
