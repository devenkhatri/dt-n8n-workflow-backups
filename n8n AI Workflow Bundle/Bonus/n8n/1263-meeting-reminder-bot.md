# Workflow Analysis for Meeting Reminder Bot for Google Calendar

## Description
This workflow acts as a meeting reminder bot, fetching upcoming Google Calendar events and sending reminders via Telegram.

## Input Details
This workflow is triggered every 5 minutes by a Cron scheduler.

## Process Summary
First, it sets the current date and time. Then, it retrieves Google Calendar events for the next 24 hours. It filters these events to include only those within the next 30 minutes that have not been cancelled. Finally, for each filtered event, it constructs and sends a reminder message to a specified Telegram chat.

## Output Details
The workflow sends meeting reminder messages to a designated Telegram chat.
