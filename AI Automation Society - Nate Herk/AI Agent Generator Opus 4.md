# Workflow Analysis for AI Agent Workflow Generator

## Description
This workflow acts as an AI agent that generates n8n workflows based on natural language requests from users. It leverages large language models (LLMs) and n8n documentation to interpret requests, automatically create functional n8n workflows, and then provides a link to the newly created workflow.

## Input Details
The workflow is primarily triggered by incoming chat messages from a user, containing a request for an n8n workflow.

## Process Summary
1. A user's chat message triggers the workflow, initiating an n8n Developer agent. 2. The n8n Developer agent, using memory and an LLM, calls a "Developer Tool" to construct a new workflow based on the user's request. 3. The "Developer Tool" executes a sub-part of this workflow, which retrieves n8n documentation from Google Drive. 4. An n8n Builder agent (powered by Claude Opus 4) leverages this documentation and the user's request to generate a complete n8n workflow in JSON format. 5. A Code node then attempts to parse and clean this generated JSON. 6. Finally, the workflow uses the n8n API to create the new workflow and generates a clickable link for the user.

## Output Details
The workflow creates a new n8n workflow based on the user's request and returns a clickable link to this newly generated workflow in the chat.
