# Workflow Analysis for Calendar Agent Demo

## Description
An AI-powered calendar assistant that can create events (with or without attendees) and retrieve daily event summaries using natural language commands.

## Input Details
The workflow is triggered manually or via another workflow and receives a natural language query about calendar actions (e.g., create an event or check events on a day).

## Process Summary
The workflow uses an OpenAI-powered Calendar Agent that interprets the user's natural language request. Based on the query, it decides to either create a calendar event (with or without an attendee) or fetch events for a specific day. It interacts with Google Calendar using the appropriate tool, passing AI-extracted parameters like event title, start/end times, and attendee emails. The agent assumes a 60-minute duration if no end time is provided. Finally, the result from the calendar operation is captured and returned as a response.

## Output Details
The workflow returns the result of the calendar operation (e.g., confirmation of event creation or a summary of retrieved events) as a structured response.

## Tags
AI Agent, Calendar Management, Google Calendar, OpenAI, Event Creation, Event Lookup, Natural Language Processing
