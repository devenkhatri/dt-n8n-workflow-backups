# Workflow Analysis for Calendly to Notion Integration with Dropcontact Enrichment

## Description
This workflow automates the process of enriching meeting invitee data from Calendly with Dropcontact and then creating a new item in a Notion database.

## Input Details
The workflow is triggered by new scheduled events in Calendly via a webhook, receiving event details such as invitee email, name, and event type.

## Process Summary
First, the workflow extracts the invitee's email address from the Calendly event data. Next, it uses Dropcontact to find and enrich contact information using the provided email. After that, it prepares the data for Notion, extracting key fields from both Calendly and Dropcontact. Finally, it creates a new item in a specified Notion database, populating it with the enriched contact and event details.

## Output Details
The workflow creates a new item in a specified Notion database, containing enriched contact information and Calendly event details.
