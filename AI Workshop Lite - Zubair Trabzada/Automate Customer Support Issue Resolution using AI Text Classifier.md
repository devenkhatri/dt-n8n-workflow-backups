# Workflow Analysis for Auto-Resolve Long-Lived Jira Issues with AI

## Description
This workflow automatically identifies unresolved Jira issues older than 7 days, analyzes their comment history using AI to determine their status, and either resolves them, requests feedback, sends reminders, or escalates them based on context and sentiment.

## Input Details
The workflow is triggered on a schedule (e.g., daily) and fetches a list of unresolved Jira issues created more than 7 days ago.

## Process Summary
First, the workflow retrieves long-lived unresolved Jira issues and processes each one in parallel. It gathers issue metadata and all comments, then simplifies the conversation thread for AI analysis. An AI classifier determines if the issue is resolved, pending more info, or still waiting for a team response. If resolved, sentiment analysis decides whether to request a review or escalate via Slack. If unresolved, an AI agent attempts to provide a solution using Jira and Notion knowledge bases. If the issue is just waiting on input, a reminder message is posted. Finally, issues are closed with appropriate messages.

## Output Details
The workflow posts comments to Jira issues, closes them when appropriate, and optionally sends notifications to a Slack channel for unresolved or negatively resolved issues.

## Tags
Jira, AI automation, issue management, sentiment analysis, customer support, knowledge base, Slack integration, workflow automation
