# Workflow Analysis for Connect Airtable Contacts to telli for Automated AI Voice Call Scheduling

## Description
This workflow seamlessly integrates Airtable CRM with telli's AI voice-agents to automate outbound calling processes. It eliminates manual call scheduling and data transfer, saving time and reducing errors for tasks like lead qualification, appointment reminders, and customer feedback.

## Input Details
The workflow is triggered by new or updated records in a specified Airtable base and table, polling for changes every minute based on the 'Created Time' field.

## Process Summary
First, new contact data from Airtable is sent via an HTTP POST request to the telli API's `/add-contact` endpoint to create the contact in telli. Next, another HTTP POST request is made to the telli API's `/schedule-call` endpoint, using the newly created contact's ID, to automatically schedule an AI voice call based on predefined smart calling strategies.

## Output Details
The workflow produces automated AI voice calls scheduled through the telli platform for the contacts added from Airtable.

## Tags
Airtable, telli, Automation, CRM, AI Voice Call, Scheduling, HTTP Request, Contact Management, Lead Qualification, Appointment Reminders, Customer Feedback
