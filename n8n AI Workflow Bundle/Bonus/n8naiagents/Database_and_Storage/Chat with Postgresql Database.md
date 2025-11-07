# Workflow Analysis for Chat with PostgreSQL Database

## Description
This workflow enables users to interact with a PostgreSQL database through a natural language chat interface, allowing them to ask questions and receive database query results in an understandable format.

## Input Details
The workflow is triggered when a chat message is received.

## Process Summary
Upon receiving a chat message, an AI Agent, configured as a DB assistant, processes the request. It utilizes an OpenAI Chat Model for language understanding and decision-making, while also maintaining chat history. The AI Agent can access three PostgreSQL tools: one to execute custom SQL queries, another to retrieve the database schema and a list of tables, and a third to fetch specific table definitions. Based on the user's query, the AI Agent intelligently selects and uses these tools to generate and execute appropriate SQL queries against the connected PostgreSQL database.

## Output Details
The workflow outputs a natural language response to the user's chat message, derived from the data retrieved by executing SQL queries on the PostgreSQL database.
