# Workflow Analysis for LINE Chatbot with Memory

## Description
This workflow creates a LINE chatbot that can remember past conversations with users by storing and retrieving messages from a database. It allows for continuous and context-aware interactions.

## Input Details
The workflow is triggered by an incoming message to a LINE chatbot via a webhook.

## Process Summary
The workflow receives a LINE message, then retrieves the user's conversation history from a PostgreSQL database. It sends the current message and past messages to a large language model (LLM) to generate a response. The LLM's response and the user's message are then saved to the PostgreSQL database to maintain the conversation history. Finally, the generated response is sent back to the user via LINE.

## Output Details
The workflow sends a message back to the LINE user, providing a context-aware response based on the conversation history.
