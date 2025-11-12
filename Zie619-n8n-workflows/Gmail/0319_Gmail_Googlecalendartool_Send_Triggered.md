# Workflow Analysis for Email Appointment Scheduler

## Description
This workflow automatically checks incoming unread Gmail messages to determine if they are appointment requests. If so, it checks the user's Google Calendar availability and sends a smart reply proposing a suitable meeting time.

## Input Details
The workflow is triggered by unread emails in a Gmail inbox, receiving the email’s subject, snippet, sender, and message ID.

## Process Summary
The workflow starts by polling for unread Gmail messages. It uses an LLM to classify whether the email is an appointment request. If it is, the workflow fetches the user’s Google Calendar events for the next month. An AI agent then composes a context-aware reply suggesting a meeting time based on calendar availability and current date/time. Finally, the workflow sends the reply and marks the original email as read.

## Output Details
The workflow sends an automated reply email with a proposed meeting time and marks the original email as read in Gmail.

## Tags
email automation, appointment scheduling, LLM, Gmail, Google Calendar, AI assistant, n8n workflow
