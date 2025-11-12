# Workflow Analysis for Daylight Saving Time Notification

## Description
This workflow checks configured timezones to see if any will switch to or from Daylight Saving Time (DST) tomorrow, and sends notifications via Slack and email to alert users so they can adjust meeting times accordingly.

## Input Details
The workflow is triggered either manually or on a schedule, and uses a hardcoded list of timezones defined in the workflow itself.

## Process Summary
The workflow starts by loading a list of timezones. For each timezone, it calculates the current date/time and tomorrow’s date/time in that zone. It then checks whether DST status differs between today and tomorrow. If a change is detected, the workflow sends a notification via both Slack and email warning of the upcoming DST change.

## Output Details
The workflow sends alerts via Slack message and email to notify users about upcoming Daylight Saving Time changes in specified timezones.

## Tags
Daylight Saving Time, DST notification, timezone automation, Slack alert, email notification, scheduled workflow, n8n
