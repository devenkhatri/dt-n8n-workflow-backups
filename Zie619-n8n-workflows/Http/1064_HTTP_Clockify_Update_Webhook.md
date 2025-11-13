# Workflow Analysis for Syncro Status Update Clockify

## Description
This workflow automatically updates the archive status of Clockify projects based on ticket status changes received from Syncro. When a ticket is marked as 'Resolved', the corresponding Clockify project is archived; otherwise, it is unarchived.

## Input Details
The workflow is triggered by a POST webhook from Syncro containing ticket data including status, ticket number, customer name, and ID.

## Process Summary
The workflow starts by receiving a webhook payload from Syncro. It checks if the ticket status is 'Resolved'. If not, it finds the corresponding Clockify project (using a constructed name from ticket details) with archived=true and sends a PUT request to unarchive it. If the ticket status is 'Resolved', it finds the project with archived=false and sends a PUT request to archive it. Error handling is included to manage failures during execution.

## Output Details
The workflow sends HTTP PUT requests to the Clockify API to either archive or unarchive the corresponding project based on the ticket status.

## Tags
Syncro, Clockify, ticketing, time-tracking, automation, webhook, project-management
