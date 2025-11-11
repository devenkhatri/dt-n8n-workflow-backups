# Workflow Analysis for Calendly Meeting → CRM Company & Contact Enrichment

## Description
This workflow automatically enriches and syncs company and contact data from Calendly meeting bookings into HubSpot CRM, using Clearbit to gather company and person details. It ensures only professional (non-personal) email domains are processed, creates or updates companies in HubSpot, and links the meeting invitee as a contact or lead.

## Input Details
The workflow is triggered by a new Calendly invitee.created event, which provides the attendee’s email and other booking details.

## Process Summary
The workflow starts when someone books a meeting via Calendly. It first filters out personal email domains (like Gmail or Yahoo). For valid business emails, it uses Clearbit to enrich the person’s data and extract their company domain. If a company domain exists, it enriches the company data via Clearbit, searches HubSpot for an existing company record, and either creates a new company or updates the existing one. Finally, it upserts the invitee as a contact in HubSpot and associates them with the company.

## Output Details
The workflow creates or updates company and contact records in HubSpot CRM with enriched data from Clearbit, ensuring accurate and actionable lead information.

## Tags
Calendly, HubSpot, Clearbit, CRM sync, lead enrichment, company enrichment, automation, n8n, production-ready
