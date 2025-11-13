# Workflow Analysis for HubSpot New Contact Onboarding Workflow

## Description
This automated workflow streamlines the onboarding process for new customers by integrating HubSpot, an AI agent for personalized communication, and Google Calendar. It aims to ensure new customers receive all necessary resources and support efficiently.

## Input Details
The workflow is primarily triggered by a webhook that receives contact creation events from HubSpot.

## Process Summary
1. The workflow starts upon receiving a new contact creation event from HubSpot via a webhook.
2. It initializes company-specific information and identifies the appropriate contact owner from HubSpot.
3. Upon confirming a new contact creation, it retrieves all details for that contact from HubSpot.
4. An AI agent generates a personalized welcome email, instructing a calendar agent to schedule a welcome call with the new contact.
5. The email body, initially in markdown, is converted to HTML and then sent to the new contact via Gmail, with a BCC to the sender. Finally, the identified owner is assigned to the newly created contact in HubSpot.

## Output Details
The workflow sends a personalized welcome email to the new contact, assigns a HubSpot owner to the contact, and schedules a welcome call in Google Calendar.

## Tags
automation, n8n, production-ready, excellent, optimized, hubspot, gmail, google calendar, AI, customer onboarding
