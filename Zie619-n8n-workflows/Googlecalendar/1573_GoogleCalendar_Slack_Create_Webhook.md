# Workflow Analysis for Generate google meet links in slack

## Description
This workflow allows users to generate Google Meet links instantly from Slack by using a custom slash command (/meet). It creates a temporary Google Calendar event with a Meet link, sends the link to the Slack channel where the command was invoked, and then deletes the temporary event.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint from a Slack slash command, which includes the Slack channel ID in the request body.

## Process Summary
The workflow starts when a user types /meet in a Slack channel, triggering a webhook. It then creates a temporary 15-minute Google Calendar event with a Google Meet link. The generated Meet link is extracted and sent as a message back to the same Slack channel. Finally, the temporary calendar event is deleted to keep the calendar clean.

## Output Details
The workflow outputs a Slack message containing a Google Meet link in the channel where the /meet command was used.

## Tags
slack, google meet, calendar, automation, webhook, video conferencing, n8n
