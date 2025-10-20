# Workflow Analysis for Multi AI Chatbot with PostgreSQL and Chart Generation

## Description
This workflow orchestrates a multi-AI chatbot interaction, stores chat history in a PostgreSQL database, and visualizes data using QuickChart.

## Input Details
The workflow is triggered by an incoming webhook, receiving chat messages as input.

## Process Summary
The workflow receives a user message and a session ID. It retrieves the chat history for the session from PostgreSQL, then generates a response using a GPT-3.5-turbo AI model. The chat history is updated with the new interaction. If the AI response includes a chart request, a QuickChart image is generated. Finally, the AI response and possibly the chart image are sent back.

## Output Details
The workflow returns the AI chatbot's response, potentially including a generated chart image, to the webhook caller.
