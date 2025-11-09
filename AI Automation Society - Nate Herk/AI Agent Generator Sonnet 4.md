# Workflow Analysis for AI Agent Generator Sonnet 4

## Description
This workflow uses AI agents to automatically generate and deploy new n8n workflows based on natural language requests from users. It leverages Google Drive documentation, AI language models (OpenRouter and Anthropic), and the n8n API to interpret requests, build valid workflow JSON, and create new workflows in the user's n8n instance.

## Input Details
The workflow is triggered either by a chat message via a webhook or when executed by another workflow with a query parameter containing the user's natural language request.

## Process Summary
When triggered, the workflow fetches n8n documentation from Google Drive and extracts its text content. This documentation is combined with the user's request and sent to an AI agent (Claude Sonnet 4) that specializes in generating complete, valid n8n workflow JSON. The generated JSON is then sent to the n8n API to create a new workflow in the user's instance. Finally, a clickable link to the newly created workflow is generated and returned.

## Output Details
The workflow produces a clickable link to a newly created n8n workflow that was automatically generated based on the user's natural language request, and this link is returned as the output.

## Tags
AI Agent, Workflow Generation, n8n Automation, Claude Sonnet, Natural Language Processing, Google Drive, API Integration
