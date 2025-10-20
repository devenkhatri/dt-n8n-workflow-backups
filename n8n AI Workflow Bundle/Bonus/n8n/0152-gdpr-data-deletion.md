# Workflow Analysis for GDPR Data Deletion Workflow

## Description
This workflow automates the process of deleting user data from various services in compliance with GDPR regulations when a deletion request is received via a webhook.

## Input Details
The workflow is triggered by an HTTP webhook that receives a deletion request containing user information (email or user ID).

## Process Summary
First, the workflow extracts the user ID and email from the incoming webhook data. Then, it attempts to delete the user from Stripe using the provided email or ID. Subsequently, it searches for and deletes the user from Intercom and Slack workspaces. Finally, it sends a confirmation email to the individual who initiated the deletion request, along with a summary of the deletion actions.

## Output Details
The workflow sends a confirmation email detailing the deletion actions taken across Stripe, Intercom, and Slack.
