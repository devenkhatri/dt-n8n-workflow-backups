# Workflow Analysis for Zendesk to Asana Task Creation

## Description
This workflow automatically creates tasks in Asana based on new or updated tickets in Zendesk.

## Input Details
The workflow is triggered by an HTTP webhook that receives data from Zendesk whenever a ticket is created or updated.

## Process Summary
The workflow starts by receiving ticket data from Zendesk. It then checks if the ticket assignee is present; if not, it sets the assignee to "Unassigned" and adds a note. Next, it retrieves a custom field in Zendesk (if applicable) and structures the ticket details. Finally, it creates a new task in Asana using the processed Zendesk ticket information, including a link back to the original Zendesk ticket.

## Output Details
The workflow creates a new task in Asana with details from the Zendesk ticket, including a direct link to the ticket.
