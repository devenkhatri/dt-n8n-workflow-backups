# Workflow Analysis for Automate Jira Long-Lived Issue Resolution with AI

## Description
This n8n workflow helps customer support teams by automatically identifying and resolving long-lived or forgotten Jira issues. It uses AI to classify issue states, attempts to find solutions from a knowledge base, and manages communication by sending reminders or closing tickets based on the resolution status and customer satisfaction.

## Input Details
The workflow is triggered on a schedule and retrieves a list of unresolved Jira issues that have been open for more than 7 days.

## Process Summary
The workflow is scheduled to run periodically, finding Jira issues that are unresolved for over seven days. Each identified issue is processed in a sub-workflow, where its metadata and all comments are retrieved and formatted for AI analysis. An AI model then classifies the issue's current state. Based on this classification, the workflow either performs sentiment analysis and closes the ticket (potentially requesting feedback or escalating to Slack), attempts to resolve the issue using a knowledge base and closes it, or sends an AI-generated reminder if more information is pending.

## Output Details
The workflow updates Jira issues by adding comments (feedback requests, auto-close messages, solutions, or reminders) and changing their status to "Done," and it sends notifications to a Slack channel for unhappy resolutions or when a solution cannot be found.
