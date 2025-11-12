# Workflow Analysis for Send Discord message from Webflow form submission

## Description
This workflow automatically sends form submissions from Webflow to Discord. It checks if a Discord channel matching the form name already exists. If it does, the submission is sent there. If not, it creates a new channel, notifies the #general channel, and posts the form data in the new channel.

## Input Details
The workflow is triggered by a form submission on a Webflow site, receiving the form data and form name via a Webflow webhook.

## Process Summary
The workflow starts with a Webflow form submission trigger. It fetches all Discord channels in a specified server and checks if a channel matching the lowercase, hyphenated form name exists. If a matching channel is found, it formats the form data into a Markdown message and sends it to that channel. If no matching channel exists, it creates a new one using the form name, sends a notification to the #general channel linking to the new channel, and then posts the form submission in the newly created channel.

## Output Details
The workflow outputs a formatted message containing the Webflow form submission data to an existing or newly created Discord channel, and optionally sends a notification to the #general Discord channel when a new channel is created.

## Tags
Webflow, Discord, form submission, automation, channel creation, messaging, n8n
