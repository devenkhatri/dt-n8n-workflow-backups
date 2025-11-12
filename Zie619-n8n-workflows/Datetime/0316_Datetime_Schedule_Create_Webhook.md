# Workflow Analysis for Sync Outlook Calendar Events to Notion

## Description
This workflow automatically fetches upcoming Outlook calendar events and syncs them to a Notion database, creating new entries for events not already present or updating existing ones.

## Input Details
The workflow is triggered on a schedule (every minute) and fetches Outlook calendar events from the current time up to one year in the future via an authenticated HTTP request.

## Process Summary
The workflow starts by triggering on a schedule, then calculates a future date one year ahead. It fetches Outlook calendar events between the current time and that future date. The events are split into individual items and compared against existing pages in a Notion database using a merge operation based on event ID. If an event doesn’t exist in Notion, it creates a new database page; if it does exist, it updates the existing page with the latest event details.

## Output Details
The workflow either creates new or updates existing pages in a specified Notion database with event details such as title, start/end time, event ID, and a related URL.

## Tags
calendar sync, Outlook, Notion, automation, scheduled workflow, event management, two-way sync
