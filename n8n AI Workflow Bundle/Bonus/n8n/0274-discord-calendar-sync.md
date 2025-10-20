# Workflow Analysis for Discord Calendar Sync

## Description
This workflow automatically syncs Google Calendar events to Discord, creating new events and updating existing ones to keep your community informed about upcoming happenings.

## Input Details
This workflow is triggered daily by a Schedule Trigger.

## Process Summary
The workflow starts by retrieving events from a specified Google Calendar. It then iterates through these events, checking if each event already exists as a Discord event. If an event is new, the workflow creates a new Discord event. For existing events, it updates them to reflect any changes. Finally, it removes any Discord events that are no longer present in the Google Calendar.

## Output Details
The workflow creates and updates events in a designated Discord channel and removes outdated events.
