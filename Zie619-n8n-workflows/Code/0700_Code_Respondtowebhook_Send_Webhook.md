# Workflow Analysis for AI-Powered Appointment Scheduler with Calendar Integration

## Description
This workflow automates the process of scheduling appointments by interacting with users via a chat interface, checking calendar availability, and either booking meetings or escalating inquiries to a human via email.

## Input Details
The workflow is triggered by a webhook containing a user's chat input, which may include requests to check availability, book appointments, or send messages to a human representative.

## Process Summary
The workflow starts by checking if a valid chat message was received. If so, it uses an AI agent (configured with OpenAI) to interpret the user’s intent based on conversation context and business rules. If the user wants to check availability, the system fetches calendar events for the next 14 days, identifies free time slots within business hours (8am–5:30pm, Monday–Friday, Europe/London), and returns available times. If the user wants to book an appointment, the AI ensures all required details (name, email, company, reason, and valid time) are collected and creates a calendar event via Microsoft Outlook. If the user isn’t ready to book or has unrelated questions, the system gathers detailed project information and sends a formatted email to the founder.

## Output Details
The workflow responds to the user via the webhook with either available time slots, a confirmation of a booked appointment, or an acknowledgment that their message has been forwarded to a human; it also creates calendar events in Microsoft Outlook or sends detailed emails as needed.

## Tags
AI chatbot, appointment scheduling, calendar integration, Microsoft Outlook, OpenAI, webhook automation, customer support, lead qualification, business hours, time slot availability
