# Workflow Analysis for Lmchatopenai Workflow

## Description
This workflow acts as an intelligent assistant, routing user chat inputs to specialized agents for managing Google Calendar events or Notion tasks. It uses AI models to understand requests and maintains conversation context, providing a seamless experience for scheduling and task management.

## Input Details
The workflow is triggered by either an incoming webhook request or a chat message, receiving a user prompt (chat input) and a session ID.

## Process Summary
1. The workflow receives a chat message or webhook request containing user input and a session ID.
2. It maps the incoming data into `chatInput` and `sessionId` variables.
3. A "Main Agent", powered by an OpenAI Chat Model and utilizing conversation memory, analyzes the `chatInput` to determine its intent.
4. Based on the intent, the "Main Agent" routes the request to either a "calendarAgent" (for Google Calendar event management) or a "taskAgent" (for Notion task management), each operating as a sub-workflow with its own AI model and tools.
5. The chosen sub-agent processes the request, performs the relevant action (e.g., checking calendar availability, booking an appointment, or creating a Notion task), and generates a response.
6. Finally, the main workflow formats the agent's response, separating the text and speech components, before sending it back to the user.

## Output Details
The workflow responds to the originating webhook with a structured JSON containing the processed text response and a speech-optimized version of the response.

## Tags
automation, n8n, production-ready, excellent, optimized, AI, Agent, Calendar, Task Management, OpenAI, Google Calendar, Notion, Workflow Orchestration
