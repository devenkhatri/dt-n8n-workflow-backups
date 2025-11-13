# Workflow Analysis for Splitout Workflow

## Description
This workflow retrieves recent Stripe checkout sessions, splits the data for easier handling, and filters contacts based on specific custom fields like nickname and job title.

## Input Details
The workflow is triggered manually and receives no external input data at start.

## Process Summary
The workflow begins with a manual trigger and sends an HTTP request to the Stripe API to fetch checkout sessions created in the last 20 days, using pagination to retrieve all results. It then splits the 'data' array from the API response into individual items. Next, it splits the 'custom_fields' from each item to isolate those fields. Finally, it filters the records to keep only those where the custom field key matches either 'nickname' or 'job_title'.

## Output Details
The workflow outputs filtered records containing only the specified custom fields, ready for downstream processing or analysis.

## Tags
Stripe, checkout sessions, custom fields, data splitting, filtering, manual trigger, pagination, n8n
