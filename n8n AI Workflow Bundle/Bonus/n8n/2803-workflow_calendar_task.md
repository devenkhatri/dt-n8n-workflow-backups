# Workflow Analysis for Automate Calendar Event Creation from Webhook

## Description
This workflow automates the creation of Google Calendar events based on information received from a webhook. It can handle both single events and recurring events, assigning them to a specified calendar and sending email notifications.

## Input Details
The workflow is triggered by an incoming webhook, receiving event data in JSON format.

## Process Summary
The workflow starts by extracting event information from the webhook data, including event name, description, start and end times, and attendee emails. It then checks if the event is recurring based on a "repetitions" property. If recurring, it creates a series of events; otherwise, it creates a single event. Before creating the event, it selects the target Google Calendar. Finally, it sends email notifications to attendees.

## Output Details
The workflow creates new events in Google Calendar and sends email notifications to the specified attendees.
