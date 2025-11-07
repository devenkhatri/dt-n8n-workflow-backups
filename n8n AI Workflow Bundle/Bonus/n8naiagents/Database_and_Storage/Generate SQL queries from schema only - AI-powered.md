# Workflow Analysis for AI-Powered SQL Query Generation from Schema

## Description
This workflow allows users to interact with a MySQL database by generating SQL queries based solely on its schema, using an AI chat model. It first extracts and stores the database schema locally, then leverages AI to interpret user natural language requests and generate corresponding SQL queries or direct answers without needing to see the actual data.

## Input Details
The workflow is triggered by user input via a chat interface, receiving chat messages and session information.

## Process Summary
Initially, the workflow connects to a MySQL database to list all tables, extracts the schema for each table, and saves this consolidated schema to a local JSON file. For every subsequent chat message, it loads this local schema and combines it with the user's input. This data is then fed to an AI agent (OpenAI Chat Model) which generates an SQL query or a direct answer based on the schema and chat input. If an SQL query is generated, the workflow executes it against the MySQL database, formats the results, and merges them with the AI agent's response. If no SQL query is needed, the AI's direct response is provided.

## Output Details
The workflow outputs a conversational response, which can include the AI agent's answer, a generated SQL query, and the formatted results of the executed query.
