# Workflow Analysis for Set Workflow

## Description
This workflow automatically processes new HubSpot deals by extracting key deal information, evaluating deal stage and value, and triggering appropriate actions such as sending Slack notifications, creating Google Slides presentations, logging lost deals in Airtable, or generating high/low priority support tickets based on deal criteria.

## Input Details
The workflow is triggered by a new deal creation event in HubSpot and receives the deal ID, which is then used to fetch full deal details from HubSpot.

## Process Summary
When a new deal is created in HubSpot, the workflow retrieves the full deal data and extracts key fields like name, value, stage, type, and description. It then routes the deal through a Switch node based on its stage: notifying the team in Slack if the deal is 'closedwon', creating a Google Slides presentation if it's 'presentationscheduled', or logging the deal in Airtable if it's 'closedlost'. Separately, an If node evaluates whether the deal is of type 'newbusiness', has a value over 500, and is not yet closed; if so, it creates a high-priority HubSpot ticket, otherwise a medium-priority ticket.

## Output Details
The workflow produces Slack messages, Google Slides documents, Airtable records, and HubSpot tickets depending on the deal's stage and characteristics.

## Tags
HubSpot, deal management, automation, Slack, Airtable, Google Slides, ticketing, workflow routing, n8n
