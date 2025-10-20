# Workflow Analysis for Slack to Linear Ticket Creation

## Description
This workflow automates the creation of Linear tickets from Slack messages, allowing teams to quickly convert discussions or issues into structured tasks.

## Input Details
The workflow is triggered by an HTTP POST request, typically from a Slack message event.

## Process Summary
The workflow receives data from Slack via an HTTP webhook, then extracts the user, channel, and message text. It then constructs a title and description for a new Linear issue, including a link back to the original Slack message. Finally, it creates a new issue in Linear with the prepared title and description.

## Output Details
The workflow creates a new issue in Linear with details extracted from the Slack message.
