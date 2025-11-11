# Workflow Analysis for Joke agent (with HTTP tool)

## Description
This workflow creates a fun and interactive joke bot that responds to user messages by fetching and delivering jokes from a public joke API. The bot can adapt its humor based on user preferences and uses conversation memory to keep interactions engaging and non-repetitive.

## Input Details
The workflow is triggered when a chat message is received via a webhook.

## Process Summary
The workflow starts when a user sends a chat message. The message is processed by an AI-powered 'Joke agent' that uses a configured language model, short-term memory, and access to two HTTP tools. One tool fetches jokes from the JokeAPI, while the other retrieves the API’s documentation to help the agent understand available joke filters. Based on the user's request, the agent decides whether to call the joke API, formats a humorous response, and sends it back to the user.

## Output Details
The workflow returns a chat message containing a joke or humorous response, delivered back to the user through the chat interface.

## Tags
chatbot, joke, humor, AI agent, HTTP tool, OpenAI, LangChain
