# Workflow Analysis for AI Meeting Agent for Project Task Automation

## Description
This workflow automatically processes meeting transcripts from Fireflies to create actionable tasks in Airtable, notify clients via email, and schedule follow-up meetings in Google Calendar when needed—specifically for meetings related to projects.

## Input Details
The workflow is triggered by a POST webhook that receives a meeting completion event with a meeting ID from Fireflies.

## Process Summary
The workflow starts by fetching the full meeting transcript using a GraphQL API call to Fireflies. If the meeting title contains 'project', an AI agent analyzes the transcript to extract tasks assigned to the user, then creates those tasks in Airtable. The agent also identifies action items for other participants and emails each participant their specific tasks via Gmail. If the transcript indicates a need for a follow-up call, the workflow schedules a Google Meet event in Google Calendar with the relevant client.

## Output Details
The workflow creates tasks in Airtable, sends personalized email summaries with action items to meeting participants, and optionally schedules Google Calendar events for follow-up calls.

## Tags
AI agent, meeting automation, task management, Airtable, Fireflies, Google Calendar, Gmail, project management, n8n, workflow automation
