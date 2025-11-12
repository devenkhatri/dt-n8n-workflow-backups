# Workflow Analysis for Linear Ticket Classification Workflow

## Description
This workflow automatically classifies incoming bug tickets in Linear by using AI to analyze the ticket's title and description, then assigns it to the appropriate internal team based on predefined responsibilities.

## Input Details
The workflow is triggered by updates to Linear issue tickets that meet specific criteria: the ticket must have a valid description, be in the 'Triage' state, and include a 'type/bug' label.

## Process Summary
When a qualifying Linear ticket is updated, the workflow retrieves all available Linear teams, then uses OpenAI to analyze the ticket's content and match it to the most appropriate team based on predefined team responsibilities. If the AI identifies a valid team (not 'Other'), the ticket's team assignment in Linear is updated. If the AI cannot confidently assign a team, a notification is sent to a specified Slack channel.

## Output Details
The workflow either updates the Linear ticket with the correct team assignment or sends a notification to Slack when the AI cannot determine the appropriate team.

## Tags
Linear, AI classification, ticket routing, OpenAI, Slack notification, bug triage, team assignment, workflow automation
