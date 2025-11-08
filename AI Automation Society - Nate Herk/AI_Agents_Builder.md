# Workflow Analysis for AI Agents Builder

## Description
This workflow acts as an AI-powered n8n workflow builder. It takes a user's natural language request and generates a complete n8n workflow JSON, which is then used to create a new workflow within n8n.

## Input Details
The workflow is triggered by a chat message, receiving the user's request for an n8n workflow as input.

## Process Summary
Upon receiving a chat message, the workflow first downloads the n8n documentation from Google Drive. It then extracts the text content from the downloaded documentation. An AI agent, powered by Claude Opus 4, uses the user's request and the n8n documentation as context to generate a new n8n workflow in JSON format. This generated workflow JSON is then used to create a new, functional workflow within n8n itself. Finally, a link to the newly created n8n workflow is generated.

## Output Details
The workflow produces a new n8n workflow based on the user's request and generates a direct link to this newly created workflow.
