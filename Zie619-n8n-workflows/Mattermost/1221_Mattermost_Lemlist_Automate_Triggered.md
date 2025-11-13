# Workflow Analysis for Lemlisttrigger Workflow

## Description
This workflow automates the process of notifying a team when a recipient replies to an email sent through a specific Lemlist campaign.

## Input Details
This workflow is triggered automatically when an email in a designated Lemlist campaign receives a reply.

## Process Summary
First, the workflow waits for a reply to an email from a specific Lemlist campaign. Once a reply is detected, it extracts the replier's first name, the campaign name, and the content of the reply. Finally, it formats this information into a message and sends it to a designated Mattermost channel.

## Output Details
The workflow sends a notification message containing the replier's details and their response to a specified Mattermost channel.

## Tags
automation, n8n, production-ready, excellent, optimized
