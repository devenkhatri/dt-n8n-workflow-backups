# Workflow Analysis for Public Webhook Relay

## Description
This workflow acts as a relay that receives public webhook requests via webhook.site and forwards them to a local n8n workflow endpoint. It periodically polls for new POST requests, filters out already-processed ones, and forwards only the new ones to your internal system.

## Input Details
The workflow is triggered on a schedule (every 10 seconds) and receives no direct user input; instead, it polls an external webhook service (webhook.site) for new incoming HTTP POST requests.

## Process Summary
The workflow starts by checking for a stored authentication token. If none exists, it requests a new one from webhook.site. It then retrieves the timestamp of the last processed request. Using these, it fetches all recent webhook requests and filters for only new POST requests. These unprocessed requests are then forwarded to a local n8n webhook URL specified in the workflow. Finally, it updates the last processed timestamp for the next cycle.

## Output Details
The workflow sends new webhook requests as POST requests to a local n8n endpoint and stores the latest processed timestamp and auth token for future use.

## Tags
webhook, relay, automation, polling, n8n, integration, public webhook, local workflow
