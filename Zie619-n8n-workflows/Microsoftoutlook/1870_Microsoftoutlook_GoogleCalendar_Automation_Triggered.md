# Workflow Analysis for Google calendar to Outlook

## Description
Automated workflow: Google calendar to Outlook. This workflow processes data and performs automated tasks.

## Input Details
The workflow is triggered by new or cancelled events detected every minute in a specified Google Calendar.

## Process Summary
The workflow continuously monitors a Google Calendar for new or cancelled events. Upon detecting a new event, it creates a corresponding event in an Outlook Calendar, copying details such as the event summary, description, start, and end times. If an event is cancelled in Google Calendar, the workflow searches the Outlook Calendar for the matching event, deletes it, and then sends an email notification via Outlook to a specified recipient confirming the event's cancellation.

## Output Details
The workflow creates or deletes events in Microsoft Outlook Calendar and sends email notifications for cancelled events.

## Tags
automation, n8n, production-ready, excellent, optimized
