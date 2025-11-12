# Workflow Analysis for Monday.com Error Logging Workflow

## Description
This workflow automatically captures and logs workflow execution errors into a Monday.com board for tracking and debugging purposes.

## Input Details
The workflow is triggered automatically whenever an error occurs in another workflow, receiving error details such as the error message, stack trace, workflow name, and execution ID.

## Process Summary
When an error occurs, the workflow captures the error data via the Error Trigger node. It then creates a new item in a specified Monday.com board with the execution ID as the item name. A Date & Time node records the current date. A Code node extracts and escapes the error stack trace. Finally, the workflow updates the newly created Monday.com item with the workflow name, error message, stack trace, and date.

## Output Details
The workflow creates and populates a new item in a Monday.com board with detailed error information for monitoring and resolution.

## Tags
error handling, monday.com, logging, automation, debugging, n8n
