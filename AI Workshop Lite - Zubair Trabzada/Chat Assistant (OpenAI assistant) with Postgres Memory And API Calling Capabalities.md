# Workflow Analysis for modelo do chatbot

## Description
This workflow powers an AI chatbot that collects user information, stores conversation history, and provides contextual responses by querying external tools such as a product database, knowledge base, and third-party APIs.

## Input Details
The workflow is triggered by a chat message sent via a public webhook, which includes user input and a session ID.

## Process Summary
When a chat message arrives, the workflow checks if lead data is present. If so, it formats a personalized introduction message containing the user's details and sends it to an OpenAI assistant with access to short-term chat memory. If no lead data is present, it routes the raw user input to a different OpenAI assistant configured with long-term memory and connected to multiple tools. These tools include a PostgreSQL chat memory, a MySQL product database query, an external HTTP knowledge base, and a third-party API for user verification. The assistant uses these tools to generate informed, contextual responses.

## Output Details
The workflow returns an AI-generated response to the user via the chat interface, while also storing conversation history in a PostgreSQL database.

## Tags
chatbot, OpenAI, PostgreSQL, MySQL, API integration, AI assistant, memory, lead data, health insurance
