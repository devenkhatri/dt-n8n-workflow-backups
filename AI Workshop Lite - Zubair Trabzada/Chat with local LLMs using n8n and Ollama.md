# Workflow Analysis for Chat with local LLMs using n8n and Ollama

## Description
This n8n workflow enables users to interact with self-hosted Large Language Models (LLMs) via a chat interface, leveraging Ollama to manage local LLMs, send prompts, and receive AI-generated responses directly within n8n.

## Input Details
The workflow is triggered by a chat message received through a chat interface.

## Process Summary
The workflow starts by capturing a user's input from the chat interface. This input is then passed to the "Chat LLM Chain" node, which utilizes the "Ollama Chat Model" to send the prompt to a local Ollama server. Ollama processes the input with a self-hosted LLM and generates a response. Finally, the "Chat LLM Chain" delivers this AI-generated response back to the chat interface.

## Output Details
The workflow delivers the AI-generated response from the local LLM back to the originating chat interface.
