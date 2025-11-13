# Workflow Analysis for Httprequest Workflow

## Description
This workflow interacts with a Systeme.io-compatible API to fetch contacts and tags, filter contacts by specific tags, and add new contacts in bulk. It includes built-in pagination and rate-limit handling to ensure reliable data synchronization without exceeding API limits.

## Input Details
The workflow is manually triggered and does not receive external input data—it operates based on predefined configurations and environment variables such as API credentials and base URL.

## Process Summary
The workflow starts with a manual trigger and concurrently fetches all contacts and all tags from the API using paginated requests. It then fetches contacts that have a specific tag (ID: 1012751), supporting multi-tag filtering if needed. Separately, it can add new contacts in batches of 9 via POST requests, including custom fields like 'utm_source'. Each HTTP request includes pagination logic and error handling to manage API rate limits and ensure complete data retrieval or submission.

## Output Details
The workflow outputs retrieved contact and tag data as individual items after splitting paginated responses, and successfully added contacts are confirmed via API responses—no external storage or notification is configured in this workflow.

## Tags
Systeme.io, contacts, tags, API integration, pagination, bulk import, HTTP request, manual trigger, rate limiting, data sync
