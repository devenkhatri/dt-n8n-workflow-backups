# Workflow Analysis for n8n Error Report to Line

## Description
This workflow automatically sends a notification to a LINE account whenever an error occurs in any n8n workflow, providing details like the workflow name and execution URL for quick troubleshooting.

## Input Details
The workflow is triggered automatically by any error occurring in other n8n workflows that have this set as their error-handling workflow.

## Process Summary
The workflow starts with an Error Trigger node that activates when any monitored workflow fails. It then uses an HTTP Request node to send a POST request to the LINE Messaging API. The message includes the name of the failed workflow and a link to its execution details. Authentication for the API call is handled via HTTP header credentials stored in n8n. The message is sent to a specific LINE user whose UID must be configured in the request body.

## Output Details
The workflow sends a formatted error alert message to a specified LINE user via the LINE Messaging API.

## Tags
error handling, n8n, LINE notification, automation, production-ready, alerting
