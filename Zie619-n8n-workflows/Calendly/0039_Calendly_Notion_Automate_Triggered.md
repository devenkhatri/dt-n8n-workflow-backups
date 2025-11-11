# Workflow Analysis for Calendlytrigger Workflow

## Description
This workflow automatically captures new Calendly meeting invitee details and saves them as a new entry in a Notion database.

## Input Details
The workflow is triggered when a new invitee is created in Calendly, receiving the invitee's name, email, and related event data.

## Process Summary
The workflow starts when a new Calendly invitee is created. It captures the invitee's name and email from the Calendly payload. These details are then formatted and sent to a specified Notion database. A static status (or other property) is also set in Notion using a predefined ID. If any step fails, the workflow halts with an error message.

## Output Details
The workflow creates a new page in a Notion database with the invitee's name, email, and a preset property value.

## Tags
Calendly, Notion, automation, invitee, database, scheduling, CRM, production-ready
