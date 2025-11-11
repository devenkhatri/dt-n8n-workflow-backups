# Workflow Analysis for Autopilottrigger Workflow

## Description
This workflow automatically captures new contacts added in Autopilot and saves their first name, last name, and email address to a designated Airtable base.

## Input Details
The workflow is triggered whenever a new contact is added in Autopilot via a webhook.

## Process Summary
When a new contact is added in Autopilot, the trigger node captures the contact data. The Set node then extracts and formats the contact's first name, last name, and email. This cleaned data is then sent to Airtable where it is appended as a new record in 'Table 1'. If any step fails, the workflow routes to an error handler that stops execution and logs an error message.

## Output Details
The workflow creates a new record in the specified Airtable table with the contact’s name and email.

## Tags
automation, Autopilot, Airtable, contact sync, n8n, production-ready
