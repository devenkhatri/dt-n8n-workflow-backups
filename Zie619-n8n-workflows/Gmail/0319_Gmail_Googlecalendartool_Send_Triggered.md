# Workflow Analysis for Email Appointment Scheduler

## Description
This workflow automatically checks incoming unread Gmail messages to determine if they are appointment requests. If so, it checks the user's Google Calendar availability and sends a smart reply suggesting a meeting time, then marks the email as read.

## Input Details
The workflow is triggered by unread emails in a Gmail inbox, polling every minute for new messages.

## Process Summary
The workflow starts by polling unread Gmail messages. It uses an LLM to classify whether the email is an appointment request based on the subject and snippet. If it is, the workflow fetches the user’s Google Calendar events for the next month. An AI agent then composes a response proposing a specific meeting time based on availability, ensuring a 15-minute buffer between meetings. Finally, the workflow sends the reply and marks the original email as read.

## Output Details
The workflow sends an email reply with a proposed meeting time and marks the original email as read in Gmail.

## Tags
email automation, appointment scheduling, AI assistant, Gmail integration, Google Calendar, LLM, workflow automation
