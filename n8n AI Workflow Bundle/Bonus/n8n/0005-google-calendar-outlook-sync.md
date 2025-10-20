# Workflow Analysis for Google Calendar Outlook Sync

## Description
This workflow synchronizes events between a Google Calendar and an Outlook Calendar, ensuring that events created in one calendar are replicated in the other.

## Input Details
The workflow is triggered by an HTTP Webhook, which receives data from an external source, likely signaling a new or updated calendar event.

## Process Summary
The workflow begins by receiving event data via an HTTP webhook. It then determines if the event originated from Google Calendar or Outlook Calendar using an IF node. Depending on the source, it extracts event details, transforms them to the format required by the destination calendar, and then creates the event in the respective calendar. For example, if a Google Calendar event is detected, the workflow creates that event in Outlook Calendar.

## Output Details
The workflow outputs synchronized calendar events, creating new events in either Google Calendar or Outlook Calendar based on the input.
