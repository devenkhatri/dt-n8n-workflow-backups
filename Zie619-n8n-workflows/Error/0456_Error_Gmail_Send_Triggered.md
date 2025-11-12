# Workflow Analysis for Errortrigger Workflow

## Description
This workflow automatically sends an email notification whenever another workflow in the system fails, providing details about the error and a link to the failed execution.

## Input Details
The workflow is triggered automatically by errors occurring in other workflows that have this workflow set as their error handler.

## Process Summary
When an error occurs in a monitored workflow, this error-trigger workflow captures details such as the workflow name, execution URL, the last executed node, and the error message and stack trace. It then formats this information into an email notification. The email is sent via Gmail to a pre-configured recipient address using OAuth2 authentication.

## Output Details
The workflow sends a detailed error notification email via Gmail to the specified recipient address.

## Tags
error handling, email notification, Gmail, automation, n8n, production-ready
