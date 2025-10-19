# Workflow Analysis for OpenAI Assistant Chat with Memory

## Description
This workflow facilitates a conversational AI chat experience by leveraging OpenAI to generate responses and a memory system to maintain context across interactions. Users can interact with the AI assistant, and the system remembers previous conversation turns.

## Input Details
The workflow is triggered by an HTTP POST request containing a "question" from the user.

## Process Summary
The workflow starts by retrieving the current conversation history from a Google Sheet. It then combines the new user question with the history and sends this to OpenAI for a completion. After receiving the AI's response, a function node formats the conversation history to include both the user's input and the AI's reply. Finally, the updated conversation history is saved back to the Google Sheet.

## Output Details
The workflow returns the AI assistant's response to the user via the HTTP request, and saves the updated conversation history to a Google Sheet.
