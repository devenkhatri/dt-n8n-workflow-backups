# Workflow Analysis for Linear Ticket Classification and Team Assignment

## Description
This workflow automatically classifies incoming bug tickets from Linear and assigns them to the appropriate engineering team based on the ticket's title and description, using AI. If the AI cannot determine the right team, it sends a notification to a Slack channel for manual review.

## Input Details
Triggered by updates to Linear issue tickets that meet specific criteria: the issue must have a non-placeholder description, be in the 'Triage' state, and carry a 'type/bug' label.

## Process Summary
The workflow starts when a Linear issue is updated. It first filters tickets to only process valid bug reports with sufficient details. It then retrieves a list of available Linear teams via a GraphQL API call. Using OpenAI, it analyzes the bug’s title and description against predefined team responsibilities (configured in the workflow) to determine the best-fitting team. If the AI identifies a team other than 'Other', the Linear ticket is updated with the new team assignment; otherwise, a Slack alert is sent for manual triage.

## Output Details
The workflow either updates the Linear ticket with the correct team ID or sends a Slack message notifying the team that AI could not classify the ticket.

## Tags
Linear, AI classification, team assignment, bug triage, OpenAI, Slack notification, automation, workflow routing, n8n
