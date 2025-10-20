# Workflow Analysis for Zendesk to Jira Integration

## Description
This workflow automates the creation of Jira issues from new or updated Zendesk tickets, ensuring seamless communication and task management between customer support and development teams.

## Input Details
The workflow is triggered by an HTTP POST request containing data from Zendesk, likely representing a new or updated ticket.

## Process Summary
First, the workflow extracts the Zendesk ticket ID and checks if a corresponding Jira issue already exists. If not, it retrieves additional ticket details from Zendesk, such as the subject and description. It then creates a new Jira issue using these details. Finally, it updates the original Zendesk ticket with a link to the newly created Jira issue, ensuring traceability.

## Output Details
The workflow creates a new Jira issue and updates the corresponding Zendesk ticket with a link to the Jira issue.
