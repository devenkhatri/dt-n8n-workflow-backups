# Workflow Analysis for HubSpot to Zendesk Contact and Company Sync

## Description
This workflow synchronizes contact and company information between HubSpot and Zendesk, ensuring that customer data is consistent across both platforms. When a new contact is created in HubSpot, the workflow checks if a corresponding user or organization exists in Zendesk. Based on the presence of matching records, it either creates new entries or updates existing ones in Zendesk.

## Input Details
The workflow is triggered by new contact creations in HubSpot via a webhook.

## Process Summary
Upon a new contact creation in HubSpot, the workflow first checks for a matching user in Zendesk using the contact's email. If no user is found, it attempts to find a matching organization in Zendesk using the company name. Subsequently, it creates or updates the user and organization records in Zendesk based on the findings, linking them appropriately. Finally, it creates an activity in HubSpot to log the synchronization event.

## Output Details
The workflow creates or updates user and organization records in Zendesk and logs an activity in HubSpot.
