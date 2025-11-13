# Workflow Analysis for Webhook Workflow

## Description
This workflow automatically creates a new record in a Grist table when a confirmed entry is received via a webhook, ensuring each entry is only processed once even if the webhook is triggered multiple times.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint containing a JSON payload with an 'id' and a 'Confirmed' boolean field.

## Process Summary
The workflow starts when a POST webhook is received. It first checks if the 'Confirmed' field in the payload is true. If confirmed, it queries the Grist destination table to see if a record with the same 'id' already exists. If no existing record is found, it creates a new row in the Grist table with the 'Source' field set to the received 'id'. The workflow ensures that already existing records are not updated or duplicated.

## Output Details
If conditions are met, the workflow creates a new row in a Grist table; otherwise, it takes no action.

## Tags
webhook, Grist, conditional logic, deduplication, automation, data sync
