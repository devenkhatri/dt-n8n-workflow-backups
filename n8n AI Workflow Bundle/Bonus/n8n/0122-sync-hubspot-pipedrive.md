# Workflow Analysis for Sync HubSpot Contacts to Pipedrive

## Description
This workflow automates the synchronization of new or updated HubSpot contacts to Pipedrive, ensuring both CRM systems have the most current contact information.

## Input Details
The workflow is triggered by new or updated contact data from HubSpot.

## Process Summary
The workflow starts by listening for new or updated contacts in HubSpot. It then checks if a corresponding person already exists in Pipedrive using the contact's email address. If the person exists, the workflow updates their details in Pipedrive; otherwise, it creates a new person in Pipedrive. Finally, it creates an activity in Pipedrive to log the contact synchronization.

## Output Details
The workflow updates existing contacts or creates new contacts in Pipedrive and logs an activity for each synchronization.
