# Workflow Analysis for Chat with Google Sheet

## Description
This workflow enables users to interact with a Google Sheet through a natural language chat interface powered by an AI agent. The AI can query the sheet by listing available columns, fetching specific customer data by row number, or retrieving values from a specific column across all rows—allowing complex questions like 'Which is our biggest customer?' to be answered automatically.

## Input Details
The workflow is triggered by a user message via a chat interface or by a call from an AI agent with a specific operation (e.g., 'column_names', 'row', or 'column_values') and optional query parameters.

## Process Summary
The workflow starts with a chat trigger that feeds user input to an AI agent. The agent decides which tool to use and calls the same workflow as a sub-workflow with an operation type and query. Based on the operation, the workflow either retrieves column names, filters a specific row, or extracts values from a given column in a connected Google Sheet. The sheet URL is set from an environment variable, and the results are formatted into a structured JSON response. Finally, the response is returned to the AI agent for further processing or direct user response.

## Output Details
The workflow returns structured JSON data (such as column names, a specific customer's data, or column values across all rows) back to the AI agent or chat interface for natural language response generation.

## Tags
AI agent, Google Sheets, natural language query, chatbot, workflow automation, n8n, production-ready, data lookup, OpenAI, reAct agent
