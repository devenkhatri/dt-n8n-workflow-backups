# Workflow Analysis for Send Slack message from Webflow form submission

## Description
This workflow automatically sends form submissions from Webflow to Slack. It checks if a Slack channel matching the Webflow form name already exists; if it does, the submission is sent there. If not, it creates a new channel, notifies the #general channel, and posts the form data in the new channel.

## Input Details
The workflow is triggered by a Webflow form submission and receives the form data and form name from Webflow.

## Process Summary
The workflow starts by fetching all Slack channels and checking if any channel name matches the Webflow form name (converted to lowercase with hyphens). If a matching channel exists, the form data is formatted into a Slack message block and sent to that channel. If no match is found, a new Slack channel is created using the form name, a notification is sent to the #general channel, and the form submission is posted in the newly created channel.

## Output Details
The workflow sends formatted form submission messages to existing or newly created Slack channels and optionally notifies the #general channel when a new channel is created.

## Tags
Slack, Webflow, form automation, channel creation, messaging, n8n, production-ready
