# Workflow Analysis for Errortrigger Workflow

## Description
This workflow is designed to automatically capture and process data from failed workflow executions, specifically extracting any webhook payload that may have triggered the original workflow before it failed.

## Input Details
The workflow is triggered automatically whenever another workflow in the system fails (via an Error Trigger), and it receives metadata about the failed execution, including its execution ID.

## Process Summary
When triggered by a workflow error, the workflow first retrieves full execution data of the failed run using the n8n API. It then runs a custom code script to identify any webhook nodes in the original workflow and extract the payload data they received. If webhook data is found, it is captured for further use. The workflow includes a final error handler to manage any unexpected failures during this recovery process.

## Output Details
The workflow outputs the extracted webhook payload (if any) and associated metadata, which can be used for debugging, alerting, or reprocessing failed executions.

## Tags
error handling, webhook, automation, n8n, production-ready, execution recovery, debugging
