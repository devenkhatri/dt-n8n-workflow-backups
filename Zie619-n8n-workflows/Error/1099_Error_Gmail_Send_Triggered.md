# Workflow Analysis for Errortrigger Workflow

## Description
This workflow automatically sends an email notification whenever another workflow in the system fails, providing key details about the error for debugging and monitoring purposes.

## Input Details
The workflow is triggered automatically by any workflow execution failure in the system, receiving error metadata including workflow name, error message, last executed node, execution URL, and stack trace.

## Process Summary
The workflow starts with an Error Trigger node that captures failure data from any failed workflow execution. It then formats a detailed error message containing the workflow name, error description, last executed node, execution URL, and full stack trace. This message is sent via Gmail to a predefined recipient email address. Finally, the workflow stops execution with an explicit error message using the Stop and Error node.

## Output Details
The workflow sends a detailed error notification email via Gmail to a specified recipient and halts execution with an error message.

## Tags
error handling, email notification, workflow monitoring, Gmail, n8n, automation, production-ready
