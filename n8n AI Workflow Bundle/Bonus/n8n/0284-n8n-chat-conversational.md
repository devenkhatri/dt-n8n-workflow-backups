# Workflow Analysis for Conversational AI Chatbot with OpenAI and Google Search

## Description
This workflow creates a conversational AI chatbot that uses OpenAI to generate responses and Google Search to find information, allowing dynamic and informed conversations.

## Input Details
This workflow is triggered manually and does not receive any external data.

## Process Summary
The workflow starts by manually receiving user input. It then generates an OpenAI chat completion with the user question and the conversation history. If the OpenAI response indicates a need for a Google search, the workflow performs one with the specified query. Finally, it formats the message to include the search results if available, and updates the chat conversation with the latest interaction.

## Output Details
The workflow outputs the formatted chatbot response, which is then used to update the conversation history.
