# Workflow Analysis for Calendar_scheduling

## Description
This workflow automatically checks incoming Gmail messages to identify appointment requests, verifies the sender's intent using an AI model, retrieves the user's Google Calendar availability for the next month, and sends a smart reply proposing a meeting time based on free slots.

## Input Details
The workflow is triggered by unread Gmail emails and receives email data including sender, subject, and snippet text.

## Process Summary
First, it polls Gmail for unread emails. It uses an LLM to classify whether each email is an appointment request. If confirmed, it fetches the user's Google Calendar events for the next month, filters only confirmed events with set times, and formats them with start, end, and summary. The formatted availability is sorted and passed to another LLM agent that composes a human-like reply suggesting a suitable time. Finally, the original email is marked as read and the AI-generated reply is sent.

## Output Details
The workflow sends an AI-generated reply email with proposed meeting times and marks the original email as read.

## Tags
calendar, scheduling, gmail, AI, automation, n8n, production-ready, appointment, Google Calendar, LLM
