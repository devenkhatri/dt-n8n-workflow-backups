# Workflow Analysis for Appointment Leads Follow-up Workflow

## Description
This workflow automates the follow-up process for new appointment leads by sending personalized emails and SMS messages.

## Input Details
The workflow is triggered by new appointment lead data received via a webhook.

## Process Summary
The workflow starts by retrieving appointment details from the incoming webhook data. It then extracts customer information such as name, email, and phone number. Subsequently, it sends a personalized email to the customer using an SMTP service and a personalized SMS message via Twilio. Finally, the workflow records the lead data in a Google Sheet for tracking and analysis.

## Output Details
The workflow sends a personalized email and SMS to the lead and logs the lead details in a Google Sheet.
