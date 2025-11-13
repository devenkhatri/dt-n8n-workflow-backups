# Workflow Analysis for Hubspot Workflow

## Description
This workflow automates the synchronization of contact data between Pipedrive and Hubspot, specifically identifying and adding/updating contacts from Pipedrive into Hubspot.

## Input Details
The workflow is triggered automatically every minute by a scheduled cron job.

## Process Summary
1. The workflow starts by retrieving all contacts from Hubspot.
2. Concurrently, it fetches all person records from Pipedrive.
3. It then compares the fetched data to identify persons from Pipedrive who are not present in Hubspot based on their email addresses.
4. Finally, for each identified person, it creates or updates a contact in Hubspot, mapping the Pipedrive email to the Hubspot email and the Pipedrive first name to the Hubspot first name.

## Output Details
The workflow updates or creates new contact records in HubSpot.

## Tags
automation,n8n,production-ready,excellent,optimized
