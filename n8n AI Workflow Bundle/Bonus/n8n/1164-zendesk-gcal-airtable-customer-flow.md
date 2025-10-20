# Workflow Analysis for Zendesk to Google Calendar and Airtable Customer Flow

## Description
This workflow automates the process of managing customer appointments. It starts by integrating with Zendesk to create tickets, then schedules events on Google Calendar for customer support, and finally updates customer records in Airtable.

## Input Details
This workflow is triggered when a new ticket is created in Zendesk.

## Process Summary
First, it retrieves the new ticket data from Zendesk. Then, it creates a new event in Google Calendar with the customer details and ticket link. Next, it updates the corresponding customer record in Airtable with the event information. Finally, if the customer does not exist in Airtable, it creates a new record.

## Output Details
The workflow creates a Google Calendar event and updates or creates a customer record in Airtable.
