# Workflow Analysis for AI Agents Builder

## Description
This workflow allows users to describe an automation need in natural language via a chat interface, and automatically generates a complete, importable n8n workflow JSON based on that request using AI.

## Input Details
The workflow is triggered when a chat message is received containing a natural language description of a desired automation.

## Process Summary
When a chat message is received, the workflow first retrieves the n8n documentation from Google Drive and extracts its text content. This documentation is combined with the user's request and fed into an AI agent powered by Claude Opus 4, which is instructed to generate a valid, importable n8n workflow JSON. The generated JSON is then sent to the n8n API to create a new workflow in the user's instance. Finally, a direct link to the newly created workflow is generated and made available in the output.

## Output Details
The workflow produces a newly created n8n workflow based on the user's natural language request and returns a direct link to access it.

## Tags
AI Agent, Workflow Generator, Natural Language Automation, n8n Builder, Claude AI, Google Drive, Chat Trigger
