# Workflow Analysis for Chat with Google Sheet

## Description
This workflow enables users to interact with a Google Sheet through a natural language chat interface powered by an AI agent. The AI can answer questions about the sheet data by using custom tools to fetch column names, retrieve specific customer rows, or get values from a particular column across all rows.

## Input Details
The workflow is triggered either by a chat message via a webhook or by a manual execution that provides an operation type (e.g., 'column_names', 'row', or 'column_values') and an optional query parameter.

## Process Summary
The workflow starts by loading data from a predefined Google Sheet. Based on the requested operation, it either returns all column names, retrieves a specific customer row by row number, or extracts values from a specified column across all customers. The AI agent, powered by OpenAI's language model, uses these tools to answer user questions intelligently. Results are formatted into a JSON response for consumption by the chat interface or calling workflow.

## Output Details
The workflow outputs structured JSON data based on the requested operation, which is either returned to the AI agent for generating a chat response or sent back to the triggering workflow.

## Tags
AI Agent, Google Sheets, Chat Interface, OpenAI, Custom Tools, Data Query
