# Workflow Analysis for Lmchatopenai Workflow

## Description
This workflow enables users to interact with an AI-powered chat assistant that answers supply chain analytics questions by querying a BigQuery database. The AI interprets natural language requests, generates appropriate SQL queries, executes them securely, and returns clean, structured results—all through a chat interface.

## Input Details
The workflow is triggered by user input via a chat interface (e.g., a web chat, Telegram, Slack, or webhook), where the user submits natural language questions about shipment data.

## Process Summary
The workflow starts when a user sends a message through the chat trigger. The AI Control Tower Agent, powered by an OpenAI chat model (gpt-4o-mini), interprets the request and formulates a SQL query based on the 'transport.shipments' BigQuery table schema. It then calls a separate 'BigQuery Tool' workflow, passing the query. Before execution, a code node sanitizes the query by removing markdown formatting. The cleaned query is executed in Google BigQuery, and the results are returned back to the AI agent, which formats and sends them to the user as a structured response.

## Output Details
The workflow outputs a natural language response containing structured data (e.g., tables or metrics) derived from BigQuery, delivered back to the user through the original chat interface.

## Tags
AI agent, BigQuery, SQL query, supply chain analytics, chatbot, natural language to SQL, n8n workflow, OpenAI, data retrieval, automation
