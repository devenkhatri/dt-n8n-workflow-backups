# Workflow Analysis for AI Meeting Agent for Project Task Automation

## Description
This workflow automatically processes meeting transcripts from Fireflies to create project tasks in Airtable, notify clients via email about their action items, and schedule follow-up Google Meet calls when needed—all powered by AI.

## Input Details
The workflow is triggered by a webhook that receives a meeting completion event containing a meeting ID from Fireflies.

## Process Summary
The workflow starts by receiving a meeting ID via a webhook, then fetches the full meeting transcript using a GraphQL API call to Fireflies. If the meeting title includes 'project,' an AI agent analyzes the transcript to extract action items. It creates tasks in Airtable for the user (excluding others' tasks), emails each participant (except the user) their specific action items and meeting summary, and schedules a Google Meet event if a follow-up call is mentioned in the transcript.

## Output Details
The workflow creates tasks in Airtable, sends personalized email summaries to meeting participants via Gmail, and optionally schedules Google Calendar events with Google Meet links.

## Tags
AI agent, meeting automation, project management, Fireflies, Airtable, Gmail, Google Calendar, task creation, transcript analysis, n8n
