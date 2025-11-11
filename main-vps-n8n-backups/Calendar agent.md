# Workflow Analysis for Calendar Agent

## Description
An AI-powered calendar assistant that interacts with Google Calendar to check availability and retrieve events based on user requests via chat.

## Input Details
The workflow is triggered by incoming chat messages through a webhook, which contain natural language requests related to calendar availability or events.

## Process Summary
The workflow starts when a user sends a chat message. The message is processed by an AI agent using the GPT-4o-mini model with conversation memory enabled. Based on the user's request, the agent dynamically calls either the 'Get availability' or 'Get events' Google Calendar tools, using date parameters extracted by the AI. The tools fetch relevant calendar data, and the agent formulates a natural language response using the retrieved information.

## Output Details
The workflow returns a conversational AI response to the user, summarizing calendar availability or listing events based on the original request, delivered through the chat interface.

## Tags
AI Agent, Google Calendar, Chatbot, Availability Check, Event Retrieval, Natural Language Processing, Automation
