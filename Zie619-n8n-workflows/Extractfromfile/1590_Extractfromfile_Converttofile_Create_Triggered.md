# Workflow Analysis for Generate SQL queries from schema only - AI-powered

## Description
This workflow allows users to interact with a MySQL database using natural language. It uses an AI agent (powered by OpenAI's GPT-4o) that understands the database schema and generates SQL queries based on user requests—but does not execute them itself. The workflow caches the database schema locally for performance and security, then processes user questions via chat, returning either direct answers or SQL query results when applicable.

## Input Details
The workflow is triggered by a chat message input (via a Chat Trigger node) that contains a user's natural language request about the database.

## Process Summary
First, the workflow loads a pre-saved local JSON file containing the full database schema (generated once via a manual trigger by querying all table structures). When a chat message arrives, it combines the schema and user input into a prompt for an AI agent. The agent responds with either a direct answer or a SQL query wrapped in triple quotes. The workflow then uses a regular expression to extract any SQL query from the response. If a query is found, it executes the query against the MySQL database, formats the results into a readable markdown table, and merges it with the agent's response for final output.

## Output Details
The workflow outputs a combined response that includes the AI-generated explanation and, if applicable, the formatted results of the executed SQL query—sent back to the chat interface.

## Tags
AI, SQL, MySQL, database, chatbot, n8n, automation, GPT-4, schema, natural language
