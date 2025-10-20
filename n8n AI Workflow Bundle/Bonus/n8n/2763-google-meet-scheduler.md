# Workflow Analysis for Google Meet Scheduler

## Description
This workflow automates the scheduling of Google Meet meetings by taking meeting details from a form, creating a Google Calendar event, and then sending an email notification with the meeting link to the attendee.

## Input Details
This workflow is triggered manually and requires meeting details such as attendee email, meeting start and end times, and meeting topic as input.

## Process Summary
The workflow starts by retrieving manual input for meeting details. It then checks if the attendee email is valid. If valid, it creates a Google Calendar event with the provided details and a Google Meet conference. Finally, it sends an email to the attendee with the meeting link and details.

## Output Details
The workflow creates a Google Calendar event with a Google Meet link and sends an email notification to the specified attendee.
