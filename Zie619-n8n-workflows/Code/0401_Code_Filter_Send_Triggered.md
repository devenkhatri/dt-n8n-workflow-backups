# Workflow Analysis for AI Agent with Google Sheets Custom Tools

## Description
An AI-powered chat agent that can answer questions about customer data stored in a Google Sheet by using custom tools to fetch column names, column values, or full customer records without loading the entire dataset into memory.

## Input Details
The workflow is triggered either by an incoming chat message or by being called from another workflow with an operation type and query parameter.

## Process Summary
The workflow starts when a chat message is received or when invoked by another workflow. If invoked as a sub-workflow, it reads the operation type (column_names, column_values, or row) and query parameter. It fetches customer data from a Google Sheet specified by a URL from environment variables. Based on the operation, it either returns all column names, values from a specific column for all customers, or a full customer record by row number. The results are formatted and returned as structured JSON responses for use by the AI agent.

## Output Details
The workflow returns structured JSON data back to the calling AI agent or parent workflow, enabling it to answer user questions about customer data stored in Google Sheets.

## Tags
AI agent, Google Sheets, custom tools, chat interface, data querying, n8n workflow, sub-workflow, customer data
