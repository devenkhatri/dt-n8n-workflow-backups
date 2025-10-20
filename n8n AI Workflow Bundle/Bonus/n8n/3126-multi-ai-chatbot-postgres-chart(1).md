# Workflow Analysis for Multi AI Chatbot with Postgres and Chart Generation

## Description
This workflow enables an AI chatbot that can interact with users, store conversation history in a PostgreSQL database, and generate charts based on user queries.

## Input Details
The workflow is triggered by an HTTP POST request to a webhook, receiving chat messages from a user.

## Process Summary
Upon receiving a user message, the workflow extracts the message and user ID. It then retrieves previous chat history for the user from a PostgreSQL database. The current message and history are sent to a large language model (LLM) to generate a response. If the LLM response indicates a chart request, the workflow extracts chart data, creates a chart image using QuickChart, and sends the image and text response back to the user. Finally, the interaction (user message and LLM response) is saved to the PostgreSQL database.

## Output Details
The workflow responds to the originating webhook with the chatbot's text response and, if applicable, a generated chart image.
