# Workflow Analysis for AI-Powered Appointment Scheduler with Calendar Integration

## Description
This workflow powers a chatbot that helps website visitors book appointments by checking the founder's calendar availability, collecting customer details, and either scheduling a meeting or forwarding complex inquiries to a human via email.

## Input Details
The workflow is triggered by incoming chat messages via a public webhook, receiving user input such as availability preferences, contact details, and meeting reasons.

## Process Summary
The workflow starts by validating incoming chat input. If valid, it uses an AI agent (configured with business rules) to converse with the user, gather necessary details, and determine intent. If the user wants to book an appointment, the workflow fetches calendar events for the next 14 days, identifies free time slots within business hours (8am–5:30pm, Monday–Friday, Europe/London), and presents options. Once a slot is confirmed, it creates a 30-minute online meeting in Outlook. If the user prefers human assistance or has non-appointment queries, the workflow collects detailed project information and sends a branded HTML email to the founder.

## Output Details
The workflow either books an appointment in Microsoft Outlook and confirms it to the user, or sends a detailed customer inquiry email to the founder, and always responds to the original webhook with appropriate messages or availability data.

## Tags
appointment scheduling, AI chatbot, calendar integration, Microsoft Outlook, OpenAI, workflow automation, customer engagement, lead qualification, n8n, no-code
