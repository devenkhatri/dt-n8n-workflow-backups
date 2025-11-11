# Workflow Analysis for Knowledge store agent (with Google Drive)

## Description
This workflow creates a chat-enabled AI agent that answers user questions by retrieving and analyzing information from documents stored in a Google Drive folder. New files added to the folder are automatically processed and stored in a vector database for semantic search.

## Input Details
The workflow is triggered by new file uploads to a specific Google Drive folder and by incoming chat messages via a webhook.

## Process Summary
When a file is uploaded to the designated Google Drive folder, it is automatically downloaded and processed into document chunks using a default data loader. These chunks are then embedded using an OpenAI embedding model and stored in an in-memory vector store. When a chat message is received, the AI agent uses the same embedding model to perform a semantic search against the vector store, retrieves the most relevant documents, and generates an answer based on the retrieved content using a GPT-4o language model with conversation memory.

## Output Details
The workflow sends AI-generated responses to user chat messages based on the information retrieved from stored Google Drive documents.

## Tags
AI Agent, Google Drive, Vector Store, Document Processing, Chatbot, Embeddings, Retrieval Augmented Generation, Knowledge Base
