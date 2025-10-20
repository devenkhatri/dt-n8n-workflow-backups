# Workflow Analysis for Google Calendar Meeting Notifications to Slack

## Description
This workflow automatically sends notifications to a Slack channel when new meetings are created or updated in Google Calendar. This helps teams stay informed about schedule changes without manually checking their calendars.

## Input Details
The workflow is triggered at regular intervals by a Cron node, checking for new or updated Google Calendar events.

## Process Summary
The workflow starts by fetching events from Google Calendar. It then filters these events to include only those within a 30-minute window from the current time. Next, it checks if any events are found. If events exist, it formats the event details into a message for Slack. Finally, it sends this formatted message to a specified Slack channel.

## Output Details
The workflow sends meeting details as formatted messages to a designated Slack channel, ensuring team members receive timely notifications.
