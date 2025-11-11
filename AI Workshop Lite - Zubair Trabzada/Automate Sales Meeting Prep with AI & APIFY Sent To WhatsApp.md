# Workflow Analysis for AI Meeting Assistant with WhatsApp Notifications

## Description
This workflow acts as an AI-powered meeting assistant that automatically checks for upcoming meetings, gathers relevant context about attendees from emails and LinkedIn, and sends a concise pre-meeting summary to the user via WhatsApp to help them prepare.

## Input Details
The workflow is triggered on an hourly schedule and receives data about upcoming calendar meetings from Google Calendar.

## Process Summary
The workflow first checks Google Calendar for meetings scheduled within the next hour. For each meeting attendee, it extracts contact details and then attempts to fetch their last email correspondence and LinkedIn profile activity. Using AI (OpenAI's GPT-4), it summarizes the email thread and LinkedIn profile into concise, relevant talking points. Finally, it compiles all attendee summaries and meeting details into a single pre-meeting notification message.

## Output Details
The workflow produces a personalized pre-meeting summary message and sends it to the user's WhatsApp number.

## Tags
ai, meeting assistant, google calendar, gmail, linkedin, whatsapp, openai, automation, notifications, productivity
