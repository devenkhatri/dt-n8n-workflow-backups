# Workflow Analysis for CV Evaluation - Error Handling

## Description
This workflow automatically sends detailed error notifications via Gmail whenever another workflow (like a CV evaluation process) fails—either during execution or at the trigger stage. It includes links to the failed workflow, error details, and structured diagnostic data to help with debugging.

## Input Details
The workflow is triggered automatically by n8n’s Error Trigger node when another workflow fails, receiving structured error data including execution or trigger error details.

## Process Summary
The workflow starts with an Error Trigger that captures failure data from a parent workflow. It then sets configuration values like app URL, recipient email, and sender name. Based on whether the error occurred during execution or at the trigger level, it generates appropriate HTML content with error details. The relevant HTML is merged with configuration and workflow metadata, then used to compose and send a detailed email via Gmail.

## Output Details
The workflow sends a rich HTML email via Gmail containing error context, links to workflows, stack traces, and machine-readable JSON for debugging.

## Tags
error handling, gmail, notifications, debugging, workflow monitoring, n8n, automation, production-ready
