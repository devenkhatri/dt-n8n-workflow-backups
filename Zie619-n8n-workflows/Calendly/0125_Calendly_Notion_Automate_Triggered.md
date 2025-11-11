# Workflow Analysis for Notion Workflow

## Description
This workflow automatically captures new Calendly meeting bookings, enriches invitee contact details using Dropcontact, and logs the appointment information into a Notion database.

## Input Details
The workflow is triggered by a 'invitee.created' event from Calendly, receiving booking and invitee data such as name, email, and meeting times.

## Process Summary
When a new Calendly invitee is created, the workflow sends the invitee's details to Dropcontact to enrich their contact information. The enriched data, along with meeting start and end times, is then used to create a new page in a Notion database with fields for name, email, civility, meeting times, and related URLs. Environment variables like BASE_URL are used to populate URL fields consistently. If any step fails, the workflow triggers an error handler to log the issue.

## Output Details
The workflow creates a new entry in a Notion database containing the enriched invitee information and meeting details.

## Tags
Calendly, Notion, Dropcontact, automation, CRM, lead enrichment, scheduling, production-ready
