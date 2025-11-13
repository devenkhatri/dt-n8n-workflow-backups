# Workflow Analysis for Replicate Line Items on New Deal in HubSpot

## Description
This workflow automatically copies line items from a won HubSpot deal to a newly created deal, eliminating manual data entry and reducing errors.

## Input Details
The workflow is triggered by a webhook from HubSpot that includes query parameters with the won deal ID and the newly created deal ID.

## Process Summary
The workflow starts by extracting the won deal ID and created deal ID from the webhook query parameters. It then retrieves the line items associated with the won deal via an HTTP request to HubSpot's API. From those line items, it extracts product SKUs and uses them to fetch corresponding product details. Finally, it creates new line items for the created deal using the product IDs and associates them with the new deal.

## Output Details
The workflow sends a success notification to a Slack channel confirming that line items were replicated between the two deals.

## Tags
HubSpot, deal automation, line items, Slack notification, webhook trigger, CRM automation
