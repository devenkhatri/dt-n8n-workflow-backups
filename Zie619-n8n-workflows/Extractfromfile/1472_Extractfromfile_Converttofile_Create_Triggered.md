# Workflow Analysis for Generate SQL queries from schema only - AI-powered

## Description
This workflow uses an AI language model to generate SQL queries based on a database schema without accessing actual data. It first extracts and saves the schema from a MySQL database, then allows users to send natural language requests via chat. The AI interprets the request using the saved schema and generates a relevant SQL query, which is then executed and returned with formatted results.

## Input Details
The workflow is triggered by a chat message containing a natural language request, and it uses a pre-saved local JSON file of the database schema.

## Process Summary
The workflow begins by extracting the full database schema from a MySQL database and saving it as a local JSON file. When a user sends a chat message, the workflow loads this schema file and combines it with the user's input. This combined data is sent to an AI agent configured to generate SQL queries based only on the schema. If a query is detected in the AI's response, it is executed against the database, and the results are formatted into a readable table. Finally, the AI’s original response and the formatted query results are combined and returned to the user.

## Output Details
The workflow outputs a combined response containing the AI-generated explanation and the formatted SQL query results, which is sent back to the chat interface.

## Tags
AI, SQL, database, schema, chat, MySQL, automation, n8n, production-ready, LangChain
