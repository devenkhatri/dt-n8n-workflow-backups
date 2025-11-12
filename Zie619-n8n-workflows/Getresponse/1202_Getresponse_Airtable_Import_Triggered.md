# Workflow Analysis for Airtable Workflow

## Description
This workflow automatically captures new email subscribers from GetResponse and saves their name and email to an Airtable database.

## Input Details
The workflow is triggered when a new contact subscribes to a specific GetResponse mailing list (list ID: qtPk7).

## Process Summary
When a new subscription occurs in GetResponse, the trigger node captures the contact's details. The Set node extracts and formats the contact's name and email from the payload. The workflow then appends this information as a new record into a specified Airtable table (Table 1). Error handling is in place to stop execution and notify on failures.

## Output Details
The workflow creates a new record in an Airtable base containing the subscriber's name and email.

## Tags
automation, n8n, production-ready, optimized, airtable, getresponse, subscriber sync
