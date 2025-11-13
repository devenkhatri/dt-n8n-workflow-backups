# Workflow Analysis for Clockify to Syncro

## Description
This workflow automatically syncs time tracking entries from Clockify to Syncro MSP, ensuring that billable time is accurately recorded in Syncro for client tickets.

## Input Details
The workflow is triggered by a POST webhook from Clockify containing time entry data, including project name, user, time interval, and description.

## Process Summary
The workflow first checks if the Clockify entry belongs to a project with 'Ticket' in its name. If so, it extracts the Syncro ticket ID from the project name, matches the Clockify user to a Syncro technician using a predefined mapping, and checks a Google Sheet for existing Syncro timer entries. If a match exists, it updates the existing timer in Syncro; otherwise, it creates a new timer. The Google Sheet is also updated to maintain a mapping between Clockify and Syncro IDs for future lookups.

## Output Details
The workflow either creates or updates a time entry in Syncro via HTTP API and logs the ID mapping in a Google Sheet for reference.

## Tags
Clockify, Syncro, time tracking, automation, Google Sheets, webhook, API integration, technician mapping
