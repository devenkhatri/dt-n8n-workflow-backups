# Workflow Analysis for Website Chatbot

## Description
This workflow powers an AI-powered chatbot on a website that helps visitors book appointments with the founder or send detailed inquiries via email. The chatbot checks the founder's calendar for availability, books meetings in Microsoft Outlook, and collects necessary customer information while adhering to business hours and time zone constraints.

## Input Details
Triggered by incoming messages to a public webhook from the website chat widget, containing the user's chat input and session ID.

## Process Summary
The workflow receives chat messages via a webhook and uses an AI agent (powered by OpenAI) to understand user intent. If the user wants to book an appointment, it checks the founder's Microsoft Outlook calendar for free slots in the next 14 days within business hours (8am-5:30pm, Monday-Friday, Europe/London timezone). If the user prefers to speak to a human or has other inquiries, it collects detailed project information and sends a formatted email to the founder. The AI maintains conversation context using window buffer memory and ensures appointments are not double-booked.

## Output Details
Responds to the website chat with either appointment confirmation messages or acknowledgment of inquiry submission, and either creates a calendar event in Microsoft Outlook or sends a detailed HTML email to the founder.

## Tags
chatbot, appointment scheduling, Microsoft Outlook, AI agent, calendar integration, email notification, customer inquiry, OpenAI, webhook
