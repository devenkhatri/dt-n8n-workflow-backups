# Workflow Analysis for Chat with local LLMs using n8n and Ollama

## Description
This workflow enables interactive chat with self-hosted Large Language Models (LLMs) via Ollama, allowing users to send prompts and receive AI-generated responses through a chat interface.

## Input Details
The workflow is triggered when a chat message is received via a webhook from the n8n chat interface.

## Process Summary
The workflow starts by capturing the user's input message from the chat interface. It then passes this input to the 'Chat LLM Chain' node, which communicates with the locally hosted Ollama server using the configured Ollama Chat Model. The LLM processes the prompt and generates a response. The workflow returns this AI-generated response back to the chat interface for the user to see.

## Output Details
The workflow delivers the AI-generated response from the local LLM back to the user through the chat interface.

## Tags
LLM, Ollama, chat, AI, local AI, n8n chat, self-hosted AI
