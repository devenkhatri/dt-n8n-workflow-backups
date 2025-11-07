# Workflow Analysis for Chat with Google Sheet

## Description
This workflow enables an AI agent to interact with a Google Sheet to answer questions. It uses a custom tool approach, allowing the AI to query column names, retrieve all values for a specific column, or fetch an entire row for a given customer from the Google Sheet.

## Input Details
The workflow is triggered by a chat interface where a user asks questions to an AI agent, and a sub-workflow is triggered by the AI agent, receiving an operation type and a query (e.g., column name or row number).

## Process Summary
A user's chat input initiates the main workflow, which uses an AI agent powered by OpenAI. The AI agent then identifies the user's intent and utilizes one of three custom tools to interact with a Google Sheet: `list_columns`, `get_customer`, or `column_values`. These tools trigger a sub-workflow that first sets the Google Sheet's URL and retrieves its contents. Based on the specific tool called, the sub-workflow either extracts column names, filters for a specific row, or retrieves values for a specified column across all rows. Finally, the extracted data is prepared as a JSON response.

## Output Details
The workflow provides natural language answers to user queries through the chat interface, and the sub-workflow returns structured JSON data from the Google Sheet to the AI agent.
