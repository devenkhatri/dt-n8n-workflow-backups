# Workflow Analysis for Linear Bug Ticket Auto-Classifier

## Description
This workflow automatically classifies incoming bug tickets in Linear by analyzing their title and description using AI, then assigns them to the appropriate team based on predefined responsibilities.

## Input Details
The workflow is triggered by updates to Linear issue tickets that meet specific criteria: they must be in the 'Triage' state, have a 'type/bug' label, and contain a non-placeholder description.

## Process Summary
The workflow first filters Linear issues to only process valid bug tickets that need classification. It then fetches all available Linear teams and uses OpenAI to analyze the bug's title and description against predefined team responsibilities to determine the best-fit team. If the AI identifies a valid team (not 'Other'), the workflow updates the Linear ticket with the correct team ID. If the AI cannot determine a team, it sends a notification to a configured Slack channel.

## Output Details
The workflow either updates the Linear ticket with the appropriate team assignment or sends a notification to Slack when the AI cannot determine the correct team.

## Tags
Linear, AI classification, bug triage, team assignment, OpenAI, Slack notification, workflow automation
