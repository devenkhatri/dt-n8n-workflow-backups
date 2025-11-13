# Workflow Analysis for Functionitem Workflow

## Description
This automated workflow processes data and performs automated tasks.

## Input Details
The workflow is triggered daily at 7 AM by a cron schedule.

## Process Summary
The workflow starts by retrieving the last execution timestamp from its internal static data. If no previous timestamp is found, it uses the current time. It then queries Mailchimp to retrieve members who have changed since this last execution timestamp. For each changed Mailchimp member, it creates or updates a corresponding contact in HubSpot using their email, first name, and last name. Finally, the workflow updates its internal static data with the current execution timestamp for future runs, and an error handler is available for execution issues.

## Output Details
The workflow updates contact information in HubSpot and stores the timestamp of its latest execution internally.

## Tags
automation, n8n, production-ready, excellent, optimized
