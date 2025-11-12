# Workflow Analysis for Functionitem Workflow

## Description
This workflow automatically syncs Zendesk support tickets with Pipedrive CRM by assigning tickets to the appropriate support agent based on the Pipedrive contact owner. It runs every 5 minutes to process newly created tickets.

## Input Details
The workflow is triggered on a schedule every 5 minutes and retrieves the timestamp of its last execution to identify new Zendesk tickets.

## Process Summary
The workflow starts by fetching the last execution timestamp and uses it to query Zendesk for tickets created since then. For each ticket, it retrieves the requester's details, searches for the requester in Pipedrive, and gets the Pipedrive contact owner's information. It then fetches a list of Zendesk agents and matches the Pipedrive owner's email to a Zendesk agent. If a match is found, the ticket is reassigned to that agent; otherwise, an internal note is added indicating the requester was not found in Pipedrive.

## Output Details
The workflow either updates the Zendesk ticket assignee to match the Pipedrive contact owner or adds an internal note if the requester is not found in Pipedrive.

## Tags
automation, zendesk, pipedrive, ticket assignment, CRM sync, scheduled workflow, n8n
