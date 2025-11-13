# Workflow Analysis for AI Agent with charts capabilities using OpenAI Structured Output

## Description
This workflow enables an AI chat agent to generate and embed charts in conversations by leveraging OpenAI’s structured output feature to produce valid Chart.js configurations, which are then rendered as images via Quickchart.io.

## Input Details
The workflow is triggered when a chat message is received by the AI Agent, which may include a request for a chart.

## Process Summary
When a user requests a chart during a chat, the AI Agent invokes a 'Generate a chart' tool that passes the user's query to a sub-workflow. This sub-workflow sends the query to OpenAI using a structured JSON schema to ensure the response conforms to Chart.js specifications. OpenAI returns a valid chart configuration in JSON format. The workflow then embeds this configuration into a Quickchart.io URL to generate a chart image. Finally, the image URL is returned to the AI Agent to be included in its response to the user.

## Output Details
The workflow outputs a Quickchart.io image URL representing the requested chart, which is sent back to the AI Agent for inclusion in the chat response.

## Tags
AI Agent, chart generation, OpenAI, structured output, Quickchart, Chat.js, n8n, automation, production-ready, workflow
