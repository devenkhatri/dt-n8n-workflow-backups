# Workflow Analysis for Slack to Linear Bug Reporter

## Description
This workflow automatically creates a bug report in Linear when a user submits a bug via a Slack slash command (/bug). It captures the bug description and user info from Slack, creates a structured issue in Linear with a template reminder for reproduction steps, and sends a confirmation message back to the user with a link to the created issue.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint from a Slack slash command (/bug), receiving the bug description, user ID, and username in the request body.

## Process Summary
The workflow starts by receiving bug details from a Slack slash command via a webhook. It then uses the Set node to define the target Linear team and label IDs. Next, it sends a GraphQL mutation to Linear's API to create a new issue with the bug title, a standardized description template, and the assigned team and label. After the issue is created, the workflow sends a confirmation message back to Slack with a link to the newly created Linear issue.

## Output Details
The workflow creates a bug issue in Linear and posts a confirmation message with the issue URL back to the Slack user who submitted the bug.

## Tags
Slack, Linear, bug tracking, webhook, automation, issue creation, slash command
