# Workflow Analysis for Zendesk to Slack Ticket Sync

## Description
This workflow synchronizes new and updated Zendesk tickets to a designated Slack channel, ensuring your team stays informed about customer support requests in real-time.

## Input Details
The workflow is triggered by an HTTP webhook that receives data whenever a Zendesk ticket is created or updated.

## Process Summary
The workflow starts by extracting the ticket ID and status from the incoming Zendesk webhook data. It then checks if the ticket has a non-empty subject. If a ticket subject is present, it formats a Slack message containing relevant ticket details and a link back to Zendesk. The workflow concludes by posting this formatted message to a specified Slack channel.

## Output Details
The workflow posts a formatted message containing Zendesk ticket information to a designated Slack channel.
