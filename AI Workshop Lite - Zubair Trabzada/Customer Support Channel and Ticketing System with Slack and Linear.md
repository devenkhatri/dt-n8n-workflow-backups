# Workflow Analysis for Slack to Linear Ticket Automation

## Description
This workflow automatically creates support tickets in Linear for Slack messages that are tagged with a ticket emoji (🎫) in a specified channel, using AI to generate meaningful ticket details.

## Input Details
The workflow is triggered on a schedule (every minute) and fetches recent messages from a Slack channel that include the ticket emoji.

## Process Summary
It first queries Slack for messages containing the ticket emoji in a specific channel. Then, it checks existing Linear issues to avoid duplicates by comparing message IDs. If no duplicate is found, it sends the message to OpenAI to generate a title, summary, suggested fixes, and priority. Finally, it creates a new ticket in Linear with the AI-generated content and message metadata.

## Output Details
The workflow creates a new support ticket in Linear with a generated title, summary, suggested fixes, priority, and original message metadata.

## Tags
Slack, Linear, AI, Ticketing, Automation, OpenAI, Support
