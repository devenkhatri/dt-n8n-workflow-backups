# Workflow Analysis for Log errors and avoid sending too many emails

## Description
This workflow logs all system errors into a database but prevents excessive alert notifications by ensuring that alerts (like emails or push messages) are sent only if no similar error has been logged in the past 5 minutes.

## Input Details
The workflow is triggered automatically whenever an error occurs in another workflow (via n8n’s error trigger) and receives detailed error metadata including the workflow name, error message, stack trace, and execution URL.

## Process Summary
When an error occurs, the workflow first logs the full error details into a PostgreSQL table called 'N8Err'. It then queries the same table to count how many errors have been logged in the last 5 minutes. If the count is zero (meaning this is the first error in that window), the workflow proceeds to allow alert actions (though actual alerts are currently disabled in this version). Finally, it clears the execution data to prevent unintended downstream processing if used as a sub-workflow.

## Output Details
The workflow stores structured error logs in a PostgreSQL database and conditionally allows alert notifications (email, push, etc.) to be sent—though those notification nodes are currently disabled in this configuration.

## Tags
error handling, logging, alert suppression, rate limiting, PostgreSQL, n8n, production-ready, automation
