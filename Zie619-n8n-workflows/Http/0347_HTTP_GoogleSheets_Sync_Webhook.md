# Workflow Analysis for Dialpad to Syncro

## Description
This workflow automatically creates support tickets in Syncro when an inbound phone call is received via Dialpad, using caller information to link or create customer records, and logs the call-ticket mapping in Google Sheets.

## Input Details
The workflow is triggered by a POST webhook from Dialpad containing inbound call details such as caller phone number and call ID.

## Process Summary
The workflow first checks if the call is inbound. It then queries Syncro’s API to find matching contacts or customers based on the caller’s phone number. If a single matching contact is found, it either updates an existing ticket or creates a new one. If no contact is found but a single customer matches, it creates a ticket for that customer. In all successful cases, the call ID and associated ticket ID are logged to a Google Sheet for tracking.

## Output Details
The workflow creates or updates a support ticket in Syncro and logs the mapping between the Dialpad call ID and Syncro ticket ID in a Google Sheet.

## Tags
Dialpad, Syncro, ticket creation, inbound call, customer support, Google Sheets, webhook, automation
