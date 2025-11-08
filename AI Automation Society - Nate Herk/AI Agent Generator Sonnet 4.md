# Workflow Analysis for AI Agent Generator Sonnet 4

## Description
This workflow acts as an AI agent that takes a natural language request from a chat message and automatically generates a functional n8n workflow based on that request, then provides a link to the newly created workflow.

## Input Details
The workflow is triggered by a received chat message containing a user's request for an n8n workflow.

## Process Summary
A chat message with a user's request is received by the "n8n Developer" agent, which utilizes GPT 4.1 mini and a simple memory. The "n8n Developer" agent then calls a "Developer Tool" which triggers a sub-workflow. The sub-workflow downloads the n8n documentation from Google Drive and extracts its text. An "n8n Builder" agent, powered by Claude Sonnet 4, uses the extracted documentation and the original user request to construct a new n8n workflow in JSON format. This generated workflow JSON is then imported into the n8n instance, creating a new workflow. Finally, a direct link to the newly created n8n workflow is generated and returned.

## Output Details
The workflow outputs a clickable link to the newly generated and deployed n8n workflow.
