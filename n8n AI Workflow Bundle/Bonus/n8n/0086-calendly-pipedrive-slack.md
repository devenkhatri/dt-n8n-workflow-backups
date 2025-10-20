# Workflow Analysis for Automated Meeting Scheduling and CRM Update

## Description
This workflow automates the process of scheduling meetings via Calendly, updates Pipedrive CRM, and notifies a Slack channel about new meeting bookings.

## Input Details
The workflow is triggered by a Calendly webhook whenever a new meeting event is created.

## Process Summary
The workflow starts when a new Calendly event is created. It then extracts relevant data from the Calendly webhook payload. Subsequently, it creates or updates a person in Pipedrive with the guest's information. Following this, it creates a new activity in Pipedrive linked to the person and the meeting details. Finally, it sends a Slack notification to a specified channel with information about the newly booked meeting, including meeting details and Pipedrive links.

## Output Details
The workflow updates Pipedrive CRM with new person and activity data, and sends a notification to a Slack channel.
