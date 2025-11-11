# Workflow Analysis for Calendlytrigger Workflow

## Description
This workflow automatically creates or updates a contact in Mautic whenever a new event is scheduled in Calendly.

## Input Details
The workflow is triggered by a new Calendly event (specifically, an 'invitee.created' event), which provides the invitee's name and email.

## Process Summary
The workflow starts when a new Calendly event occurs. It captures the invitee's email and name from the event payload. It then uses this data to create a new contact in Mautic or update an existing one with the same email by setting the first name. The workflow includes error handling to stop execution and report errors if something goes wrong.

## Output Details
The workflow creates or updates a contact record in Mautic with the invitee's email and first name.

## Tags
Calendly, Mautic, contact sync, automation, CRM integration, lead capture
