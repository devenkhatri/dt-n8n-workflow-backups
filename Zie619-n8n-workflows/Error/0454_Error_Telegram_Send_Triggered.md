# Workflow Analysis for Errortrigger Workflow

## Description
This workflow automatically notifies a Telegram chat whenever another workflow fails, providing a clickable link to inspect the failed execution.

## Input Details
The workflow is triggered automatically when any monitored workflow encounters an error, receiving error and execution metadata.

## Process Summary
The workflow starts with an error trigger that captures details of the failed execution. It then constructs a formatted alert message containing the failed workflow's name and a link to its execution logs. Finally, it sends this message to a predefined Telegram chat using configured credentials.

## Output Details
The workflow sends an error alert message to a specified Telegram chat with a link to the failed workflow execution.

## Tags
error handling, Telegram, notifications, n8n, automation, monitoring
