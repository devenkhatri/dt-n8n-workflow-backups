# Workflow Analysis for Interview Scheduler

## Description
An AI-powered interview scheduling assistant that checks the interviewer's Google Calendar availability, proposes suitable 30-minute time slots during business hours (9am–5pm EST, weekdays only), and automatically books confirmed interviews by creating calendar events with the candidate’s contact details.

## Input Details
The workflow is triggered by an incoming chat message from a candidate via a public webhook, containing their availability preferences, email, and phone number.

## Process Summary
The workflow starts by receiving a chat message from a candidate. It uses an AI agent (powered by GPT-4o-mini) to interpret the request, verify availability by executing a sub-workflow that checks the interviewer’s Google Calendar, and identifies free 30-minute slots during business hours on weekdays. If the candidate’s proposed time is unavailable, the AI suggests alternatives. Once confirmed, the AI outputs structured JSON with interview details. The system then creates a Google Calendar event and sends a confirmation response to the user.

## Output Details
The workflow creates a Google Calendar event for the confirmed interview and returns a formatted confirmation message with the interview details to the user.

## Tags
interview scheduling, AI chatbot, Google Calendar integration, OpenAI, n8n workflow, appointment booking, automation, production-ready
