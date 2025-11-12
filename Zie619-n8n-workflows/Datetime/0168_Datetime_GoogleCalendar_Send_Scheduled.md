# Workflow Analysis for Monthly Absence Reporting Workflow

## Description
This workflow automatically retrieves employee absence records (holiday and illness) from Google Calendar for the previous month, calculates the total days per employee by absence type, and emails a summary report to the payroll team on the 1st of every month at 8 AM.

## Input Details
The workflow is triggered automatically on the 1st of every month at 8 AM via a cron scheduler and uses the current date to calculate the previous month's date range for fetching calendar events.

## Process Summary
The workflow starts by scheduling execution on the 1st of each month at 8 AM. It calculates the date range for the previous month and fetches all Google Calendar events within that period. Events are filtered based on whether their summary contains 'Holiday' or 'Illness'. For each type, it extracts the employee name from the event description, calculates the duration in days, and aggregates total days per employee. Finally, it compiles a textual summary and emails it to the payroll team.

## Output Details
The workflow sends a formatted email to payroll-team@mydomain.tld summarizing total holiday and illness days per employee for the previous month.

## Tags
absence tracking, payroll automation, Google Calendar, monthly report, email notification, HR automation, time tracking
