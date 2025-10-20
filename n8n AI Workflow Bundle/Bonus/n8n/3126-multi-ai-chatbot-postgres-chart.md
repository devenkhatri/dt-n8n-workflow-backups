# Workflow Analysis for Multi-AI Chatbot with Postgres Chart Integration

## Description
This workflow enables a multi-AI chatbot that can interact with users, remember conversation history, and generate charts based on user queries, storing chat data in a PostgreSQL database.

## Input Details
The workflow is triggered by an HTTP POST request containing chat messages.

## Process Summary
The workflow receives a user message and a unique conversation ID. It retrieves the chat history from PostgreSQL, adds the new message, and sends the updated history to a selected AI model (OpenAI or Mistral AI). The AI's response is then analyzed for chart-related keywords. If keywords are found, a Python script generates a chart, which is then uploaded to an S3 bucket and a URL sent back to the chatbot.

## Output Details
The workflow sends the AI's response, potentially including a chart image URL, back as an HTTP response.
