# Workflow Analysis for Stripe New Customer to HubSpot and Slack

## Description
This workflow automates the process of handling new customer sign-ups from Stripe. It creates or updates customer information in HubSpot CRM and sends a notification to a designated Slack channel.

## Input Details
The workflow is triggered by an HTTP webhook, typically from Stripe when a new customer is created or updated.

## Process Summary
The workflow starts by retrieving the customer details from the Stripe event. It then checks if a contact with the customer's email already exists in HubSpot. Based on this check, it either creates a new contact or updates an existing one in HubSpot. Finally, it formats a message containing key customer information and sends this message to a specified Slack channel, notifying the team about the new customer.

## Output Details
The workflow updates or creates a contact in HubSpot CRM and sends a new customer notification message to a Slack channel.
