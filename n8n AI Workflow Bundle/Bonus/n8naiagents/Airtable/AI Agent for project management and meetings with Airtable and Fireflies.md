# Workflow Analysis for AI Agent for Project Management and Meetings with Airtable and Fireflies

## Description
This automation workflow streamlines meeting follow-ups by automatically processing meeting transcripts using AI. It identifies action items, creates tasks in Airtable, notifies clients about their tasks via email, and schedules follow-up calls in Google Calendar if needed.

## Input Details
The workflow is triggered by an incoming HTTP POST request to a webhook, typically from Fireflies AI, containing a `meetingId`.

## Process Summary
First, the workflow receives a meeting ID from the webhook. It then uses this ID to query the Fireflies AI API via GraphQL to retrieve the full meeting transcript, participant details, and a summary. An AI agent, powered by OpenAI GPT-4o, analyzes this information. Based on the analysis, the AI agent can perform three main actions: trigger a sub-workflow to create specific tasks in an Airtable database, send an email notification to clients with their individual action items and a meeting summary, or create a Google Calendar event for a follow-up call. The task creation sub-workflow splits the AI-generated tasks and creates individual records in Airtable, mapping task name, description, due date, priority, and project name.

## Output Details
The workflow creates new task records in an Airtable database, sends personalized meeting summary and action item emails to meeting participants, and can schedule new events in Google Calendar.
