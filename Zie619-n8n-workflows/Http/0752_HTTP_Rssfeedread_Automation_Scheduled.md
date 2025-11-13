# Workflow Analysis for Post to Mattermost v2

## Description
This workflow periodically checks an RSS feed every 10 minutes and posts new entries to a Mattermost channel via an HTTP request. It ensures only new items are posted by tracking the last processed RSS item ID using global workflow data.

## Input Details
The workflow is triggered automatically every 10 minutes by a cron scheduler and fetches data from an RSS feed specified by the BASE_URL environment variable.

## Process Summary
The workflow starts with a cron trigger that runs every 10 minutes. It reads an RSS feed from a URL defined in the environment variables. A custom function compares each RSS item against the last posted item ID stored in global workflow data to identify new entries. Only new entries are passed forward; if none are found, a dummy 'NaN' entry is generated. An IF node filters out the dummy entries, allowing only real new items to trigger an HTTP POST request that sends the title and link to Mattermost.

## Output Details
For each new RSS item, the workflow sends a POST request to a Mattermost-compatible endpoint (configured via BASE_URL), including the item's title and link as a query parameter.

## Tags
RSS, Mattermost, automation, cron, notification, workflow, n8n
