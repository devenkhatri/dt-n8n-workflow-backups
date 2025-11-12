# Workflow Analysis for Errortrigger Workflow

## Description
This workflow automatically sends an email notification via Mailgun whenever an error occurs in any other workflow that is configured to use it as an error handler.

## Input Details
The workflow is triggered automatically by an error occurring in another workflow, receiving details such as the error message, stack trace, and the name of the failed workflow.

## Process Summary
The workflow starts with an Error Trigger node that captures error data from a failed workflow execution. It then uses a Mailgun node to compose and send an email containing the error message and stack trace. The email subject includes the name of the workflow where the error occurred. The 'To' and 'From' email addresses are expected to be configured in the node settings. Finally, a Stop and Error node halts the workflow with a generic error message.

## Output Details
The workflow sends an error notification email via Mailgun and then stops execution.

## Tags
error handling, email notification, Mailgun, automation, n8n, production-ready
