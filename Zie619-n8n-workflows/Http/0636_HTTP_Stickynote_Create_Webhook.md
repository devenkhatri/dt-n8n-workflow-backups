# Workflow Analysis for SQL Agent with Chart Generation

## Description
This workflow enables users to ask natural language questions about a SQL database and receive answers enhanced with automatically generated charts when appropriate. It combines a SQL query agent with AI-powered chart creation to support data-driven conversations.

## Input Details
The workflow is triggered by a user sending a chat message containing a natural language question about database data.

## Process Summary
First, the user's question is extracted, removing any chart-related phrasing. Then, an SQL agent queries the connected database and returns a plain-text answer. A text classifier determines if the response would benefit from a visual chart. If so, the workflow sends the data and request to OpenAI with a structured JSON schema to generate a Chart.js configuration. This configuration is embedded into a Quickchart.io URL to produce a chart image, which is appended to the original text response.

## Output Details
The workflow outputs a combined response containing the SQL agent's answer and, when relevant, an embedded chart image linked via Quickchart.io.

## Tags
SQL agent, data visualization, AI chart generation, natural language query, Chart.js, OpenAI structured output, Quickchart.io, database analytics, n8n automation, production-ready
