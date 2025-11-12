# Workflow Analysis for Google Cal to Zoom meeting

## Description
This workflow automatically creates Zoom meetings for upcoming Google Calendar events that meet specific criteria, ensuring virtual meetings are set up without manual intervention.

## Input Details
The workflow is triggered either manually or automatically once a day at 7 AM UTC, and it fetches upcoming Google Calendar events within the next 12 hours.

## Process Summary
The workflow starts by calculating a time window of the next 12 hours. It then retrieves Google Calendar events within that window. An IF node filters out unwanted events such as canceled meetings, in-person meetings, Signal meetings, or meetings created by Calendly. For each qualifying event, the workflow creates a corresponding Zoom meeting using the event's title, start time, duration, and time zone. Errors during execution are caught and handled by an error handler node.

## Output Details
The workflow creates Zoom meetings for eligible Google Calendar events and outputs the meeting details via the Zoom API.

## Tags
automation, calendar integration, Zoom, Google Calendar, meeting scheduler, n8n, production-ready
