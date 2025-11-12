# Workflow Analysis for Slack Workflow

## Description
This workflow sends automated Slack notifications whenever another n8n workflow fails, providing details like the workflow name, error message, and a link to the failed execution.

## Input Details
The workflow is triggered automatically when an error occurs in another n8n workflow that has this workflow configured as its error handler.

## Process Summary
When triggered by a workflow error, the error data is passed to a 'Set message' node that formats a detailed alert message including the failed workflow name, execution URL, last executed node, and error message. This message is then sent to a predefined Slack channel named '#alerts-n8n-workflows'. After sending the message, the workflow ends with a stop-and-error node to finalize the error handling process.

## Output Details
The workflow sends a formatted error alert message to a Slack channel and then stops execution.

## Tags
error handling, slack, notifications, n8n, automation, production-ready
