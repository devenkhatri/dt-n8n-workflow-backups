# Workflow Analysis for AI-Powered Meeting Follow-Up Reminder and Booking

## Description
This workflow automatically checks for past meetings where no follow-up email was sent, suggests available time slots for a follow-up meeting using AI, and books the meeting after getting human approval via email.

## Input Details
The workflow is triggered daily at 6 AM and receives no external input—it fetches past calendar events and corresponding email threads automatically.

## Process Summary
The workflow starts by fetching Google Calendar events from 2–4 days ago. It then checks Gmail for any messages exchanged with meeting attendees since each event ended. Events with no follow-up emails are flagged. For those, an AI agent analyzes the original meeting details and retrieves available time slots from the user’s calendar. A follow-up message with suggested slots is sent to the user via Gmail’s send-and-wait-for-approval feature. Based on the user’s reply, another AI agent either books the follow-up meeting or takes no action.

## Output Details
The workflow either creates a new Google Calendar event for the follow-up meeting or does nothing if the user declines, based on human-in-the-loop approval received via email.

## Tags
ai agent, google calendar, gmail, meeting follow-up, human-in-the-loop, automation, sales engagement, calendar availability, OpenAI, n8n
