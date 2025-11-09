# Workflow Analysis for AI Agent Generator Opus 4

## Description
This workflow uses AI to automatically generate n8n automation workflows based on natural language requests from users. It leverages documentation, advanced language models, and internal tools to produce ready-to-deploy workflow JSON.

## Input Details
The workflow is triggered either by a chat message via a webhook or by another workflow passing a natural language query.

## Process Summary
When triggered, the workflow first retrieves and extracts content from an n8n documentation Google Doc. It then passes the user's request along with the documentation to an AI agent (Claude Opus 4) that generates a complete, valid n8n workflow JSON. A code node cleans and parses the AI's JSON output. The parsed workflow is then submitted to the n8n API to create a new workflow, and a clickable link to the new workflow is generated.

## Output Details
The workflow produces a new n8n workflow in the user's instance and outputs a direct link to it, which can be returned to the user via the chat interface.

## Tags
AI Agent, Workflow Generator, n8n Automation, Claude Opus, Natural Language to Workflow, Google Drive, API Integration
