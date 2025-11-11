# Workflow Analysis for Chattrigger Workflow

## Description
An AI-powered workflow that allows users to interact with a chatbot to analyze transaction data stored in Google Sheets. The AI can answer questions about sales, refunds, and other transaction details by querying the data using various tools and sub-workflows.

## Input Details
The workflow is triggered by incoming chat messages and can also be invoked by another workflow with input parameters like start_date, end_date, and status.

## Process Summary
When a chat message is received, it is processed by an AI Agent powered by OpenAI's GPT-4o. The agent has access to multiple tools: it can fetch all transactions, filter by product name or status, or request data within a specific date range by calling a sub-workflow. The sub-workflow makes an HTTP request to Google Sheets, processes the JSONP response using custom JavaScript code to convert it into structured JSON, filters by status if needed, and aggregates the results before sending them back to the AI. The AI then formulates a natural language response based on the retrieved data.

## Output Details
The workflow outputs a natural language response from the AI agent back to the chat interface, based on the analyzed Google Sheets transaction data.

## Tags
AI Agent, Google Sheets, Chatbot, Data Analysis, Sub-workflow, n8n, automation, OpenAI, GPT-4o, HTTP Request, JSON parsing
