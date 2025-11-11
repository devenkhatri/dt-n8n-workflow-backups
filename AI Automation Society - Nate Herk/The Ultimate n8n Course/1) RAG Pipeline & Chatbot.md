# Workflow Analysis for RAG Pipeline & Chatbot

## Description
This workflow automatically processes new files added to a Google Drive folder by embedding their content into a Pinecone vector database, enabling a chatbot to retrieve and use this information to answer user questions intelligently.

## Input Details
The workflow is triggered when a new file is created in a specific Google Drive folder and also receives user messages via a chat interface.

## Process Summary
When a new file is added to the designated Google Drive folder, it is automatically downloaded. The file content is then loaded, split into manageable text chunks, and converted into vector embeddings using OpenAI. These embeddings are stored in a Pinecone vector database under the 'FAQ' namespace. Separately, when a user sends a chat message, the AI agent uses the same Pinecone database as a knowledge tool—querying it with OpenAI embeddings—to retrieve relevant information and generate informed responses using the Claude 3.5 Sonnet model via OpenRouter.

## Output Details
The workflow enables an AI chatbot to provide contextual, knowledge-based responses to user queries by leveraging the indexed documents from Google Drive, with responses generated through the OpenRouter API.

## Tags
RAG, chatbot, Google Drive, Pinecone, OpenAI embeddings, vector database, document processing, AI agent, OpenRouter, Claude
